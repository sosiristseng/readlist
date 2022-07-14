---
title: "Bazil 2017: Analysis of a Functional Dimer Model of Ubiquinol Cytochrome c Oxidoreductase
"
subtitle: ""
date: 2022-07-14T13:21:31+08:00
draft: false
author: ""
authorLink: ""
description: ""

tags: ["complex 3", "ROS", "mitochondria"]
categories: []
series: ["ETC review"]
seriesNavigation: true

featuredImage: ""
featuredImagePreview: ""

hiddenFromHomePage: false
hiddenFromSearch: false

twemoji: false
ruby: true
fraction: true
fontawesome: false

toc:
  enable: true
  auto: true
math:
  enable: true
lightgallery: true
---

[Sciwheel](https://sciwheel.com/work/#/items/6833116) [^Bazil2017]

[^Bazil2017]: Bazil JN. Analysis of a functional dimer model of ubiquinol cytochrome c oxidoreductase. Biophys J. 2017 Oct 3;113(7):1599–612. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5627346/

<!--more-->

## Introduction

Complex III catalyzes the exergonic two-electron oxidation of quinol to the one-electron reduction of cytochrome c. The enzyme operates using a Q-cycle mechanism whereby electron flow is bifurcated. 

Although other mathematical models of the bc1 complex exist (30, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51), they are too complex to integrate into larger-scale metabolic models (47, 48, 49), do not include free radical production (39, 40, 41, 42, 43, 44, 45, 46, 48), are not thermodynamically constrained (30, 42, 43, 44, 45, 46, 50, 51), or simulate a limited range of conditions (30, 41, 42, 43, 44, 45, 46, 48). 

We previously showed that a simple monomer model was sufficient to explain a majority of the kinetic data (53). However, simulating free radical production in addition to the available kinetic data requires a dimer model.

## Model

![fig1](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5627346/bin/gr1.jpg "Model diagram of the bc1 dimer")

- The model is based on a functional dimer mechanism (31) with each monomer containing four redox centers.
- QH2 oxidation at the Qp site is the rate-limiting step
- effect of pH
- In the dimer, the electrons equilibrate on the complex through the heme bL-bL electronic bus bar (i.e., electron bridge)
- However, model simulations reveal an extremely low occupancy of states past five electrons on eight redox centers due to Columb repulsions. Therefore, only six electronic states are considered (oxidized plus up to the five-electron state).
- The fractional substates of these redox centers for each electronic state are computed using the Boltzmann distribution.
- The steady-state equation for the six-state model was solved analytically using MATLAB’s symbolic toolbox.

## Data

To calibrate the model, we used a wide variety of data from the literature. These data consist of kinetic data (41, 43, 44, 55, 56) in addition to data on superoxide production rates (28, 57) and dimeric function (31). We also included additional data to constrain the maximum rate of antimycin A-stimulated free radical production (58) in mammalian mitochondria.

A custom, parallelized simulated annealing algorithm was used to globally search the parameter space before identifying a local minimum with a gradient-based local optimizer. [Code link](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5627346/bin/mmc2.zip)

## Results

![Fig2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5627346/bin/gr2.jpg "Cytochrome c turnover and superoxide production rate by the bc1 complex reconstituted in liposomes")

![Fig3](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5627346/bin/gr3.jpg "Free radical production rates by bc1 complex in submitochondrial particles and intact mitochondria")
- The model simulates maximum levels of superoxide production when the Q pool is approximately half-oxidized.
- The *semireverse mode* of superoxide production occurs when the reduced heme bL reduces Q at the Qp site to form the unstable SQ that reacts with O2. (States E1 through E4)
- The *semiforward mode* of superoxide production occurs when QH2 is oxidized whereas heme bL is reduced, leaving an unstable SQ at the Qp site. (State E5 in the model)

## Antimycin A

The ability of antimycin A to stimulate cytochrome c reduction by the bc1 complex is compelling evidence for cross-monomer electron equilibration. Only a single antimycin A molecule is bound to the dimer, cytochrome c reduction is stimulated. This is only possible if the enzyme operates as a functional dimer with electron equilibration between monomers.

![Fig4](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5627346/bin/gr4.jpg "Antimycin-stimulated cytochrome c reduction")

## Native Q10

![Fig5](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5627346/bin/gr5.jpg "Physiological behavior of bc1 dimer")

Superoxide is primarily produced through the three- and four-electron reduced states (semireverse mechanism). Superoxide production from the five-electron reduced state (semiforward mechanism) is only important in the antimycin A-inhibited state.

## Physiological Q-pool operating range and cardiac bc1 content

![Fig6](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5627346/bin/gr6.jpg "Model predictions of bc1 content and Q-pool redox state during various bioenergetics states")

## Conclusion

This model
- Capable of simulating the enzyme kinetics under a wide range of conditions
- Calibrated with superoxide production data obtained using the purified complex and antimycin A-treated mitochondria
- Coulombic effects between intramonomer heme bL and heme bH and between intermonomer heme bL and heme bL were required to fit the data with a single, consistent set of parameters.
- Semireverse mode of superoxide production constitutes the major mechanism of free radical production by the bc1 complex.
- Under physiological conditions, the Q pool is primarily in the oxidized state. In the presence of succinate or under pathological conditions (e.g. hypoxia), it can reach a significantly reduced state.
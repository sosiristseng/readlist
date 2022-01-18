---
title: "Fridlyand 2010 : Glucose sensing in the pancreatic beta cell: a computational systems analysis"
subtitle: ""
date: 2021-07-20T22:10:49+08:00
draft: false
author: ""
authorLink: ""
description: ""

tags: ["mitochondria", "mitochondrial dynamics", "ATP", "beta-cell", "glycolysis", "calcium", "differential equations"]
categories: ["Reading"]
hiddenFromHomePage: false
hiddenFromSearch: false

featuredImage: ""
featuredImagePreview: ""

toc:
  enable: true
lightgallery: true
---

[Sciwheel](https://sciwheel.com/work/#/items/7974655)[^Fridlyand2010],  [PMC2896931](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/)

[^Fridlyand2010]: Fridlyand LE, Philipson LH. Glucose sensing in the pancreatic beta cell: a computational systems analysis. Theor Biol Med Model. 2010 May 24;7:15.

<!--more-->

## Background

Glucose-stimulated insulin secretion (GSIS) model:

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-1.jpg "Schematic diagram")

Pyruvate is the main end product of glycolysis in β-cells and essential for mitochondrial ATP synthesis.

An important β-cell specialization is the very low expression of lactate dehydrogenase (LDH).

Re-oxidizing cytoplasmic NADH by two mitochondrial hydrogen shuttles: the malate-aspartate shuttle and the glycerol phosphate shuttle.

The respiratory rate is lower and relative leak activity is higher in isolated β-cell mitochondria.

Glycolytic flux is mainly controlled by glucokinase reaction.

Previous work
- Magnus and Keizer: examining the possible mechanisms underlying oscillations in pancreatic β-cells
- [Nan Jiang](https://www.ncbi.nlm.nih.gov/pmc/articles/instance/1998884/bin/335_2007_9011_Fig1_HTML.jpg): too complex (44 reactions).


This model has qualitative properties consistent with expectations for the pancreatic β-cell including showing appropriate oscillations in mitochondrial metabolism and Ca2+ concentration.

## Results and Discussion

### Steady state stimulation with a step increase in glucose concentration

[Table1](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/table/T1/): timulated steady-state values for low glucose (5 mM)

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-2.jpg "Effect of increasing glucose on cell energetics")

The rise in ATP/ADP ratio as well as in relative NAD(P)H, Ψm, [Ca2+]m and oxygen consumption were also observed with glucose stimulation in control INS-1 cells.

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-12.jpg "Relative steady-state ATP production activity with respect to Ψm")
Relative rate of phosphorylation (□) was based on experimental data [131] for human cell line mitochondria

### Decreased Ψm and respiratory activity regulate mitochondrial glucose sensitivity in β-cells

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-3.jpg "Comparison with muscle cell mitochondria")
- increased step by step the maximal rate of respiration (Vme, Equation 5) from basal β-cell level (arrow)

### Changes in leak activity and the role of uncoupling agents

Decreased leak activity increased Ψm and reduced the sensitivity range of the inner membrane potential to glucose leading to a left-shift in the ATP/ADP ratio and $\ce{[Ca^2+]}_c$ response.

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-4.jpg "Effect of increasing glucose at different leak activity")

The shifting set-point mechanism would regulate insulin secretion particularly during a fluctuating nutrient supply.Either an under or over-expression of UCP2 may lead to a failure of β-cells to properly respond to glucose.

### Role of Lactate dehydrogenase (LDH) and lactate production

The simulated lactate production increased significantly in response to high glucose. This can be accounted for by increased $\ce{[NADH]}_c$/$\ce{[NAD+]}_c$.

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-5.jpg "Model parameters in response to changes of lactate dehydrogenase activity")

Low levels of LDH expression in insulin-secreting cells are important for the correct channeling of pyruvate towards mitochondrial metabolism

### Role of NADH in cytoplasm and shuttle activity

Changes in cytoplasmic redox level could be manifested primarily through variation in $\ce{[NADH]}_c$. NADH generated by glycolysis was efficiently reoxidized by highly active mitochondrial shuttles rather than by lactate dehydrogenase in basal conditions in our model

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-6.jpg "Model parameters in response to changes of the transport rate coefficient for NADH shuttles")

NADH shuttle are important for coupling glycolysis and OXPHOS.

### Role of calcium

Mitochondrial Ca2+ concentration as an accelerator of ATP production.

Mitochondrial Ca2+ influx as a suppressor of ATP production is not supported in beta-cell data. The contribution of Ca2+ cycling to proton leak was estimated to be only about 1% of the state 3 rate.

Regulation of cytoplasmic Ca2+ concentration by [Ca2+]m:
- Cardiomyocytes: 58.5% cytosolic and 36% mitochondrial volumes. Mitochodria are large buffer of Ca.
- β-cell mitochondrial volumes ranged from only 4% to 8% per cell. Mitochodrial buffering is limited.


**ER** volume can be up to 20% of total β-cell volume.

### Suppression of respiratory activity

Increased [NADH]m with decreased Vme, however, Ψm, ATP production, respiration rate, ATP/ADP ratio and [Ca2+]c were also decreased.

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-8.jpg "Model parameters in response to changes of the maximal rate of proton pumping in ETC")

### Suppression of F1F0 ATPase activity


![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-9.jpg "Model parameters in response to changes of the maximal rate of proton flux in F1F0 ATPase")

## Oscillation processes

Oscillations in cytoplasmic and mitochondrial metabolism, membrane potential, intracellular and mitochondrial Ca2+ due to increased glucose concentrations has been described as a specific characteristic of glucose signaling in the β-cell.

For ease of use here we employed a simplified mathematical model that created a periodically varied [Ca2+]c in the cytoplasm.

![](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2896931/bin/1742-4682-7-15-11.jpg "Model-predicted dynamic responses of parameters in pancreatic β-cells for independent [Ca2+]c oscillations at 9 mM glucose concentration")

The metabolic and membrane variables in the cytoplasm and mitochondrial matrix can display oscillatory behavior when [Ca2+]c oscillated independently.

Each [Ca2+]c increase during oscillations:
- increased cytoplasmic ATP consumption and thus increased ADP
- amplification of ATP synthesis by the mitochondrial F1F0 ATPase
- decrease in Ψm
- increases ETC activity
- enhanced [NADH]m consumption and the respiration rate (O2 consumption).

## Regulation of ROS content in β-cells

β-cells have relatively low levels of free radical detoxifying and redox-regulating enzymes such as superoxide dismutase, glutathione peroxidase, catalase and thioredoxin.

- ROS may also subserve a signaling function.
- β-cells usually work at a relatively lower Ψm (< 160 mV) compared with other types of cells. Low ROS production.
- increased sensitivity of β-cell mitochondria to damage.

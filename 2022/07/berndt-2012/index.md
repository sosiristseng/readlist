# Berndt 2012: Kinetic Modeling of the Mitochondrial Energy Metabolism of Neuronal Cells


[Sciwheel](https://sciwheel.com/work/#/items/6062859) [^Berndt2012]

[^Berndt2012]: Berndt N, Bulik S, Holzhütter H-G. Kinetic Modeling of the Mitochondrial Energy Metabolism of Neuronal Cells: The Impact of Reduced α-Ketoglutarate Dehydrogenase Activities on ATP Production and Generation of Reactive Oxygen Species. Int J Cell Biol. 2012 Jun 10;2012:757594. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/

<!--more-->

## Introduction

The citric acid cycle is catalyzed by eight enzymes, among which α-Ketoglutarate Dehydrogenase complex (KGDHC) has the lowest activity. Thus, KGDHC is considered one of the rate-limiting enzymes in the tricarbonic acid cycle (TCAC). 

## Model

The model consists of *184 state variables* describing the neuronal citric acid cycle, the respiratory chain, the oxidative phosphorylation, the mitochondrial ATP generation, the nucleotide exchange between the mitochondrial matrix and the cytosol, and the electrophysiological coupling between the pathways.

- citric acid cycle
- OXPHOS
- ANT
- Exchangers / ion channels on the inner mitochondrial membrane (IMM)

![Fig1](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.001.jpg "Schematic of the full model")

![Fig2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.002.jpg "Schematic of the respiratory chain")

The functional parts of complex I are the flavine mononucleotide (FMN), eight iron-sulfur clusters (i.e., N3, N1a, N1b, N4, N5, N6a, N6b, and N2), and the docking site for ubiquinone. Model simulations show that lumping together the complexes N1b, N4, N5, N6a, and N6b gives similar results as the full model but reduces the number of state variables from 1536 to 96.

Each state of complex III is described as an array describing the reduction and binding states of its functional parts: cytochrome c1 (c1), the iron sulfur cluster (Fe-S), the binding site for ubisemiquinone at p-site (SQp), the low b-type heme (bL), the high b-type heme (bH), and the binding site for ubisemiquinone at n-site (SQn).

It is assumed that electrons are transferred from ubiquinol at p-side in a two-step process, first reducing the Fe-S and binding of SQp and afterward reducing bL, and release of Qp. As long as SQp is bound, Fe-S cannot transfer the electron to c1. This gives 48 state variable and 88 reactions for complex III.

![Fig4](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.004.jpg "System characteristics under energetic challenge")

Since multiple sites for mitochondrial ROS production in complex I and complex III have been suggested in the literature, we monitored the occupation states of the disputed ROS producing sites at varying ATP consumption rate. We concluded that the fully reduced flavin, the semi-ubiquinone bound at n-site in complex I, and the semiubiquinone bound at p-site in complex III are in agreement with expected dependencies on the membrane potential, while the flavin radical and the semiubiquinone at p-site can be ruled out as main ROS producers.

![Fig5](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.005.jpg "Potential ROS producing states in the RC")

## Reduced KGDHC Activities

![Fig6](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.006.jpg "System characteristics under KGDHC inhibition")

![Fig7](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.007.jpg "Mitochondrial membrane potential characteristics at inhibition of KGDHC")

![Fig8](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.008.jpg "NADH level characteristics at varying ATP demand and KGDHC inhibition")

![Fig9](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.009.jpg "NADH level comparison experiment and simulation")

![Fig10](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3376505/bin/IJCB2012-757594.010.jpg "ROS production at inhibition of KGDHC")

With increasing degree of KGDHC inhibition, there was a remarkable reduction in the occupation state of the fully reduced flavin in complex I as well as SQp of complex III at all workloads.

## Discussion

Decreased KGDHC activity in neuronal cells of the brain is associated with a number of neurodegenerative diseases.

Our model simulations showed a steady decline of the mitochondrial NADH level with progressive KGDHC inhibition, whereas up to 95% inhibition of the aconitase had virtually no impact. A reduced NADH content does not translate linearly to reduced energy production. Aconitase shows the highest susceptibility towards ROS, because of its sulfur-iron complex, but aconitase inhibition remains irrelevant if it does not exceed 90 percent.  KGDHC is tightly bound to the inner mitochondrial membrane and might be part of a citric acid cycle super-complex. It binds to complex I of the mitochondrial respiratory chain, which might make it a prominent target of ROS. Thus, ROS is one possible reason for KGDHC deficiency.

Since akg is in equilibrium with glutamate by a deaminase reaction, this might lead to glutamate poisoning, another pathological feature associate with KGDHC inhibition.



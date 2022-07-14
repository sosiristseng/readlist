# Takeuchi 2020: Integration of mitochondrial energetics in heart with mathematical modelling


[Sciwheel](https://sciwheel.com/work/#/items/12430931)[^Takeuchi2020]

[^Takeuchi2020]: Takeuchi A, Matsuoka S. Integration of mitochondrial energetics in heart with mathematical modelling. J Physiol (Lond). 2020 Apr;598(8):1443–57. https://physoc.onlinelibrary.wiley.com/doi/10.1113/JP276817

<!--more-->

## Introduction

![image](https://user-images.githubusercontent.com/40054455/177813928-a2464c34-e418-4b21-a7ec-f339c25c62c3.png)

In a normal heart, the primary source of ATP is oxidative phosphorylation in mitochondria (>95%), and a small amount of ATP is produced by glycolysis. Acetyl CoA mainly comes from β-oxidation of fatty acids (60−90%), and the remainder comes from pyruvate (10−40%)[^Stanley2005]

[^Stanley2005]: Stanley WC, Recchia FA & Lopaschuk GD (2005). Myocardial substrate metabolism in the normal and failing heart. Physiol Rev 85, 1093–1129.

## Mechanism underlying metabolite constancy during cardiac workload transition

![image](https://user-images.githubusercontent.com/40054455/177815023-031b25cd-1ca2-4e34-b955-85a6491fc4b3.png)

Metabolite stays constant upon workload change (flux adapts pretty fast).

- feedback OXPHOS activation by ADP, versus
- parallel TCA cycle/ETC activation by calcium and/or other unknown factors

### Calcium

No experimental data support the idea that Ca2+ activates multiple metabolic pathways to the same extent.

Cortassa 2003 model: Based on calcium activating Pyruvate dehydrogenase complex (PDHC), 2-oxoglutarate dehydrogenase (OGDH), and isocitrate dehydrogenase (ICDH) in the TCA cycle.

The activation of respiration by Ca2+does not account for the (sarcomere) length–force relationship of heart muscle, which is the basis of the Frank–Starling law of the heart.

Second, in spite of disturbed mitochondrial Ca2+ influx, cardiac function in mice lacking the mitochondrial Ca2+ uniporter (MCU) is unaltered or almost normal.

The contribution of mitochondrial Ca2+ to cardiac respiration is minor, if any.

### Compartmentalized energy transfer systems

Saks models: micro-compartments defined as intracellular energetic units (ICEUs). Metabolite constancy during cardiac workload transition can be achieved by assuming a *compartmentalized MtCK-ANT*-voltage dependent anion channel coupling system.
- ADP produced by myosin ATPase can readily be transferred to the cytosolic CK system
- Functional coupling between MtCK and ANT decreases the reactive oxygen species (ROS) production in mitochondria

But, CK system is dispensable for (mouse heart) mitochondrial energetics, structural organization, and intracellular compartmentation in cardiomyocytes.

### Phosphate

Oxidative phosphorylation (OXPHOS) in cardiac mitochondria was activated by Pi via increasing NADH generation, distribution of free energy throughout the cytochrome chain, and ATP synthase. (Beard's models)
- Pi-dependent Complex III activation. But in later experiments, they found Pi does not directly activate Complex III, but it increases overall turnover of oxidative phosphorylation (OXPHOS).
- (In later experiments) baseline Pi concentration is 0.29 mM and maximal Pi concentration during workload increases to 2.3 mM.

### Calcium plus phosphate

![image](https://user-images.githubusercontent.com/40054455/177819037-4b020da5-39f6-4fd9-92e9-dc5e679a5771.png)

[Saito 2016 model](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5275773/). 
- Cacium activates PDHC, ICDH, OGDH, and aspartate-glutamate transporter (AGC).
- Phosphate activates complex III and OGDH.


Sensitivity to Ca/Pi shifted upon substrate change (doing full TCA cycle vs half of the cycle)

![image](https://user-images.githubusercontent.com/40054455/177819293-446ded30-9fdd-4912-980e-ff177a1d1edf.png)

## ROS modeling

ROS generation/scavenging system in cardiac mitochondria in Cortassa's and Gauthier's models: redox-optimized ROS balance hypothesis. There is a middle ground of redox state where the ROS production is minimized (and ATP generation is the most efficient). de Oliveira's model for doxorubicin-mediated cardiotoxicity. 

## Metabolome

[Cortassa](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4286601/) and her colleagues succeeded in establishing a novel procedure for translating metabolite profiles (metabolome) into the set of metabolic fluxes (fluxome). 

Beard, Bazil and their colleagues independently developed thermodynamically consistent kinetic models of mitochondrial ROS production from Complex I and III.

## Cacium dynamics in the mitochondria

Mitochondrial Ca2+ dynamics in the heart is important because Ca2+ is implicated as a possible regulator of mitochondria metabolism, at least for transient changes of NADH. It's also important for opening of the mitochondrial permeability transition pore, apoptosis and cytosolic Ca2+ signalling.

Mitochondrial Ca2+ uniporter (MCU) and the mitochondrial Na+-Ca2+ exchanger (NCLX) are the two major pathways determining mitochondrial Ca2+ dynamics. And other smaller players are
- Rapid mode of Ca2+ uptake
- Ca2+-H+ exchanger
- Ca2+ buffering
- Calcium phosphate precipitation

Other considerations
- Calcium influx is rather complicated (MICU1, MICU2 and EMRE).
- Calcium outflux by NCLX still remain to be elucidated (allosterically regulated by mitochondrial membrane potential?)
- Distinct spatial distributions of MCU and NCLX

## Conclusion

- The role of Ca2+ is limited under physiological conditions.
- Feedback activation by ADP and Pi is likely the main regulatory mechanism of mitochondrial oxidative phosphorylation (OXPHOS).
- But the rise of ADP or Pi is still difficult to detect experimentally.

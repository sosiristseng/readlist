# Li 2012 : Mechanisms by which Cytoplasmic Calcium Wave Propagation and Alternans Are Generated in Cardiac Atrial Myocytes Lacking T-Tubules—Insights from a Simulation Study


[Sciwheel](https://sciwheel.com/work/#/items/6252573) [^Li2012],  [PMC3318133](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3318133/)

<!--more-->

## Introduction
* the mechanisms underlying Ca2+ wave propagation and [Ca2+]i alternans in cardiac myocytes lacking t-tubules (atrial cells in small mammals) are still unclear
* Here: biophysically detailed computer model for Ca2+ release and Ca2+ wave propagation in cardiac myocytes lacking t-tubules

## Methods
### Mathematical model of Ca2+ wave propagation in atrial myocytes
![image](https://user-images.githubusercontent.com/40054455/125468120-ae09920f-001a-4006-9fe7-fa604220e94e.png)
* Adapted from Tao et al. equations to simulate Ca2+-wave propagation in atrial myocytes that lack t-tubules
* A cell divided into 13 elements with a spatial resolution of 2 μm
### Stimulation protocol and simulated intracellular Ca2+-wave propagation
* on each voltage-clamp pulse, Ca2+ influx via VOCCs triggered CICR at the peripheral units, resulting in large [Ca2+]i transients in these regions
* localized [Ca2+]i transients diffused inward toward the central region, provoking successive CICR that led to Ca2+-wave propagation.
* Ca2+ wave did not fully propagate to the center. the [Ca2+]i transients (Fig. 1 B ii) and the SR Ca2+ release (Fig. 1 B iii) were large in the periphery of the cell but small in the central region
* These simulation results matched experimental observations in rat (15,19), guinea-pig (20), and cat (4) atrial myocytes that lack t-tubules.
### Model validation
* sustaining the intracellular Ca2+ waves through increasing Ca2+ influx by elevating the extracellular Ca2+ concentration
* increasing the RyR sensitivity by decreasing the threshold of RyR for CICR
* elevating the SR content by pausing pacing for 10 s while increasing SERCA Ca2+ uptake (Pup increased by 75%) to allow SR Ca2+ content accumulation
* increases in the Ca2+ influx, the RyR sensitivity, or the SR content helped to sustain full Ca2+-wave propagation from the periphery to the center of the cell, producing a more homogeneous [Ca2+]i, similar to experimental results.

## Results
### Effect of increasing Ca2+ influx
* An increase in Ca2+ influx via elevating [Ca2+]o has been shown to help facilitate full Ca2+-wave propagation toward the center region and to reduce the [Ca2+]i spatial heterogeneity in atrial cells
* Also in increasing the maximum channel conductance of the VOCCs (gCaL)

![image](https://user-images.githubusercontent.com/40054455/125468142-1070f737-16c7-4172-8855-60f5133979a5.png)

* There is a time delay in the [Ca2+]i and [Ca2+]SR transients between the peripheral and central regions => propagation rather than synchronized

### Effect of increasing RyR sensitivity
![image](https://user-images.githubusercontent.com/40054455/125468171-932b6305-23ed-4161-9a84-9d305cea3811.png)

* reducing the threshold of RyR for CICR (Krel)
* When Krel was reduced by 10%, a complete Ca2+ wave spreading toward the interior region of the cell was established temporarily. But amplitude is smaller.
* Due to the reduced SR content, propagation of the Ca2+ wave toward the center of the cell was unstable, leading to alternans

### Effect of increased SR content
![image](https://user-images.githubusercontent.com/40054455/125468534-88396069-69a1-41d8-b14c-69007581c4f1.png)
* increased SR Ca2+ content (Fig. 4Bi, lower), leading to a period of complete Ca2+ wave propagation into the center of the cell; then Ca alternans
* enhancing the SR Ca2+ uptake (ii):  hindered the inward Ca2+ wave propagation at first. Then a stable complete Ca2+ wave was observed (Fig. 4 A ii) when the SR Ca2+ content was significantly elevated in both central and peripheral regions
*

### Effect of partial inhibition of SERCA pump
![image](https://user-images.githubusercontent.com/40054455/125468587-c5a94990-20ec-4e4d-aa70-12799d586daf.png)
* SERCA pump rate (Pup) was decreased by 10%: alternans
* increasing the threshold of SERCA Ca2+ uptake (Kup) by 20% + SERCA pump rate (Pup) was increased by 50% : enhanced Ca2+-wave propagation; the amplitude of [Ca2+]i transients was greatly enhanced in the interior region of the cell

## Exploring the mechanisms for Ca2+ alternans

### Ca2+ diffusion
![image](https://user-images.githubusercontent.com/40054455/125468643-05e5409e-592f-44c4-8c8d-694a8514f4d7.png)
* increase of the time constant of the Ca2+ diffusion (τ) => [Ca2+]i alternans (bifurcation)
* complicated pattern of alternans are possible
* cancelling Ca diffusion (rapid equilibrium) eliminates Ca alternans
* Ca diffusion dramatically increased the steepness of dependence on SR Ca content
* Increasing Kup shifted the dependence curve leftward (smaller SR Ca2+ content region)
### Ca2+ influx & RyR sensitivity  & the SERCA pump
![image](https://user-images.githubusercontent.com/40054455/125468691-28c4ac0f-eade-48f7-a508-6976da593a9e.png)
* When gCaL was increased over the range 100%–500% of its control value, a cascade of bifurcations occurred
* More dramatic in the central region than in the peripheral region
* With decreasing Krel, a cascade of bifurcations occurred, leading to [Ca2+]i alternans with various patterns
* When Kup was increased from 100% to 140% of its control value, a cascade of bifurcations was triggered, decreased SR uptake due to increased Kup resulted in a low level of SR Ca2+ content and, consequently, reduced [Ca2+]i transient amplitude
### Spontaneous Ca2+ release
![image](https://user-images.githubusercontent.com/40054455/125468730-4c3d745d-86da-42fe-89e5-eabf1a7e58b9.png)
* Overloading the SR Ca2+ content may produce spontaneous Ca2+ release from the SR
* Increased Ca2+ influx (gCaL increased to 370%) and SERCA pump activity (Pup increased to 150%) => irregular pattern of [Ca2+]i transients

## Discussion
### Findings
* Model validated by its ability to reproduce typical Ca2+-wave propagation patterns of atrial myocytes without t-tubules
* reproduce experimentally observed effects of modulations of various aspects of Ca2+ cycling, such as Ca2+ influx, SERCA pumps (SR Ca2+ uptake), and RyRs (SR Ca2+ release), on spatial distribution of Ca2+ transients
* steep relationship between the SR Ca2+ content and the cytoplasmic Ca2+ concentration due to Ca transient propagation, more prone to Ca alternans
* theoretical exploration of possible associations between the occurrence of Ca2+ alternans and parameters related to calcium handling
* Spontaneous Ca2+ release observed

### Mechanisms of incomplete Ca2+-wave propagation in cardiac cells without t-tubules
### Mechanisms of Ca2+ alternans in cardiac cells devoid of t-tubules


## References
[^Li2012]: Li Q, O'Neill SC, Tao T, Li Y, Eisner D, Zhang H. Mechanisms by which cytoplasmic calcium wave propagation and alternans are generated in cardiac atrial myocytes lacking T-tubules-insights from a simulation study. Biophys J. 2012;102(7):1471-82.


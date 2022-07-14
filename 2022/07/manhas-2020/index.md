# Manhas 2020: Computationally modeling mammalian succinate dehydrogenase kinetics identifies the origins and primary determinants of ROS production


[Sciwheel](https://sciwheel.com/work/#/items/9751911) [^Manhas2020]

[^Manhas2020]: Manhas N, Duong QV, Lee P, Richardson JD, Robertson JD, Moxley MA, et al. Computationally modeling mammalian succinate dehydrogenase kinetics identifies the origins and primary determinants of ROS production. J Biol Chem. 2020 Nov 6;295(45):15262–79. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/

<!--more-->

## Introduction

Succinate dehydrogenase (SDH) is a heterotetrametric protein attached to the mitochondrial inner membrane of eukaryotes and many bacteria. It is both a Krebs cycle enzyme and a member of the mitochondrial electron transport system (ETS).

The flavoprotein subunit SDHA contains a flavin adenine dinucleotide (FAD) covalently bound to one of the active sites. The SDHB subunit contains three iron-sulfur clusters (ISCs): [2Fe-2S], [4Fe-4S], and [3Fe-4S]. Subunits C and D (SDHC and SDHD) contain a single transmembrane cytochrome b heme.
 
In mammalian mitochondria, 11 sites including SDH are known to produce reactive oxygen species (ROS). Complex III is commonly argued as the dominate source of ROS under resting condition, whereas complex I is attributed as the primary source of ROS under many pathological conditions, including ischemia/reperfusion (I/R) injury. However, the role of complex II is less certain.

Recent studies have shown that SDH may significantly contribute to total mitochondrial ROS production in a variety of physiological and pathological settings.
- Complex I and III are inhibited
- Skeletal muscle mitochondria respiring on succinate.
- ROS from SDH promotes the pro-inflammatory phenotype in macrophages and differentiation of helper T cells.

Unfortunately, experimental studies on the origin of ROS production by SDH are inconclusive. 

Our analysis of the model presented herein reveals that although the FAD site does produce ROS, the primary source is the **[3Fe-4S] ISC** under normal physiological conditions.

## Model

![Fig1](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F001.jpg "Overview of the SDH model")

Under normal conditions, succinate oxidation is coupled to quinone reduction and mediated by one- or two-electron reactions. The data used in model fitting and validation are summarized in [Table 1](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/table/T1/). The fixed model parameters consist of many thermodynamic parameters obtained from the literature. All the 19 adjustable parameters ([Table2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/table/T2/)) are in a physiologically suitable range, and nearly all are identifiable. Identifiable parameters are highly sensitive and independent of other parameters.

## Results

![Fig2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F002.jpg "Succinate oxidation rates at varied concentrations of different electron acceptors")

![Fig3](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F003.jpg "Succinate oxidation kinetics in the presence of SDH inhibitors using bovine heart SMP")

![Fig4](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F004.jpg "Maximum ROS produced by SDH occurs at submillimolar concentrations of succinate")

![Fig5](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F005.jpg "Succinate-dependent ROS production of SMPs in the presence of stigmatellin or atpenin")

![Fig6](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F006.jpg "Effects of titrating atpenin and non-SDH dicarboxylate substrates on ROS production by complex II")

![Fig7](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F007.jpg "Effects of varying fumarate/succinate ratios on atpenin and complex III inhibitor induced ROS production")

![Fig8](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F008.jpg "The effects of pH on ROS production rates in the presence of inhibitors")

## Model testing

The experimental data used above to constrain the SDH model lacked sufficient perturbations to the endogenous Q pool to adequately identify some of the Q site–related parameters. Done another experiment to verify the model.

![Fig9](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F009.jpg "Decylubiquinone can directly reduce oxygen and amplify resorufin fluorescence.")

At the lower succinate concentration, adding DQ resulted in a dramatic drop in ROS production by SDH. This is due to a decrease in both the succinate and QH2 concentrations and an increase in fumarate and Q concentrations catalyzed by SDH. The result was predicted by the model.

In contrast, the addition of DQ when the succinate concentration is higher (5 mm) leads to a surprising increase in ROS production. Because Decylubiquinone can directly reduce oxygen and amplify resorufin (ROS reporter) fluorescence.

The model was also corroborated using the experimental data from Grivennikova et al.

![Fig10](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F010.jpg "Model corroboration of ROS production and SDH kinetics")

Model analysis demonstrates that ROS production by SDH occurs in both the “forward” and “reverse” modes. It does not matter where the electrons come from: either succinate in the forward mode or QH2 in the reverse mode.

![Fig11](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F011.jpg "Model prediction of site-specific ROS production when the enzyme oxidation state is determined by the Q pool redox state.")
- When the Qp site is inhibited, superoxide derived from the flavin radical is the primary source of ROS.
- When the flavin site is inhibited, most of the total ROS originates from the [3Fe-4S] iron0-sulfur cluster.

To test the model's ability to simulate ROS production from intact mitochondria, it was integrated into a recent model of oxidative phosphorylation ([Malaya's model](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6336351/)).

## Model predicts the [3Fe-4S] ISC is the primary source of ROS

![Fig12](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7650251/bin/SB-JBCJ200583F012.jpg "Model simulations of succinate and ROS turnover of SDH as a function of succinate/fumarate and QH2/Q ratios")

## Discussion

In SDH, the two major sites for ROS production are proposed to be the covalently bound FAD and the Q site. The [3Fe-4S] ISC site has recently been suggested to produce ROS.

Factors that make SDH produces ROS
- Highly reduced Q pool
- Increased pH

This model is an alegebraic equations rather than systems of differential equations with state variables. Thus this model is more computationally tractable for large-scale simulations.

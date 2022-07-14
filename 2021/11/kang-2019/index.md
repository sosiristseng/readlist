# Kang 2019: Exposing the Underlying Relationship of Cancer Metastasis to Metabolism and Epithelial-Mesenchymal Transitions


[Sciwheel](https://sciwheel.com/work/#/items/9267342)[^Kang2019], [PMC5835768](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5835768/)

<!--more-->

![Graphical Abstract](https://user-images.githubusercontent.com/40054455/142387555-99f12e86-7bd8-4003-9e1e-6d9aa8d4de05.png "Graphical Abstract")

## Introduction

Cancer cells often use glycolysis to generate energy, whereas normal cells use glucose for oxidative phosphorylation (OXPHOS). This phenomenon is called Warburg effect (Munozpinedo et al., 2012).

Recently, Yu et al. proposed a mathematical model to study the regulations for genes and metabolites on cancer metabolism (Yu et al., 2017), which has been extended to a more complete model in the following work (Jia et al., 2019).

However, the global stability and stochastic dynamics of cancer metabolism remain to be elucidated. More importantly, the connection between metabolism and metastasis remains unclear.

![The Regulatory Network](https://user-images.githubusercontent.com/40054455/142431555-3d37d80b-b8d8-474f-b463-d53dd5312f5c.png "The Regulatory Network")

ODEs describe the time evolution of relative expression levels for each of the 16 genes or metabolites.

Previously, we have developed a partial self-consistent approximation approach to study the stochastic dynamics for high-dimensional systems by the potential landscape theory (Li and Wang, 2013, Li and Wang, 2014a). Here, we improved previous methods and developed a Truncated Moment Equations (TME) approach (see Supplemental Information Section S3 and Section S4). We calculated the steady state probability distribution of the system employing the TME approach and acquired the potential landscape by $U=-lnP_{ss}$


![Landscape and Path for the Metabolism-EMT-Metastasis Model Shown in ZEB, HIF-1, and BACH1 Coordinates](https://user-images.githubusercontent.com/40054455/142432421-29672deb-2e07-45a2-84f5-49ef043d6db4.png "Landscape and Path for the Metabolism-EMT-Metastasis Model Shown in ZEB, HIF-1, and BACH1 Coordinates")


Major Model Predictions and supportive Experiments: Table 1

![image](https://user-images.githubusercontent.com/40054455/142432797-30114edc-a9a8-4a3b-96e0-db7331828457.png "Table 1")

## Landscape and Kinetic Paths for EMT and Cancer Metabolism

From the landscape of (epithelial to mesenchymal transition) EMT-metabolism, we identified three attractors (cell states), which characterize the epithelial (E), the mesenchymal (M), and an intermediate abnormal metabolic (A) state.

![image](https://user-images.githubusercontent.com/40054455/142433009-f08376c1-c03e-41c8-91b0-61565cd2e115.png "The Tristable Landscape for EMT-metabolism Model and Comparisons with Experimental Data")

To investigate the transition dynamics for the EMT-metabolism system, we calculated the MAPs among different attractors by minimizing the transition actions L. The MAPs for different transitions are shown on the landscape (Figures 6A and 6B)

## Modeling Anti-Cancer Therapeutic Strategies

![image](https://user-images.githubusercontent.com/40054455/142433384-3d2732d4-28cf-40a1-bed5-5e500e89e009.png "Landscape in Terms of HIF-1 and BACH1 in Response to Different Drugs in Different Levels")

We also found that even very large doses of any of these drugs (last column in Figures 7B–7D) alone cannot induce the cells to the E state completely because there are always other abnormal cell states present. Combined therapy showed a more effective outcome.

Recently, an integrated computational and experimental approach was designed to identify effective therapeutic strategies based on temporal sequencing of multiple drugs from deterministic models (Goldman et al., 2015, Goldman et al., 2019).

## Discussion

We constructed a metabolism-EMT-metastasis regulatory network and identified four stable states from the landscape: epithelial (E), abnormal metabolic (A), mesenchymal (M), and metastatic (Met) cell states. Metastatic cancer cells can be destroyed by altering the underlying landscape such that the metastasis state is no longer a stable state. E.g. EMT-derived breast cancer cells can be induced to differentiate into post-mitotic adipocytes through a combination therapy.

The abnormal metabolism (such as aerobic glycolysis) is critical for activating metastasis.

[^Kang2019]: Kang X, Wang J, Li C. Exposing the Underlying Relationship of Cancer Metastasis to Metabolism and Epithelial-Mesenchymal Transitions. iScience. 2019 Nov 22;21:754–72.


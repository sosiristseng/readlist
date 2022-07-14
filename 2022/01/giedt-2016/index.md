# Giedt 2016: Computational imaging reveals mitochondrial morphology as a biomarker of cancer phenotype and drug response


[Sciwheel](https://sciwheel.com/work/#/items/3131672)[^Giedt2016]

## Abstract

1. cancer cells of different origins, including patient-derived xenografts, express highly diverse mitochondrial phenotypes.
2. a given phenotype is characteristic of a cell population and fairly constant over time
3. mitochondrial patterns correlate with cell metabolic measurements
4. therapeutic interventions can alter mitochondrial phenotypes in drug-sensitive cancers

<!--more-->

## Introduction

Mitochondrial dysfunction has been widely linked to cancer, aging and degenerative diseases[^Nunnari2012]

Mechanistic studies of mitochondrial dynamics in cultured cells have shown that mitochondrial fission and fusion are mediated by *post-translational modifications* in key proteins including Drp1/Fis1 and Mfn1&2/Opa1, respectively.

Mitochondrial phenotype might provide a biomarker for cancer diagnosis and/or treatment.

Morphologic phenotyping of mitochondrial states could be a biomarker (in addition to genomic and protein analyses) for cancer cells for a clinical need.

## Analytical pipeline to assess mitochondrial phenotype

Mitochondrial morphology is highly dynamic over time, as revealed by live imaging of Mito-GFP cells.

![Fig1](https://user-images.githubusercontent.com/40054455/147846143-b022bff9-51c8-40a1-a87c-a18ef40afdea.png "Workflow for processing cell samples")

Conventional fixation methods such as methanol, lyse/fix buffers and rapid freezing resulted in destruction of mitochondrial networks and non-representative samples. Instead, we used a cytoskeletal buffer25/4% paraformaldehyde (PFA) solution as a fixative.

A 3-D all-in-focus algorithm combined multiple Z-layers of mitochondria into a single image.

![Fig2](https://user-images.githubusercontent.com/40054455/147846207-b3373a73-3fa3-48cf-89f4-2f34368ecb21.png "Representative examples of mitochondrial segmentation and classification")

## Measuring Mitochondrial Heterogeneity in Cultured Human Cancer Cells

![Fig3](https://user-images.githubusercontent.com/40054455/147846226-9066a0b5-c264-4b35-a1ba-e5fdcc1a0527.png "Population level mitochondrial heterogeneity for fixed stained samples")

Interestingly, the fraction of different mitochondria populations, sizes and densities in both OVCA-429 cells and other profiled populations remained remarkably constant over time, at least during the four weeks of observations recorded in this study. This finding provides further evidence that mitochondrial patterns, while stochastic, are pre-programmed as a whole.

## Correlations between mitochondrial phenotype and bioenergetics

![Fig4](https://user-images.githubusercontent.com/40054455/147846434-66179ee2-40a9-4eb8-9cb1-27a910fadf46.png "Metabolic parameters in patient derived xenograft models")

Punctate mitochondria correlated with increased glycolysis levels, decreased oxygen consumption and reduced spare respiratory capacity.

No correlation between mitochondrial phenotype and cellular grown rates in patient-derived samples. Also limited correlation with total protein levels.

## Mitochondrial morphology is an early biomarker of therapeutic intervention

![Fig5](https://user-images.githubusercontent.com/40054455/147846466-ea3c8268-0545-4438-9828-4cb9c08ab3aa.png "Effect of pro-apoptotic treatment on mitochondrial morphology and heterogeneity")

Adding ABT-263 (apoptosis inducer) and cisplatin (chemotherapy substance) to OVCA-429 cells resulted in fragmented (punctate) mitochondrial networks.

The heterogeneity (the distribution curve in the figures) of mitochondrial morphology present in pre-treated samples was retained following treatment with the medians of the curves shifted toward a more punctate phenotype.

Results of cisplatin is in (Fig. S11).

## Fine needle aspirations of tumors allow therapeutic efficacy measurements

![Fig6](https://user-images.githubusercontent.com/40054455/147846493-310004d6-8fc3-42b9-aad3-b54159385444.png "Mitochondrial morphology as a biomarker to assess drug treatment")

In samples drawn following cisplatin treatment, A2780 cells showed considerable mitochondrial fragmentation (albeit with greater heterogeneity than in vitro samples), while A2780 platinum-resistant cells phenotype retained a phenotype similar to their pre-treatment controls.

## Materials and Methods

### Cells

Cell source: breast, ovarian, pancreatic, hematologic, as well as patient-derived cancers cell lines. These cell lines were transduced with a mitochondrial targeted-GFP using a lentiviral construct consisting of mito-PAGFP, where the mitochondrial targeting sequence and GFP were cut and inserted into a pLVX-AcGFP1-C1 Vector backbone.

Cell Fixing:  4% Paraformaldehyde (Electron Microscopy Sciences) dissolved in Cytoskeletal Buffer.

Staining: immunofluorescence staining (TOMM-20 antibody) to mark mitochondria.

### Image collection

Images were collected as a Z-series using a BX-63 Upright Automated Fluorescence Microscope.

100X oil objective at a resolution of 2560 × 2160 pixels using Metamorph Software.

### Image Analysis

Images were analyzed using Matlab scripts developed in house.

### Measuring Oxygen Consumption and Extracellular Acidification

Oxygen Consumption Rate (OCR) and Extracellular Acidification Rate were measured using an XFe96 Extracellular Flux Analyzer (Seahorse Bioscience).

### Animal Models and Fine Needle Aspiration

Nude mice injected with cancer cells

### Cell Viability Assays

Presto Blue Cell Viability reagent

### Western blot

Drp1, Mfn1, Mfn2, Opa1.

### Statistical Analysis

Three separate experiments, each of which included ~50–100 cells.

- Friedman’s rank sums test: to identify any statistical differences among the distributions
- Dunn’s post-hoc test was used to determine group subset differences.
- The p values were considered significant when less than 0.01. (**Not 0.05**)
- Multiple comparison tests were conducted via ANOVA with Tukey’s test with all populations compared to each other.
- Kaplain-Meir curves (survival curves): log-rank test

## Discussion

### Morphological heterogeneity of cancer cell mitochodnrial networks

While previous methods have been utilized to automatically classify mitochondria into various groupings, our work differs in our use of **a 3-D all in focus algorithm**, which allows us to directly compare optically diverse cell types and automatically classify them in a manner consistent with previous work. Comparing heterogeneity of mitochondrial morphology within individual cell lines and among different cell populations in large numbers of cells became possible.

Our analysis of mitochondrial phenotype revealed broad variation both within cell lines and among different cell populations. While mitochondrial morphology and phenotype at the single mitochondria and single cell level is subject to high levels of change and remodeling, **mitochondrial phenotype is stable in cell populations**.

## Mitochondrial morphologies and cell metabolism

shorter and more punctate mitochondria:

1. use glycolysis over oxidative phosphorylation
2. less functional mitochondria in our patient samples

More aggressive tumor phenotypes <=> increased glycolysis levels.

Analysis of mitochondrial morphology proteins including Drp1, Mfn1/2 and Opa1 showed only limited correlation with overall mitochondrial morphology. (They are regulated  by post-trasnlational modifications and protein-protein interactions? That is, they are regulated qualitatively rather than quantitatively.)

Mitochondrial morphology is altered by chemotherapy in previous studies and in this study, resulting in increased fragmentation/the number of punctate mitochondria.

We observed highly heterogeneous responses to the drug treatments, illustrating the need for population level (~ 50-100 cells in this study) analyses as completed here when analyzing the effects of drugs on mitochondrial morphology.

Mitochondrial phenotype *in vivo* might differ from what is observed in cell culture. (The former was more fragmented)

Mitochondrial network phenotype appears to correlate closely with metabolic alterations in cells and may therefore reveal targetable susceptibilities with follow-on protein analyses.

## Reference

[^Giedt2016]: Giedt RJ, Fumene Feruglio P, Pathania D, Yang KS, Kilcoyne A, Vinegoni C, et al. Computational imaging reveals mitochondrial morphology as a biomarker of cancer phenotype and drug response. Sci Rep. 2016 Sep 9;6:32985.
[^Nunnari2012]: Nunnari J, Suomalainen A. Mitochondria: in sickness and in health. Cell. 2012 Mar 16;148(6):1145–59.


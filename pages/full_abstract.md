---
layout: page
title: Project summary
description: Full project summary with references
---

### 1. Introduction
Neuroimaging has contributed considerably to our understanding of brain development and its relationship to cognition and behavior [1,2,3,4,5,6]. Magnetic Resonance Imaging (MRI) has enabled us to non-invasively study growth in children and adolescents. With increasing availability of longitudinal neuroimaging studies [7,8,9,10], we can apply statistical models to longitudinal datasets to study the temporal trajectories of development and illness progression [11,12,13], as well as the interplay between brain and behavior. However, despite advancements in neuroimaging, replicability in research remains a key issue and there is no gold standard to evaluate neuroanatomical correlates of cognition and behavior and their interplay.

Replicability of brain-behavior studies will improve with pre-registration, better study design (e.g. longitudinal studies), better phenotyping, technological advancement which can lead to better quality data and signal to noise ratio, increased sample size afforded by large scale studies, data sharing and open science [14,15]. However, one of the challenges in the field of neuroimaging is that in most cases we lack knowledge about the underlying truth and whether our methods can detect these changes. Simulated datasets are one way that we can test hypotheses and assess whether our current models can capture the complex brain-behavior relationship.

Here, we focus on the critical period of childhood and adolescence, a time of rapid change in physical, emotional, and intellectual growth. We propose a project which consists of three stages: 

* **Stage 1 – Generation of simulated data by the collaborators** 
Multiple independent groups create simulated longitudinal datasets in line with how they think brain development takes place, including the interaction between brain, behavior, and cognition. Each group will work independently and blinded to the approaches and assumptions made by the other groups. The generated simulated datasets will be made freely available to the research community. The code to generate the datasets will not be shared within the first year, to provide researchers the opportunity to test different models.

* **Stage 2 – Generation of models by the community**
The community works on finding underlying models used to generate the simulated datasets. Models generated by the community will be shared with the collaborators.

* **Stage 3 – Evaluation of models by the collaborators**
Collaborators will evaluate how community models correspond to the underlying models of their own simulated datasets, results will be shared in an educational symposium. The code used to create the datasets, as well as the complete datasets (including any data that was excluded due to e.g., simulation of missing or truncation of distributions to better reflect some measures) will be released to the community.  


### 2. Method

Each group with expertise in brain development will simulate longitudinal data independently, based on their understanding of development and its relationship to brain, behavior, and cognition. We focus on global metrics derived from anatomical MRI such as total gray matter volume and cortical thickness as these measures have a good test-retest reliability [16,17], as well as several subcortical regions. 

Each group will simulate three sets of longitudinal data for brain measures such as volume and cortical thickness as well as cognitive and behavioral measures based on their understanding and models of development. These datasets will be released to the research community where different modeling approaches (e.g., linear mixed effects model, cross-lagged panel model) can be used to estimate brain-behavior relationship.

Please follow the following guidelines when you create the datasets, more information about each variable is available in the [data dictionary](./measures.md):
* **Number of subjects**: 10,000
* **Number of waves/time-points per subject:** 7 (about every two years)
* **Age:** 7-20 years
    * Wave 1 – 7-8 years-of-age
    * Wave 2 – 9-10 years-of-age
    * Wave 3 – 11-12 years-of-age
    * Wave 4 – 13-14 years-of-age
    * Wave 5 – 15-16 years-of-age
    * Wave 6 – 17-18 years-of-age
    * Wave 7 – 19-20 years-of-age 
* **Sex:** 0: male (approximately 50%), 1: female (approximately 50%)
* **Cognitive measures:** IQ (mean = 100, standard deviation = 15)
* **Behavioral measures:** internalizing and externalizing symptoms and attention problems scale based on child behavior checklist (CBCL)
* **Autism diagnosis:** 0: no, 1: yes
* **Brain volume measures:** intracranial volume, total gray matter volume, total white matter volume, hippocampal volume, amygdala volume, and cortical thickness of frontal lobe. The units should be in mm<sup>3</sup> for volumetric measures and mm for cortical thickness. Each group determines the starting point and trajectory of each brain measure 
* **Parental Education:** 0: less than 12th grade (5.3%), 1: High School or GED (35.4%), 2: Bachelor’s Degree (25.3%), 3: Master’s or higher degree (34%)

**Attrition/Missing data:** Missing timepoints 20% \
**Effect size, noise:** Each group should decide what effect size and amount of noise they would like to include 

[Back](../index.html)

---
### References

[1] Giedd, J. N, Blumenthal, J, Jeffries, N. O, Castellanos, F. X, Liu, H, Zijdenbos, A, Paus, T, Evans, A. C, & Rapoport, J. L. (1999) Brain development during childhood and adolescence: a longitudinal mri study. Nature neuroscience 2, 861–863.

[2] Casey, B, Tottenham, N, Liston, C, & Durston, S. (2005) Imaging the developing brain: what have we learned about cognitive development? Trends in cognitive sciences 9, 104–110. 

[3] Shaw, P, Greenstein, D, Lerch, J, Clasen, L, Lenroot, R, Gogtay, N, Evans, A, Rapoport, J, & Giedd, J. (2006) Intellectual ability and cortical development in children and adolescents. Nature 440, 676–679. 

[4] Luders, E, Toga, A. W, Lepore, N, & Gaser, C. (2009) The underlying anatomical correlates of long-term meditation: larger hippocampal and frontal volumes of gray matter. Neuroimage 45, 672–678. 

[5] Raznahan, A, Shaw, P, Lalonde, F, Stockman, M, Wallace, G. L, Greenstein, D, Clasen, L, Gogtay, N, & Giedd, J. N. (2011) How does your cortex grow? Journal of Neuroscience 31, 7174–7177. 

[6] Pelphrey, K. A, Shultz, S, Hudac, C. M, & Vander Wyk, B. C. (2011) Research review: constraining heterogeneity: the social brain and its development in autism spectrum disorder. Journal of Child Psychology and Psychiatry 52, 631–644. 

[7] Van Essen, D. C, Ugurbil, K, Auerbach, E, Barch, D, Behrens, T. E, Bucholz, R, Chang, A, Chen, L, Corbetta, M, Curtiss, S. W, et al. (2012) The human connectome project: a data acquisition perspective. Neuroimage 62, 2222–2231. 

[8] Sudlow, C, Gallacher, J, Allen, N, Beral, V, Burton, P, Danesh, J, Downey, P, Elliott, P, Green, J, Landray, M, et al. (2015) Uk biobank: an open access resource for identifying the causes of a wide range of complex diseases of middle and old age. PLoS medicine 12, e1001779. 

[9] Volkow, N. D, Koob, G. F, Croyle, R. T, Bianchi, D. W, Gordon, J. A, Koroshetz, W. J, P ́erez-Stable, E. J, Riley, W. T, Bloch, M. H, Conway, K, et al. (2018) The conception of the abcd study: From substance use to a broad nih collaboration. Developmental cognitive neuroscience 32, 4–7. 

[10] Karcher, N. R & Barch, D. M. (2021) The abcd study: understanding the development of risk for mental and physical health outcomes. Neuropsychopharmacology 46, 131–142. 

[11] Giedd, J. N & Rapoport, J. L. (2010) Structural mri of pediatric brain development: what have we learned and where are we going? Neuron 67, 728–734. 

[12] Sadeghi, N, Prastawa, M, Fletcher, P. T, Wolff, J, Gilmore, J. H, & Gerig, G. (2013) Regional characterization of longitudinal dt-mri to study white matter maturation of the early developing brain. Neuroimage 68, 236–247. 

[13] Gilmore, J. H, Knickmeyer, R. C, & Gao, W. (2018) Imaging structural and functional brain development in early childhood. Nature Reviews Neuroscience 19, 123–137. 

[14] White, T., Blok, E. and Calhoun, V.D., 2022. Data sharing and privacy issues in neuroimaging research: Opportunities, obstacles, challenges, and monsters under the bed. Human Brain Mapping, 43(1), pp.278-291.

[15] Nichols, T.E., Das, S., Eickhoff, S.B., Evans, A.C., Glatard, T., Hanke, M., Kriegeskorte, N., Milham, M.P., Poldrack, R.A., Poline, J.B. and Proal, E., 2017. Best practices in data analysis and sharing in neuroimaging using MRI. Nature neuroscience, 20(3), pp.299-303.

[16] Wonderlick, J, Ziegler, D. A, Hosseini-Varnamkhasti, P, Locascio, J, Bakkour, A, Van Der Kouwe, A, Triantafyllou, C, Corkin, S, & Dickerson, B. C. (2009) Reliability of mri-derived cortical and subcortical morphometric measures: effects of pulse sequence, voxel geometry, and parallel imaging. Neuroimage 44, 1324–1333. 

[17] Madan, C. R & Kensinger, E. A. (2017) Test–retest reliability of brain morphology estimates. Brain informatics 4, 107–121. 

---

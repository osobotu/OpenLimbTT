# OpenLimbTT
An Open-Source transtibial residual limb anatomic dataset

**DOI:** [![DOI](https://img.shields.io/badge/doi-10.1101/2024.11.27.24317622-brightgreen)](https://doi.org/10.1101/2024.11.27.24317622)
**Data License:** [![License](https://img.shields.io/badge/license-CC--BY--SA--4.0-green)](../main/DATA-LICENSE)
**Code License:** [![License](https://img.shields.io/badge/license-MIT-blueviolet)](../main/CODE-LICENSE)

There are over 5,000 new lower limb amputations every year in the UK, and a major challenge is rehabilitating people with amputations by enabling them to return to normal activities, using a prosthetic limb. However, the residual limb is not initially suited for supporting the loads associated with standing or walking, and discomfort is common. The production of an appropriate patient-specific prosthetic socket is key, and today this is designed as a work of sculpture, by a highly experienced prosthetist. 

Many patient anatomy, surgery and disease factors can influence the socket design; however, few researchers have access to volumetric medical imaging data required to perform biomechanical analysis of socket designs. 

OpenLimbTT is a resource which contains a statistical description of transtibial amputated residual limbs based upon MRI scan data collected by the University of Southampton, UK, Flinders University, Australia, and Imperial College, UK in ethically-approved research projects, and at the New Mexico Decedent Individuals Database, USA, based on CT images. These descriptions include the external surface of the residual limb, the distal femur, patella, and residual tibia and fibula  (Figure 1, below). The Machine Learning method Principal Component Analysis (PCA) has been used to reduce the dimensionality of this anatomic dataset to generate a mean residual limb shape, and independent modes of shape variation. As such, the dataset describes the anatomic variation across the training dataset without including any identifiable representation of the individuals.

<p align="center">
  <img src="../main/abstract/Process.png" alt="Generating a transtibial residual limb Statistical Shape Model from medical imaging data (1), segmented, aligned and registered (2) to produce a mean shape (3) and principal modes of shape variability (4) shown in anterior and lateral views, with associated variance %" width="600"/>
</p>

In addition to characterising and measuring residual limb size and shape, this statistical shape analysis method allows synthetic data generation (Figure 2, below), whereby anatomically feasible residual limbs can be created with desired characteristics, for example to generate virtual test cases of particular interest or concern, to assist in prosthetics design or structural analysis.

<p align="center">
  <img src="../main/abstract/Modes1&2.png" alt="Creating example virtual individuals from the mean limb shape and its variation in the first two principal modes" width="250"/>
</p>

This dataset is intended to allow the research community to perform more statistically robust prosthetic biomechanics research, without the costs, inconvenience, and risk of putting our relatively small community of eligible research participants through medical imaging.

The latest OpenLimbTT Version-2025-04 is based upon 33 training datasets, 4 female and 29 male of a variety of ethnicities (12 White European/US, 9 Hispanic, 5 Native American, 1 African American, and 6 not recorded). The publications below comment upon its limited statistical generality, but it does provide a preliminary representation of UK and a proportion of the US populations. 

You can download the model's mean shape, and virtual patient shapes covering 95% of training dataset variation in residual limb length and soft tissue bulbous-conical profile, as .stl files. These are normalised to the fractional intact length of the tibia, so should be scaled up to the desired intact tibia length.

For more detailed descriptions of the dataset and statistical testing behind it, please refer to the publication linked below.

How to acknowledge
------------------

OpenLimbTT has been presented at the 2023 International Society for Prosthetics & Orthotics World Congress, and a preprint of a full journal paper is currently under peer review. Please cite as:

F.E. Sunderland, A.J. Sobey, J.L. Bramley, J.W. Steer, R. Al-Dirini, C.D. Metcalf, the OpenLimb Group, P.R. Worsley, A.S. Dickinson (2024), OpenLimbTT, a Transtibial Residual Limb Shape Model for Prosthetics Simulation and Design: creating a statistical anatomic model using sparse data. medRxiv 2024.11.27.24317622; doi: [https://doi.org/10.1101/2024.11.27.24317622](https://doi.org/10.1101/2024.11.27.24317622), and [https://github.com/abel-research/openlimbTT](https://github.com/abel-research/OpenLimbTT).

or:

F.E. Sunderland, J.L. Bramley, R.M.A. Al-Dirini, J.W. Steer, P.R. Worsley & A.S. Dickinson (2023), OpenLimb: an Open Source Transtibial Residual Limb Model for Simulation and Design. Prosthetics & Orthotics International 47, p165; doi: [https://doi.org/10.1097/pxr.0000000000000240](https://doi.org/10.1097/pxr.0000000000000240) and [https://github.com/abel-research/openlimbTT](https://github.com/abel-research/OpenLimbTT).

OpenLimb Group Membership
--------

At the time of writing, the OpenLimb Group includes:
- Dr Jennifer Bramley, Prof Alex Dickinson, Prof Cheryl Metcalf, Prof Adam Sobey, Dr Joshua Steer, Fiona Sunderland, and Prof Peter Worsley (University of Southampton, UK),
- Dr Rami Al-Dirini (Flinders University, Australia),
- Dr Reza Safari (University of Derby, UK),
- Dr Graci Finco (The University of North Texas, USA),
- Dr Ziyun Ding (University of Birmingham, UK),
- Prof Anthony Bull, Dr Diana Toderita and Dr David Henson (Imperial College London, UK), and
- Dr Arjan Buis (University of Strathclyde, UK).

Funding
--------

The research behind this dataset was funded by the following organisations:
- the Royal Academy of Engineering (RAEng), UK (grant no. RF/130 (A Dickinson))
- the European Union 'Eurostars' programme (grant no. 9396 (A Dickinson & J Steer))
- the Engineering & Physical Sciences Research Council (EPSRC), UK (grant nos. EP/S02249X/1 Centre for Doctoral Training in Prosthetics & Orthotics (F Sunderland), EP/N509747/1 (J Bramley), EP/M508147/1 (J Steer))
- the Alan Turing Institute, UK (grant no. EP/N510129/1 (A Dickinson, A Sobey))
- the US National Institute of Justice (grant no. 2016-DN-BX-0144 (The Free Access Decedent Database))
- the Royal British Legion (A Bull, Z Ding, D Toderita, D Henson)

Ethical Approvals
--------

This secondary data analysis work was granted ethical approval by the University of Southampton's Ethics and Research Governance Office (ERGO 65748.A2)

Original data collection work was granted ethical approval by the following committees:
- Fraunhofer IPA Biomechanics Laboratory (2016_BLM_0009)
- the University of Southampton's Ethics and Research Governance Office (ERGO 41864.A1, ERGO 29927)
- the Southern Adelaide Clinical Human Research Ethics Committee (HREC/18/SAC/225)
- the Imperial College Research Ethics Committee (Reference 16IC3562) and the NHS Research Ethics Committee (REC reference 16/LO/1715)

License
--------

This dataset uses a Creative Commons Attribution Share Alike 4.0 International license, which can be found [here](../main/LICENSE)
Share Alike means that if you remix, transform, or build upon the dataset, you must distribute your contributions under the same license.


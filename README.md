<img src="docs/images/readme.png" alt="MRI-Based Brain Age Estimation"/>

<div align="center">
   <a href="https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge" alt="Python"><img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge" alt="Python"></a>
   <a href="/docs/credits.txt"><img src="https://img.shields.io/badge/credits-link-green?style=for-the-badge&logo=adobeacrobatreader&logoWidth=20&logoColor=green&color=94DD15" alt="Credits"></a>
   <a href="https://colab.research.google.com/github/antonioscardace/MRI-BrainAge/blob/main/notebooks/tutorial.ipynb" target="_blank"><img src="https://img.shields.io/badge/Open%20in-Colab-red?style=for-the-badge" alt="Open in Colab"></a>
   <a href="https://github.com/antonioscardace/MRI-BrainAge/blob/master/LICENSE"><img src="https://img.shields.io/badge/License-GPLv3-blue?style=for-the-badge" alt="License"></a>
</div>
<br/>

This project was developed as part of the Fundamentals of Data Analysis course examination. Inspired by the groundbreaking paper titled "**[Accurate brain‐age models for routine clinical MRI examinations](https://www.sciencedirect.com/science/article/pii/S1053811922000015?via%3Dihub)**", the work focuses on creating a predictive model using volumetric features extracted via **SynthSeg (FreeSurfer)** from **3D T1w Brain MRIs**. It estimates brain age, detecting deviations between chronological and biological brain age, showing that **Alzheimer’s Disease (AD)** links to accelerated brain ageing.

## Linking Brain Age and Alzheimer’s Disease

A polynomial regression model was trained via Cross-Validation, achieving a **MAE of 4.42 years**, with age as the dependent variable and other features as predictors. Trained on CN data, it predicted brain age for CN patients, with a Brain PAD of **-0.7 years**, closely matching chronological age. For AD patients, however, it showed a Brain PAD of **+5.32 years**, indicating that AD’s association with accelerated brain ageing.

<p align="center">
   <img src="docs/images/ages.png" height="240px"/>
</p>

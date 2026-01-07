# ***VOC-DRIVEN PLANT PHENOTYPING: PATTERNS AND INSIGHTS VIA PCA E FEATURE ANALYSIS***

![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![Jupyter](https://img.shields.io/badge/tools-Jupyter-orange.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

## **ABSTRACT**
This study aims to analyze the **emissions of *VOCs*** (volatile organic compounds) from **tomato plants** of **different genetic** lines subjected to **distinct treatments**. 

The work specifically focused on analyzing **raw data** obtained from Proton Transfer Reaction-Time of Flight Mass Spectrometry (**PTR-ToF-MS**). The VOC data were stored in **HDF5** (.h5) format, containing **mass spectrometry** measurements that provide insights into the temporal dynamics of volatile emissions.

Each HDF5 file was related to a singular plant and the surveys occurred at **three different times**: September 2023 (**T1**), October 2023 (**T2**), and November 2023 (**T3**).

Using *Principal Component Analysis (**PCA**)* allowed us to **reduce the dimensionality** of the problem, and through ***Feature Importance*** we were able to shift the focus to **key variables** in describing the phenomena.

The process is aimed at observing the **responses** of different plants to **various treatments**, track **VOCs variations** and frame the phenomenon in the broader context of **plant-plant interaction**.

## **PROJECT WORKFLOW**
1. **Data Extraction**: Parsing complex **HDF5** structures to extract temporal mass spectra.
2. **Preprocessing**: Implementing **One-Hot Encoding** for categorical variables (Genotype, Priming, Stress) and **Standard Scaling** for numeric mass features.
3. **Statistical Analysis**: Dimensionality reduction via **PCA** to identify the variance explained by principal components.
4. **Feature Importance**: Calculating the **absolute contribution** of each mass to identify the most influential chemical markers.
5. **Visualization**: Generation of **Radar Charts** to define the **Spectral Footprint** of each experimental condition.

## **KEY INSIGHTS**
- Identification of specific mass markers (e.g., **Mass_2**, **Mass_80**) that show high variability under stress conditions.
- Evidence of **differential chemical responses** between **Wildtype** and **Mutant** genotypes.
- Observation of **preparatory responses** in **Primed** plants, suggesting a significant role in **plant-to-plant signaling** and stress resilience.

## **REQUIREMENTS**
To run the analysis, the following Python libraries are required:
- `pandas`
- `numpy`
- `scikit-learn`
- `h5py`
- `matplotlib`
- `seaborn`

## **DATA AVAILABILITY**
The raw VOC data used in this project is private and not included in this repository. It resides on a secure, personal Google Drive and is referenced in the analysis notebook using local paths.

## **LICENSE**
This project is licensed under the MIT License. You are free to use, modify, and distribute this software with proper attribution.

## **AUTHORS**
- Laraia Letizia
- Peluso Pietro
- Zippo Luigi Emanuele

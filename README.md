# Prediction of Thermoelectric Material Properties with Machine Learning

## Overview
This project focuses on predicting the properties of thermoelectric materials using machine learning techniques. Thermoelectric materials convert heat into electricity, and their performance is measured by the figure of merit (ZT), which depends on properties such as the Seebeck coefficient, electrical conductivity, thermal conductivity, and temperature.

Using a data-driven approach, this project aims to identify key material descriptors that influence thermoelectric performance and to develop predictive models that can accelerate the discovery and design of efficient thermoelectric materials.

## Background
Thermoelectric effects such as the Seebeck, Peltier, and Thomson effects have been studied since the 19th century and have applications in waste heat recovery, solar power generation, and refrigeration. Improving thermoelectric materials requires balancing multiple physical properties, making it challenging to discover new materials experimentally.

Machine learning offers a powerful tool to analyze large datasets of known compounds, extract meaningful correlations, and predict material properties, potentially speeding up materials discovery.

## Dataset
The dataset used in this project is compiled from publicly available sources such as the TE Design Lab database and the NIST Atomic Spectra database. It contains about 5000 compounds with experimentally and computationally measured properties including:

- Seebeck coefficient
- Electrical conductivity
- Thermal conductivity
- Temperature

Additionally, elemental descriptors such as ionization energies, atomic radii, lattice parameters, electronegativity, and valence electron counts were calculated as weighted averages for each compound.

## Methodology
- Data preprocessing including normalization and standardization
- Feature engineering to calculate weighted averages of elemental descriptors
- Correlation analysis (Pearson and Spearman) to identify important features
- Random Forest regression models trained to predict:
  - Thermal conductivity
  - Electrical conductivity
  - Seebeck coefficient
  - Thermoelectric figure of merit (ZT)

The data was split into 80% training and 20% testing sets to evaluate model performance.

## Results
- The Random Forest models showed varying accuracy for different target properties.
- The Seebeck coefficient prediction had the best accuracy with about 22% MAE relative to the target mean.
- The ZT prediction model achieved a reasonable accuracy with about 47% MAE.
- Thermal and electrical conductivity predictions showed higher errors, reflecting the complexity of these properties.

## Usage
To run the models and reproduce the analysis:

1. Install required Python libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`, etc.
2. Prepare the dataset files as described.
3. Run the preprocessing scripts to generate feature matrices.
4. Train and evaluate the Random Forest models with the provided scripts.

Detailed scripts and data preprocessing codes are available in the repository.

## References
The project builds on foundational research in thermoelectric materials and recent advances in machine learning for materials science. Key references are included in the final report.

---

*Author:* Armağan Dağıstan  
*Advisor:* Assist. Prof. Dr. Irmak Sargın  
*Course:* PHYS400  
*Year:* 2023-2

---

Feel free to explore the code and contribute to further improving thermoelectric material predictions!


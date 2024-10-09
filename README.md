# London Crime Rate

This repository contains an R project that analyses crime rates across London's boroughs by building regression models and exploring spatial patterns. The primary goal is to create a minimal adequate model that accounts for multicollinearity and spatial autocorrelation, improving our understanding of the factors that influence crime rates.

## Table of Contents

- Introduction
- Dataset
- Project Contents
- Conclusions
- Contributing

## Introduction

This project explores the relationships between crime rates and socio-economic, demographic, and spatial factors in London's boroughs. It employs various statistical techniques and tools to preprocess data, analyze correlations, and build predictive regression models. The project also includes spatial analysis to examine geographic crime rate patterns and ensure the models account for spatial autocorrelation.

## Dataset

The dataset includes:

**Crime Rate Data:** Information on crime rates per 1,000 people across London boroughs.

**Deprivation Data:** Socio-economic deprivation scores for each area.

**LSOA Shapefiles:** Geographic boundaries for detailed spatial analysis.

**Note:** Please refer to the documents attached to this repository for greater detail on the data variables and the data sources.

## Project Contents

The analysis is structured as follows:

1. **Data Loading and Preparation:** Importing required libraries, loading datasets and merging datasets for comprehensive analysis.
2. **Exploratory Data Analysis (EDA):** Visualising the crime rate distribution, performing transformations, and creating correlation matrices to identify significant variables.
3. **Initial Regression Model:** Building an initial linear regression model to explain crime rates based on socio-economic factors.
4. **Model Refinement:** Checking for multicollinearity using Variance Inflation Factor (VIF), and iterating the model by removing non-significant variables and outliers.
5. **Spatial Analysis:** Mapping crime rates across London, calculating spatial autocorrelation with Moran's I, and examining residual autocorrelation to enhance model accuracy.

## Conclusions

The final regression model explains 44.7% of the variance in crime rates across London boroughs. Key factors influencing crime include the Index of Multiple Deprivation (IMD) Score, Black ethnicity percentage, and Muslim percentage. The model also accounts for spatial patterns through the use of spatial weights matrices, Moran's I, and residual diagnostics.

While the model is fairly robust, issues like heteroskedasticity highlight areas for further improvement, such as the potential inclusion of additional variables or transformations to address variance inconsistencies.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or submit a pull request.

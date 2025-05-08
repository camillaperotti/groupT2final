# Boston Housing Price Predictor

This project presents a predictive model for estimating housing prices in Boston using linear regression techniques. The goal is to provide a simple, transparent, and interactive tool for users to explore how key factors influence housing costs and receive tailored price estimates.

## Project Overview

Boston home buyers face a range of challenges—such as varying crime rates, pollution, school quality, and taxation—that affect housing prices. This project builds a linear regression-based predictive model that allows users to input housing-related features and get an estimated market value.

## Features

- User-friendly **Streamlit app** for interactive predictions.
- Explores the impact of variables such as:
  - Number of rooms
  - Crime rate
  - Pollution levels
  - Pupil-teacher ratio
  - Distance to employment centers
  - Tax rate and industrial concentration
- Built-in **EDA tools**: distribution plots, correlation heatmaps, and boxplots.

## Modeling Approach

- **Elastic Net Regression** with cross-validation
- Three datasets used:
  - **df**: all features (14 total)
  - **df1**: features with |correlation| > 0.4
  - **df2**: features with |correlation| > 0.2
- Best model performance:
  - **R² = 0.714**
  - **RMSE = 4.14**

## Key Findings

- The model using **all features (df)** outperformed simplified versions.
- Linear regression provides a baseline but lacks flexibility—suggesting future work should explore more complex models like neural networks.

## Try the App

You can test the prediction tool live via Streamlit:

[Open App](https://groupt2final-nscty94o2wqgnpndr49uec.streamlit.app/)

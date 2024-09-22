# Predictive Maintenance Project

## Overview
This project focuses on predicting equipment failures using machine learning techniques. The goal is to analyze data, apply various algorithms, and utilize methods like SMOTE (Synthetic Minority Over-sampling Technique) to balance class distributions for improved prediction accuracy.

## Table of Contents
- [Project Description](#project-description)
- [Data](#data)
- [Methods](#methods)
- [Models](#models)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Description
Predictive maintenance aims to foresee equipment failures before they occur, enabling proactive maintenance actions that enhance equipment reliability and reduce downtime. This project implements multiple machine learning models to achieve accurate predictions.

## Data
The dataset includes various features related to equipment operation and conditions:
- `UDI`: Unique identifier for each observation
- `Product ID`: Unique identifier for each product
- `Type`: Equipment type (label-encoded)
- `Air temperature [K]`: Ambient air temperature
- `Process temperature [K]`: Equipment process temperature
- `Rotational speed [rpm]`: Rotational speed of the equipment
- `Torque [Nm]`: Torque applied
- `Tool wear [min]`: Wear time of the tool
- `Target`: Binary target variable indicating failure (1) or no failure (0)
- `Failure Type`: Type of failure (if any)

## Methods
1. **Data Preprocessing**: Data cleaning, handling missing values, and encoding categorical variables.
2. **SMOTE**: Applied to balance the target classes to improve model performance on minority classes.
3. **Feature Selection**: Dropped unnecessary columns such as identifiers.

## Models
Two models were implemented:
- **Logistic Regression**: A baseline model for binary classification.
- **Random Forest Classifier**: An ensemble model used for its robustness and ability to capture complex patterns.

## Results
- **Random Forest Model**: Achieved an accuracy of **96%**.
- **Logistic Regression Model**: Achieved an accuracy of **86%**.

The Random Forest model outperformed the Logistic Regression model, making it the preferred choice for predicting equipment failures.

## Installation
To run this project locally, you need to have Python installed along with the required libraries. You can install the necessary libraries using pip:

```bash
pip install pandas numpy scikit-learn plotly imbalanced-learn



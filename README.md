# Commercial-Building-EUI-Prediction

## Project Overview
This project focuses on predicting the energy efficiency of commercial buildings in Seattle using the **Seattle Building Energy Benchmarking** dataset. By leveraging machine learning models such as **Random Forest** and **Gradient Boosting**, the goal is to predict the **Energy Use Intensity (EUI)** and provide insights into the factors that most significantly affect energy consumption.

---

## Problem Statement
Buildings are among the largest consumers of energy in urban areas. Improving energy efficiency in commercial buildings is crucial to reducing overall energy consumption and emissions. This project aims to develop a machine learning model that can accurately predict the **Energy Use Intensity (EUI)** of commercial buildings based on various building characteristics.

### Key Questions:
1. Can we predict a building’s energy efficiency using attributes like size, age, and energy sources?
2. Which factors most influence energy consumption in commercial buildings?
3. How can we use these predictions to help building managers optimize energy use?

---

## Data Source
The dataset used is the **Seattle Building Energy Benchmarking** dataset, which contains detailed energy usage and building characteristics for various commercial buildings in Seattle.

### Data Description
Key features include:
- **BuildingAge**: Age of the building.
- **PropertyGFATotal**: Gross Floor Area.
- **ENERGYSTARScore**: Energy efficiency score.
- **Electricity (kBtu)**: Electricity consumption.
- **NaturalGas (kBtu)**: Natural gas consumption.
- **GHGEmissionsIntensity (kgCO2e/ft²)**: Greenhouse gas emissions per square foot.
- **SiteEUI (kBtu/sf)**: Target variable, representing the energy use intensity.

---

## Project Structure
The project is divided into two main notebooks:

### 1. Data Wrangling and Exploratory Data Analysis (EDA)
- Data loading and inspection.
- Handling missing values, outliers, and feature engineering.
- Correlation analysis and visualizations.

### 2. Preprocessing, Modeling, Evaluation, and Improvements
- Feature selection, transformation, and normalization.
- Model training: **Linear Regression**, **Random Forest**, **Gradient Boosting**.
- Hyperparameter tuning using **GridSearchCV** and **RandomizedSearchCV**.
- Evaluation using **RMSE**, **MAE**, and **R²** metrics.
- Feature importance analysis and actionable insights.

---

## Models Used
- **Linear Regression**: Basic benchmark model.
- **Random Forest**: Ensemble model to reduce variance.
- **Gradient Boosting**: Incremental model that minimizes errors.

### Model Evaluation Metrics
- **MAE**: Measures the average magnitude of errors.
- **RMSE**: Penalizes larger errors.
- **R² Score**: Variance explained by the model.

### Results
| Model               | RMSE  | MAE  |
|---------------------|-------|------|
| **Random Forest**    | 18.73 | 7.71 |
| **Gradient Boosting**| 17.10 | 7.95 |

Gradient Boosting outperformed Random Forest based on RMSE, with both models providing strong predictive capabilities.

---

## Feature Importance (Gradient Boosting)
Top contributing factors to energy efficiency include:
1. **Electricity (kBtu)**: Largest contributor to EUI.
2. **PropertyGFATotal**: Larger buildings consume more energy.
3. **NaturalGas (kBtu)**: Significant impact on energy use.
4. **GHGEmissionsIntensity (kgCO2e/ft²)**: Higher emissions often mean less efficient buildings.
5. **ENERGYSTARScore**: Higher scores indicate more efficient buildings.
6. **BuildingAge**: Older buildings tend to consume more energy.

---

## Recommendations
1. **Reduce Electricity Consumption**: Implement energy-efficient lighting, HVAC systems, and smart energy management systems.
2. **Target Natural Gas Usage**: Retrofit heating systems or switch to renewable sources.
3. **Improve Energy Efficiency in Older Buildings**: Use modern insulation, HVAC systems, and smart building technologies.
4. **Increase ENERGY STAR Scores**: Conduct energy audits and implement targeted improvements.
5. **Monitor GHG Emissions**: Focus on reducing emissions through energy-efficient upgrades and renewable energy adoption.

---

## Answering the Key Questions:
1. **Can we predict a building’s energy efficiency using attributes like size, age, and energy sources?**  
   Yes, both **Random Forest** and **Gradient Boosting** models provided strong predictions of energy efficiency based on these attributes.

2. **Which factors most influence energy consumption in commercial buildings?**  
   The most influential factors are **Electricity Consumption**, **PropertyGFATotal**, and **Natural Gas Consumption**.

3. **How can we use these predictions to help building managers optimize energy use?**  
   By providing actionable insights on high energy consumers and identifying areas for retrofitting and optimization, building managers can focus on the most impactful energy-saving strategies.

---

## Conclusion
This project successfully applied machine learning models to predict the energy efficiency of commercial buildings. The insights gained from feature importance analysis can guide building managers in optimizing energy consumption, reducing emissions, and improving overall sustainability.


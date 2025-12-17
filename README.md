Site URL: Github Pages : https://INFO523-Fall25-101-201.github.io/final-project-min-set-khant-solo/
Quarto Pub:  https://minsetkhant.quarto.pub/info-523--bmw-price-prediction
# BMW Car Price Analysis & Prediction
## Temporal Validation of Market Value

**Course:** INFO 523 - Data Mining and Discovery
**Author:** Min Set Khant
**Institution:** College of Information Science, University of Arizona

---

## Abstract

This project focuses on analyzing worldwide **BMW car sales data from 2010 to 2024** to understand the complex factors that determine a vehicle's market value. The core of the analysis involves building a robust machine learning model (Random Forest Regressor) and validating its performance using a **temporal train-test split**. This simulates a real-world scenario where the model predicts 2024 prices based on data up to 2023.

The final model achieves strong temporal stability, successfully predicting 2024 market prices with a **Mean Absolute Error (MAE) of approximately $531.13**. This provides high-confidence insights for pricing and inventory optimization strategies.

---

## Research Questions & Objectives

### Primary Objective
To build a machine learning model that accurately predicts used BMW car prices and evaluate the **temporal stability** of those predictions.

### Key Questions
1.  What are the key factors influencing BMW used-car prices in the market?
2.  How stable are the model's predictions over time?
3.  Using a temporal split, how well can the model predict pricing trends for the next year?

---

## Dataset

* **Source:** BMW Worldwide Sales Records (2010–2024).
* **Data:** Over 50,000 records of BMW sales and specifications across multiple regions.
* **Key Features:** Model, Year, Region, Engine\_Size\_L, Transmission, Fuel\_Type, and Price\_USD.

---

## Methodology & Results

### Modeling Approach
* **Model:** **Random Forest Regressor**.
* **Validation:** **Temporal Split** (Train: 2010–2023, Test: 2024).

### Key Results
| Metric | Value | Interpretation |
| :--- | :--- | :--- |
| **Mean Absolute Error (MAE)** | **\$531.13** | Average absolute prediction error on 2024 prices. |
| **R-squared (R²)** | **0.9952** (on Log Price) | High predictive power and variance explained. |

### Top Price Drivers
The model identified the most critical features impacting price:
1.  **Price per KM** (Engineered Feature)
2.  **Mileage (KM)**
3.  **Engine Size (L)**

---

## Deliverables

* **Quarto Website:** Full analysis, EDA, and methodology (HTML format).
* **Presentation:** 5-minute slide deck summarizing key insights (RevealJS format).
* **Model Artifact:** Trained model saved as `rf_best_model.joblib`.
* **Code Repository:** Fully reproducible code including analysis notebooks (`01_Data_Preparation_and_EDA.ipynb`, `02-modeling.ipynb`).

---

#### Disclosure:
Derived from the original data viz course by Mine Çetinkaya-Rundel @ Duke University

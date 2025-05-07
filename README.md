#  Telecom Churn Prediction ML Project

**Authors**: Rachana Amgai, Baldwin Dyce, Isis Lara  
**Date**: April 13, 2025

---

##  Project Overview

This project focuses on predicting customer churn in the telecommunications industry using a **multi-level classification approach**. By identifying whether a customer will churn, along with the **category** and **specific reason**, telecom companies can take targeted action to improve retention and reduce losses.

---

## Business Problem & Hypothesis

- **Problem**: Telecom churn rates range from **20–40% annually**, with mobile churn peaking at **31%**. Retaining a customer is **5–7 times cheaper** than acquiring a new one.

- **Hypothesis**: If churn risk and reasons can be predicted accurately, then personalized retention strategies can be applied early—saving revenue and improving customer satisfaction.

---

##  Methods and Analysis

We framed the problem as a **supervised machine learning** task:

### Modeling Strategy

- **Multi-Class Classification** → Churn Category  
- **Multi-Label Classification** → Churn Category + Reason

### Techniques Used

- Data Cleaning and Feature Aggregation
- Label Encoding for Categorical Variables
- Handling Imbalanced Data:  
  - **SMOTE** (Synthetic Minority Oversampling)  
  - **RandomUnderSampler**
- Models:
  - **Random Forest** for Churn Category
  - **Deep Neural Network** for Multi-Label Classification
- Metrics: Accuracy, F1-Score, and Categorical Accuracy

---

## Results

### Key EDA Insights

- 50% of churn occurred within **first 2 months** of service.
- Customers in low-population regions had slightly higher churn rates.
- Top churn reasons included:
  - Service dissatisfaction (6.2%)
  - Lack of self-service options (6.1%)

### Model Performance

| Model                      | Task                       | Accuracy   |
|---------------------------|----------------------------|------------|
| Random Forest Classifier  | Multi-Class Classification | **74.7%**  |
| Deep Neural Network       | Multi-Label Classification | **63.4%**  |

---

## Recommendations

- Improve onboarding and engagement within the first 2 months.
- Enhance self-service tools and digital support options.
- Continuously retrain models with updated data to adapt to customer behavior trends.

---

##  Ethical Considerations

- Balanced the dataset to prevent majority class bias.
- Monitored feature importances to avoid unfair targeting based on protected attributes.
- Focused on interpretable models to enable transparent business decisions.

---





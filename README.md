# Kaggle Titanic

## 1. Overview
This project aims to predict the survival of passengers on the Titanic using the classic Kaggle dataset. 

## 2. Approach & Feature Engineering
To improve the model's accuracy, I focused on the following techniques:

* **Title Extraction**: Extracted titles (Mr, Mrs, Miss, etc.) from names to better estimate age and social status.
* **Family Analysis**: Categorized FamilySize (SibSp + Parch + 1) into discrete bins (Alone, Small, Medium, Large) to capture non-linear relationships between family density and survival probability.
* **Ticket Grouping**: Identified passenger groups by shared ticket numbers.
* **Scaling**: Standardized numerical features like Ticket using StandardScaler.
* **Model**: **LightGBM** with 4-fold Stratified Cross-Validation.

## 3. Results
* **Kaggle Public Leaderboard Score:** **0.79425**
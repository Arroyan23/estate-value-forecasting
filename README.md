```markdown
# 🏡 Estate Value Forecasting

An advanced machine learning regression pipeline designed to predict residential property prices with high precision. This project leverages robust data preprocessing, feature engineering, and ensemble-based learning to model complex real estate pricing dynamics.

Developed as part of the Kaggle Housing Prices Competition.

---

## 🛠️ Tech Stack & Badges

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)

---

## 🚀 Key Features & Pipeline Architecture

This project implements a disciplined end-to-end Machine Learning pipeline optimized to prevent common pitfalls like data leakage and overfitting.

### 1. Data Preprocessing & Leakage Prevention
* **Golden-Rule Train-Test Split:** Strict isolation of validation sets prior to any stateful data transformations.
* **Categorical Encoding:** Seamless encoding of high-cardinality categorical columns using custom encodings mapping high-value features.
* **Robust Imputation:** Statistical imputation (median/most-frequent strategies) fitted *strictly* on training distribution and applied dynamically via `.transform()` to validation and test data to avoid data leakage.

### 2. Predictive Modeling
* **Algorithm:** Ensemble-based decision-making using a **Random Forest Regressor**.
* **Feature Alignment:** Automated dimension and column alignment ensuring the model's test prediction payload perfectly matches the training vector space.

---

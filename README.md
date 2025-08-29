## Dry Eye Disease Prediction

### Project Overview

This project aims to predict the **presence of Dry Eye Disease (DED)** based on a comprehensive dataset of lifestyle, health, and physiological factors. By analyzing features such as age, gender, sleep habits, stress levels, blood pressure, heart rate, and eye-related symptoms like redness and itchiness, the goal is to develop a machine learning model that can accurately classify DED risk. This can assist in early diagnosis and patient management.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Dry Eye Disease](https://www.kaggle.com/datasets/dakshnagra/dry-eye-disease)
  * **Size**: 20,000 entries, 26 columns
  * **Key Features**:
      * **Demographics & Lifestyle**: `Gender`, `Age`, `Sleep duration`, `Sleep quality`, `Stress level`, `Daily steps`, `Physical activity`, `Height`, `Weight`, `Smoking`, `Alcohol consumption`.
      * **Physiological & Symptoms**: `Blood pressure`, `Heart rate`, `Discomfort Eye-strain`, `Redness in eye`, `Itchiness/Irritation in eye`.
  * **Approach**:
      * **Data Cleaning**: The dataset was clean with no missing values or duplicates. The 'Blood pressure' column, which is a string, was handled implicitly by Label Encoding.
      * **Exploratory Data Analysis**: The code checks basic statistics, null values, duplicates, and unique values for all columns.
      * **Label Encoding**: Applied to all categorical features.
      * **Binary Classification**: The target variable `Dry Eye Disease` indicates the presence (`Y`) or absence (`N`) of the disease. The target class distribution is balanced.
      * **Models Used**:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * **70.1%** with Gradient Boosting Classifier.
      * **69.7%** with Random Forest Classifier.
      * **69.4%** with AdaBoost Classifier.
      * The moderate accuracies suggest that while the models have some predictive power, predicting DED from this set of features is a challenging task.

-----

### Purpose and Applications

  * Assist medical professionals in the **preliminary diagnosis and screening of Dry Eye Disease**.
  * Identify individuals at high risk for DED to recommend preventative measures and lifestyle changes.
  * Support public health initiatives by enabling a better understanding of DED risk factors.
  * Provide a tool for educational purposes in ophthalmology and medical data analysis.

-----

### Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Dry-Eye-Disease-Prediction-Using-ML.git
cd Dry-Eye-Disease-Prediction-Using-ML
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Performing comprehensive hyperparameter tuning and cross-validation for all models to ensure robustness.
  * Investigating the impact of different preprocessing techniques, especially for the 'Blood pressure' column, which is currently handled as a categorical feature.
  * Exploring more advanced feature engineering, such as creating a Body Mass Index (BMI) feature.
  * Adding explainability (e.g., SHAP or LIME) to understand which health and lifestyle factors are the most critical for DED prediction.

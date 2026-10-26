# FDS Assignment 1: Case Study 3
## Logistic Regression on the Titanic Dataset

### 1. Introduction

This project is part of the Fundamentals of Data Science course assignment. It focuses on applying Logistic Regression to the Titanic dataset to predict passenger survival based on selected passenger attributes.

The project involves data exploration, preprocessing, visualization, model development, performance evaluation, and interpretation of results using Python.

### 2. Objectives

- Perform exploratory data analysis on the Titanic dataset.
- Identify and handle missing values.
- Analyze the relationship between passenger characteristics and survival.
- Build a Logistic Regression classification model.
- Evaluate model performance using standard classification metrics.
- Interpret model coefficients and visualize the ROC curve.
- Implement an optional Streamlit application for predictions.

### 3. Dataset Description

The Titanic dataset contains 891 passenger records and 12 columns.

The target variable is `Survived`:
- `0`: Passenger did not survive.
- `1`: Passenger survived.

The features used for model development are:

| Feature | Description |
|---|---|
| Pclass | Passenger class |
| Sex | Passenger sex |
| Age | Passenger age |
| SibSp | Number of siblings or spouses aboard |
| Parch | Number of parents or children aboard |
| Fare | Ticket fare |
| Embarked | Port of embarkation |

### 4. Tools and Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Streamlit

### 5. Methodology

**Data Exploration:** Examined the dataset structure, data types, summary statistics, missing values, and survival distribution.

**Data Visualization:** Created visualizations to analyze survival patterns by sex and passenger class, age distributions, and correlations among selected numerical features.

**Data Preprocessing:** Handled missing values using median and most-frequent-value imputation. Applied one-hot encoding to categorical features and standardization to numerical features.

**Model Development:** Divided the dataset into training and testing sets and trained a Logistic Regression classifier using Scikit-learn.

**Model Evaluation:** Evaluated the model using accuracy, precision, recall, F1-score, and ROC-AUC. The analysis also includes a confusion matrix and ROC curve.

**Coefficient Interpretation:** Examined the model coefficients to understand how the selected features relate to predicted survival.

**Deployment:** Included an optional Streamlit application for interactive survival predictions.

### 6. Model Evaluation Results

The following results were obtained from the held-out test dataset:

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 0.8045 |
| Precision | 0.7931 |
| Recall | 0.6667 |
| F1-score | 0.7244 |
| ROC-AUC | 0.8437 |

The model achieved an accuracy of approximately 80.45%. The ROC-AUC score of 0.8437 indicates that the model has a useful ability to distinguish between survivors and non-survivors. Precision and recall provide additional information about the types of predictions made by the classifier.

### 7. Repository Structure

The repository may contain the following files:

- `Case_Study_3_Titanic_Logistic_Regression.ipynb` – Jupyter Notebook containing the code, outputs, visualizations, and analysis.
- `titanic.csv` – Dataset used for the analysis.
- `app.py` – Streamlit application for interactive predictions, if included.
- `requirements.txt` – Required Python packages, if included.
- `README.md` – Project documentation.

### 8. Execution Instructions

The notebook can be executed using Google Colab.

1. Open the Jupyter Notebook in Google Colab.
2. Upload the Titanic dataset when prompted.
3. Execute the notebook cells sequentially.
4. Review the visualizations, statistical findings, and evaluation metrics.

To run the optional Streamlit application locally, install the required dependencies and execute:

```bash
pip install -r requirements.txt
streamlit run app.py
```

The application also requires any saved model files referenced by `app.py`.

### 9. Conclusion

This case study demonstrates the application of Logistic Regression to a binary classification problem. The analysis includes data preprocessing, exploratory visualization, model training, performance evaluation, and coefficient interpretation. The results illustrate how machine learning can be used to study passenger survival patterns while highlighting the importance of evaluating classification models using multiple metrics.

### 10. Student Details

- **Name:** V. Sai Eshwar
- **Roll Number:** 160124733205
- **Section:** CSE-3
- **Year:** Third Year
- **Subject:** Fundamentals of Data Science
- **Assignment:** FDS Assignment 1
- **Case Study:** 3 – Logistic Regression

### References

- Supplied Titanic dataset.
- Scikit-learn documentation: https://scikit-learn.org/stable/
- Pandas documentation: https://pandas.pydata.org/docs/
- Matplotlib documentation: https://matplotlib.org/stable/
- Seaborn documentation: https://seaborn.pydata.org/
- Streamlit documentation: https://docs.streamlit.io/

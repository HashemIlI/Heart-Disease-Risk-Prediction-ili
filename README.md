# 🫀 Heart Disease Risk Prediction

[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/hashemili/heart-disease-risk-prediction-ili?scriptVersionId=225705641)
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-green?logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📋 Overview

This project builds and evaluates multiple **Machine Learning classification models** to predict the risk of heart disease based on medical and lifestyle features. The analysis was performed on Kaggle using the **Heart Disease Risk Prediction Dataset (EarlyMed)**.

The goal is to compare the performance of various classifiers and identify the most effective algorithm for early heart disease risk detection.

---

## 📁 Repository Structure

```
Heart-Disease-Risk-Prediction-ili/
│
├── heart-disease-risk-prediction-ili.ipynb   # Main Jupyter Notebook (Kaggle)
└── README.md                                  # Project documentation
```

---

## 📊 Dataset

- **Source:** [Heart Disease Risk Prediction Dataset – EarlyMed (Kaggle)](https://www.kaggle.com/datasets/heart-disease-risk-prediction-dataset)
- **File:** `heart_disease_risk_dataset_earlymed.csv`
- **Target Variable:** `Heart_Risk` (Binary: 0 = No Risk, 1 = At Risk)
- **Note:** The dataset was found to be clean and ready for analysis with no missing values. The `Gender` feature was dropped after correlation analysis showed it had the least impact on the target variable.

---

## 🔬 Methodology

### 1. Data Exploration
- Loaded and inspected the dataset using `df.head()`, `df.info()`, and `df.describe()`
- Converted all columns to integer type for consistency

### 2. Data Analysis
- Generated a **correlation heatmap** to visualize feature relationships with the target
- Dropped the `Gender` column due to its low correlation with `Heart_Risk`

### 3. Model Building
Split the data (80% train / 20% test) and trained 4 classification models:

| # | Model | Library |
|---|-------|---------|
| 1 | Logistic Regression | `sklearn.linear_model` |
| 2 | Support Vector Classifier (SVC) | `sklearn.svm` |
| 3 | Random Forest Classifier | `sklearn.ensemble` |
| 4 | Gradient Boosting Classifier | `sklearn.ensemble` |

### 4. Model Evaluation
Each model was evaluated using:
- **Accuracy**
- **Recall**
- **F1-Score**
- **Confusion Matrix**

Results were compiled into a final comparison DataFrame and visualized using a line plot.

---

## 🧰 Technologies & Libraries

```python
pandas          # Data manipulation
numpy           # Numerical computation
matplotlib      # Data visualization
seaborn         # Statistical data visualization
scikit-learn    # Machine learning models & metrics
```

---

## 📈 Results

The final results are compared across all four models using **Accuracy**, **Recall**, and **F1-Score**. A comparative line plot is generated to visually highlight the best-performing classifier.

> For full results and outputs, open the notebook on Kaggle using the badge at the top.

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/HashemIlI/Heart-Disease-Risk-Prediction-ili.git
   cd Heart-Disease-Risk-Prediction-ili
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. **Run the notebook:**
   Open `heart-disease-risk-prediction-ili.ipynb` in Jupyter Notebook or JupyterLab.
   
   > **Note:** The dataset path references `/kaggle/input/`. To run locally, download the dataset from Kaggle and update the path accordingly.

4. **Or open directly on Kaggle:**
   Click the **Open in Kaggle** badge at the top of this README.

---

## 👤 Author

**Ahmed Fouad Hashem (HashemIlI)**  
[![Kaggle](https://img.shields.io/badge/Kaggle-Profile-blue?logo=kaggle)](https://www.kaggle.com/hashemili)
[![GitHub](https://img.shields.io/badge/GitHub-HashemIlI-black?logo=github)](https://github.com/HashemIlI)


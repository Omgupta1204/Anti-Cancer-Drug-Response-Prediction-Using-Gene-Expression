# 🧬 Anti-Cancer Drug Response Prediction Using Gene Expression

A machine-learning project for predicting anti-cancer drug responses using gene-expression data from the **Genomics of Drug Sensitivity in Cancer (GDSC)** database. The project uses **Pearson Correlation-based feature selection** and **ElasticNet Regression** to identify important genes and predict drug sensitivity.

---

## 📌 Project Overview

Cancer patients can respond differently to the same anti-cancer drug due to variations in their genetic and molecular profiles. Predicting drug response using gene-expression data can support **precision oncology** and help identify potential biomarkers associated with drug sensitivity.

This project develops a machine-learning framework that analyzes gene-expression profiles and predicts anti-cancer drug responses using **IC50 and AUC** measurements.

---

## 🎯 Objectives

* Predict anti-cancer drug responses using gene-expression data.
* Identify genes associated with drug sensitivity.
* Reduce the dimensionality of high-dimensional gene-expression data.
* Develop an interpretable machine-learning prediction model.
* Evaluate prediction performance using statistical metrics.
* Identify biologically relevant cancer-related pathways.

---

## 📊 Dataset

The project uses data from the **Genomics of Drug Sensitivity in Cancer (GDSC)** database.

### Dataset Includes

* Cancer cell-line gene-expression data
* Anti-cancer drug response measurements
* **IC50 (Half-Maximal Inhibitory Concentration)**
* **AUC (Area Under the Curve)**

IC50 and AUC are used as indicators of drug sensitivity.

---

## 🔄 Project Workflow

```text
GDSC Dataset
     ↓
Data Preprocessing
     ↓
Data Normalization
     ↓
Pearson Correlation Analysis
     ↓
Feature Selection
     ↓
ElasticNet Regression
     ↓
K-Fold Cross-Validation
     ↓
Model Evaluation
     ↓
Drug Response Prediction
     ↓
Biological Interpretation
```

---

## ⚙️ Methodology

### 1. Data Collection

Gene-expression and drug-response data are collected from the GDSC database.

### 2. Data Preprocessing

The dataset is prepared for machine learning through:

* Missing-value handling
* Data normalization
* Duplicate removal
* Irrelevant feature removal
* Data integration and preparation

### 3. Feature Selection

**Pearson Correlation Coefficient (PCC)** is used to measure the relationship between gene-expression values and drug-response measurements.

Genes showing stronger correlations with drug response are selected as predictive features.

### 4. Model Development

The project uses **ElasticNet Regression**, which combines:

* **L1 regularization (Lasso)** — assists in feature selection.
* **L2 regularization (Ridge)** — improves model stability and reduces overfitting.

This makes ElasticNet suitable for high-dimensional gene-expression data.

### 5. Model Validation

**K-Fold Cross-Validation** is used to evaluate the model's performance and generalization capability across different subsets of the dataset.

---

## 📈 Performance Evaluation

The model is evaluated using:

| Metric  | Full Form                       | Purpose                                                             |
| ------- | ------------------------------- | ------------------------------------------------------------------- |
| **PCC** | Pearson Correlation Coefficient | Measures correlation between predicted and actual responses         |
| **MSE** | Mean Squared Error              | Measures prediction error                                           |
| **R²**  | Coefficient of Determination    | Measures how well the model explains the variation in drug response |

The project achieved **PCC values above 0.6 for several drugs**, with stronger correlations observed for some targeted therapies.

---

## 🧪 Biological Interpretation

The selected predictor genes were further analyzed to understand their biological relevance.

The project identified associations with important cancer-related pathways, including:

* **MAPK signaling**
* **p53 regulation**
* **Cell-cycle control**

These pathways are relevant to cancer development, drug sensitivity, and treatment response.

---

## 🛠️ Technologies Used

### Programming

* Python

### Machine Learning

* Scikit-learn
* ElasticNet Regression

### Data Analysis

* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn

### Data Source

* Genomics of Drug Sensitivity in Cancer (GDSC)

---

## 📁 Project Structure

```text
Anti-Cancer-Drug-Response-Prediction/
│
├── data/
│   └── GDSC dataset
│
├── notebooks/
│   └── Drug_Response_Prediction.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── feature_selection.py
│   ├── model.py
│   └── evaluation.py
│
├── results/
│   ├── model_results
│   └── visualizations
│
├── README.md
└── requirements.txt
```

> Update the folder/file names above according to the actual files in your GitHub repository.

---

## 🔬 Key Results

* Gene-expression data demonstrated useful predictive information for anti-cancer drug response.
* Pearson Correlation helped identify relevant predictor genes.
* ElasticNet provided a balance between prediction and feature selection.
* Several drugs achieved **PCC > 0.6**.
* Selected genes showed associations with important cancer-related pathways.
* The approach demonstrates the potential of machine learning for **precision oncology**.

---

## 🚀 Future Scope

The project can be extended by integrating additional biological information such as:

* Gene mutation profiles
* DNA methylation data
* Proteomic information
* Multi-omics datasets

More advanced models can also be explored, including:

* Graph Neural Networks (GNNs)
* Autoencoders
* Transformer-based models
* Deep-learning architectures

Future work can also focus on validating the model using real patient datasets and developing a web-based clinical decision-support system.

---

## 📚 Research Publication

This project was developed as part of a research study on **machine-learning-based anti-cancer drug response prediction using gene-expression data**.

The research methodology includes GDSC data processing, Pearson Correlation-based feature selection, ElasticNet Regression, model evaluation, and biological interpretation.

---


> **Gene-expression profiles can provide valuable information for predicting anti-cancer drug responses, while machine-learning techniques such as Pearson Correlation and ElasticNet can help identify predictive genes and support precision oncology.**

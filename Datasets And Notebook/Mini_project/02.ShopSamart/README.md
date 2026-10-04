# 🛒 ShopSmart – Online Purchase Prediction

## 📌 Project Overview

**ShopSmart** is a machine learning classification project designed to predict whether an online visitor is likely to complete a purchase based on their browsing and interaction behaviour.

The dataset contains **12,330 unique user sessions** collected over a one-year period. Each session represents a unique visitor, helping reduce bias caused by repeated users, promotional campaigns, seasonal trends, or special events.

The project focuses on building a **Decision Tree Classifier** and improving its performance using **pruning techniques**. Since the target variable is imbalanced, the **F1-score** is used as the primary evaluation metric.

---

## 🎯 Problem Statement

An e-commerce company wants to understand visitor behaviour and identify sessions that are likely to result in a purchase.

The objective is to develop a machine learning model that can:

- Analyse visitor browsing behaviour
- Perform exploratory data analysis (EDA)
- Preprocess numerical and categorical features
- Handle categorical variables appropriately
- Build a Decision Tree classification model
- Apply pruning to reduce overfitting
- Evaluate the model using the **F1-score**
- Compare model performance against a benchmark F1-score of **0.55**

---

## 📊 Dataset

The dataset contains **12,330 user sessions** with numerical and categorical features.

### Features

| Feature | Description |
|---|---|
| Administrative | Number of administrative pages visited |
| Administrative_Duration | Time spent on administrative pages |
| Informational | Number of informational pages visited |
| Informational_Duration | Time spent on informational pages |
| ProductRelated | Number of product-related pages visited |
| ProductRelated_Duration | Time spent on product-related pages |
| BounceRates | Percentage of visitors leaving after one page |
| ExitRates | Percentage of page exits |
| PageValues | Average value of pages visited before a transaction |
| SpecialDay | Closeness to a special day |
| Month | Month of the visit |
| OperatingSystems | Operating system used |
| Browser | Browser used |
| Region | Geographic region |
| TrafficType | Source of website traffic |
| VisitorType | Type of visitor |
| Weekend | Whether the visit occurred on a weekend |
| Revenue | Whether the visitor completed a purchase |

### Target Variable

**Revenue**

- `True` → Purchase completed
- `False` → No purchase

---

## 🔍 Project Workflow

The project follows an end-to-end machine learning workflow:

### 1. Exploratory Data Analysis

- Inspect dataset dimensions and data types
- Check missing values
- Analyze numerical features
- Analyze categorical features
- Identify class imbalance
- Study relationships between features and `Revenue`
- Visualize important patterns

### 2. Data Preprocessing

- Handle missing values if present
- Separate features and target variable
- Encode categorical variables
- Prepare numerical features
- Split data into training and testing sets

### 3. Model Development

A **Decision Tree Classifier** is trained to predict whether a visitor will make a purchase.

The initial model is evaluated to identify possible overfitting and performance issues.

### 4. Decision Tree Pruning

Pruning is applied to control the complexity of the Decision Tree and reduce overfitting.

Parameters such as:

- `max_depth`
- `min_samples_split`
- `min_samples_leaf`
- `ccp_alpha`

can be investigated to determine their effect on model performance.

### 5. Model Evaluation

Because the dataset is imbalanced, **F1-score** is used as the primary evaluation metric.

Additional metrics can include:

- Precision
- Recall
- Accuracy
- Confusion Matrix

### 6. Benchmark

The target benchmark for the project is:

**F1-score ≥ 0.55**

The performance of the pruned Decision Tree is compared against this benchmark.

---

## 🧠 Machine Learning Algorithm

### Decision Tree Classifier

A Decision Tree is a supervised machine learning algorithm that makes predictions by recursively splitting the dataset based on feature values.

In this project, the tree learns patterns in visitor behaviour and predicts:

```text
Visitor Session
       ↓
Browsing Behaviour
       ↓
Decision Tree
       ↓
Purchase Prediction
       ↓
Revenue: True / False
```

Pruning is used to prevent the tree from becoming unnecessarily complex and overfitting the training data.

---

## 📈 Evaluation Metric

### F1-Score

The F1-score is particularly useful for this problem because the dataset contains an imbalanced target variable.

It combines **precision** and **recall**:

\[
F1 = 2 \times \frac{Precision \times Recall}{Precision + Recall}
\]

The project uses an F1-score of **0.55** as the benchmark for evaluating the effectiveness of the solution.

---

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

 

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project

```bash
cd ShopSmart-Online-Purchase-Prediction
```

### 3. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook inside the `Notebook` folder and run the cells sequentially.

---

## 📌 Expected Outcome

The final model should identify patterns in visitor behaviour that are associated with online purchases.

The project specifically aims to determine whether **pruning the Decision Tree improves generalization and F1-score**, while targeting the benchmark F1-score of **0.55**.

---

## 🔮 Future Improvements

Possible future extensions include:

- Hyperparameter tuning
- Random Forest classification
- Gradient Boosting
- XGBoost
- Cross-validation
- Feature importance analysis
- SHAP-based model interpretation
- Deployment using Flask or FastAPI
- Building a web interface for real-time purchase prediction

---

## 👩‍💻 Project Type

**Machine Learning – Classification | Minor Project**

**Focus:** E-commerce Purchase Prediction using Decision Tree Classification and Pruning
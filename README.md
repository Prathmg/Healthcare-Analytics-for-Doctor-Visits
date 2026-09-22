# 🏥 Healthcare Analytics for Doctor Visits

A data analytics and machine learning project that analyzes healthcare data to understand patterns associated with **doctor visits**. The project combines exploratory data analysis, statistical analysis using **Poisson Regression**, and **Random Forest classification** to identify important factors related to healthcare utilization.

---

## 📌 Project Overview

Healthcare utilization can be influenced by several factors such as illness, health conditions, age, income, insurance coverage, and chronic conditions.

This project analyzes a healthcare dataset containing **5,190 records and 13 variables** to explore these relationships and demonstrate how data analytics and machine learning can be applied to healthcare-related problems.

The main target variable is:

- `visits` — Number of doctor visits

For the machine learning task, this variable is converted into a binary target:

- `0` → No doctor visit
- `1` → At least one doctor visit

---

## 🎯 Objectives

- Understand the healthcare dataset and its variables.
- Clean and prepare the data for analysis.
- Explore the distribution of doctor visits.
- Analyze the relationship between illness and doctor visits.
- Examine doctor visits across different insurance categories.
- Study relationships between numerical healthcare variables.
- Apply **Poisson Regression** for doctor-visit count analysis.
- Build a **Random Forest Classification** model.
- Evaluate classification performance.
- Identify important factors using feature importance.

---

## 🗂️ Dataset

The dataset contains healthcare-related information including:

| Variable | Description |
|---|---|
| `visits` | Number of doctor visits |
| `gender` | Gender of the individual |
| `age` | Age |
| `income` | Income-related variable |
| `illness` | Number of illnesses |
| `reduced` | Number of days activity was reduced due to illness |
| `health` | General health condition |
| `private` | Private insurance indicator |
| `freepoor` | Free/poor insurance indicator |
| `freerepat` | Free/repat insurance indicator |
| `nchronic` | Number of non-chronic conditions |
| `lchronic` | Number of chronic conditions |

---

## 🛠️ Technologies Used

- **Python**
- **Pandas** — Data manipulation
- **NumPy** — Numerical computation
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Statsmodels** — Statistical modeling
- **Scikit-learn** — Machine learning
- **Google Colab** — Development environment

---

## 🔄 Project Workflow

```text
Healthcare Dataset
       ↓
Data Loading
       ↓
Data Understanding
       ↓
Data Cleaning
       ↓
Exploratory Data Analysis
       ↓
Correlation Analysis
       ↓
Poisson Regression
       ↓
Feature Preparation
       ↓
Random Forest Classification
       ↓
Model Evaluation
       ↓
Feature Importance
       ↓
Key Findings
```

---

## 📊 Exploratory Data Analysis

The project includes several visual analyses:

### 1. Doctor Visits Distribution

Examines how doctor visits are distributed across the dataset.

### 2. Doctor Visits vs. Illness

A box plot is used to investigate how the number of doctor visits varies with the number of reported illnesses.

### 3. Insurance Analysis

Average doctor visits are compared across different insurance-related categories.

### 4. Correlation Analysis

A correlation heatmap is generated to examine relationships between numerical healthcare variables.

---

## 📈 Statistical Analysis — Poisson Regression

Since `visits` represents a **count of doctor visits**, Poisson Regression is used to examine the relationship between the visit count and selected healthcare and demographic variables.

The model considers variables such as:

- Age
- Income
- Illness
- Reduced activity
- Health
- Gender
- Insurance indicators

The statistical output is used to examine the estimated relationships between these variables and doctor visit counts.

> **Note:** Statistical association should not be interpreted as proof of causation.

---

## 🤖 Machine Learning — Random Forest

A **Random Forest Classifier** is used to predict whether an individual has visited a doctor.

### Target Variable

```text
has_visited

0 → No doctor visit
1 → At least one doctor visit
```

### Model Configuration

```python
RandomForestClassifier(
    n_estimators=100,
    random_state=42
)
```

The dataset is divided into:

- **80% Training Data**
- **20% Testing Data**

Stratified splitting is used to maintain the target-class distribution.

---

## 📏 Model Evaluation

The Random Forest model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The project also visualizes the confusion matrix to compare actual and predicted classifications.

---

## 🔍 Feature Importance

Random Forest feature importance is used to identify which input variables contribute most to the model's classification decisions.

This helps provide an interpretable view of which variables are most influential within the trained model.

---

## 📌 Key Results

The final numerical results are generated directly from the notebook after execution.

The project reports:

- Doctor visit distribution
- Illness vs. doctor visit patterns
- Insurance-related visit patterns
- Correlation relationships
- Poisson Regression results
- Random Forest accuracy and classification metrics
- Confusion matrix
- Feature importance

> Results are dataset-specific and should be interpreted within the limitations of the available data.

---

## 📁 Project Structure

```text
Healthcare-Analytics-for-Doctor-Visits/
│
├── Healthcare_Analytics_for_Doctor_Visits.ipynb
├── Healthcare Analytics for Doctor Visits (1).csv
└── README.md
```

---

## ▶️ How to Run the Project

### 1. Open Google Colab

Upload or open:

```text
Healthcare_Analytics_for_Doctor_Visits.ipynb
```

### 2. Upload the Dataset

Upload:

```text
Healthcare Analytics for Doctor Visits (1).csv
```

### 3. Run the Notebook

Execute the notebook cells from top to bottom.

The notebook will perform:

```text
Data Loading
→ Data Cleaning
→ EDA
→ Correlation Analysis
→ Poisson Regression
→ Random Forest
→ Model Evaluation
→ Feature Importance
```

---

## 📸 Project Outputs

The main visual outputs include:

- 📊 Doctor Visits Distribution
- 📦 Doctor Visits vs. Illness
- 🔥 Correlation Heatmap
- 🤖 Random Forest Confusion Matrix
- 📈 Feature Importance

These visualizations provide both statistical and machine-learning perspectives on the dataset.

---

## ⚠️ Limitations

- The analysis is based on a single healthcare dataset.
- The dataset may not represent the entire population.
- Machine learning performance depends on the available features and data quality.
- Feature importance indicates model contribution, not medical causation.
- The project is intended for **educational and analytical purposes**, not for clinical diagnosis or medical decision-making.

---

## 🚀 Future Scope

- Use larger and more recent healthcare datasets.
- Include additional demographic and healthcare variables.
- Compare Random Forest with other classification algorithms.
- Perform feature engineering and hyperparameter tuning.
- Develop an interactive healthcare analytics dashboard.
- Explore advanced statistical and machine learning techniques.
- Extend the analysis to broader healthcare utilization patterns.

---

## 🎓 Project Purpose

This project demonstrates the practical application of **Python, data analytics, statistical modeling, data visualization, and machine learning** to a healthcare dataset.

It is intended as an academic/portfolio project demonstrating an end-to-end data analysis workflow.

---

## 👨‍💻 Author

**Prathmesh**

Electrical Engineering | Data Analytics | Machine Learning

---

## 📜 License

This project is intended for educational and portfolio purposes.

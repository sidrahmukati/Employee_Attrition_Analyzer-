# Employee Attrition Analyzer

An end-to-end Machine Learning pipeline using the **IBM HR Analytics Employee Attrition & Performance** dataset. This project aims to predict whether an employee is likely to leave a company based on demographic, compensation, and work experience attributes.

---

## 🛠️ Features

- **Data Preprocessing**: Drops redundant columns, maps target categories to binary format (`Yes` $\rightarrow 1$, `No` $\rightarrow 0$), standardizes numerical features, and applies One-Hot Encoding to categorical attributes.
- **Model Training & Comparison**: Fits and evaluates three classification models:
  - **Logistic Regression**
  - **Decision Tree**
  - **Random Forest**
- **Evaluation Metrics**: Compares models using **F1 Score** and **Confusion Matrices** with class weight balancing (`class_weight='balanced'`).
- **Feature Importance**: Visualizes the top 10 key drivers of employee attrition using the Random Forest model's Gini feature importances.

---

## 📁 Project Structure

```text
.
├── README.md                           # Project documentation
├── requirements.txt                     # Project dependencies
├── WA_Fn-UseC_-HR-Employee-Attrition.csv # Dataset file
└── attrition_analyzer.py                # Main analysis and modeling script
```

---

## 🚀 Getting Started

### 1. Requirements & Prerequisites
Ensure you have Python 3.8+ installed.

### 2. Installation
Install all required dependencies using `pip`:

```bash
pip install -r requirements.txt
```

### 3. Usage

#### Running in Google Colab:
1. Upload `WA_Fn-UseC_-HR-Employee-Attrition.csv` to your Google Colab root folder.
2. Run the main script cells in sequence.

#### Running Locally:
Run the script using Python:

```bash
python attrition_analyzer.py
```

---

## 📊 Evaluation Outputs

The script outputs:
1. **Model Performance Summary**: A table showing the F1 Score for all three models.
2. **Confusion Matrices**: Heatmaps comparing true vs. predicted outcomes for each model.
3. **Feature Importance Bar Chart**: A horizontal bar chart depicting the top 10 features influencing employee departure.
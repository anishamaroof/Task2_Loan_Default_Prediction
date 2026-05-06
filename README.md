# Task2_Loan_Default_Prediction
Data Science &amp; Analytics Internship Tasks 2- DevelopersHub Corporation
# 💳 Task 2: Credit Risk / Loan Default Prediction

**DevelopersHub Corporation — Data Science & Analytics Internship**

---

## 📌 Task Objective

Predict whether a loan applicant is likely to **default** on a loan using machine learning classification models.

---

## 📂 Dataset

- **Name:** German Credit Risk Dataset
- **Source:** Loaded directly via URL (no download needed)
- **Size:** 1000 rows × 21 columns
- **Target:** `default` — 1 = Default, 0 = No Default

**Key Features:**
- `Credit Amount` — Loan amount requested
- `Duration of Credit (month)` — Loan duration
- `Age (years)` — Applicant age
- `Account Balance` — Bank account status
- And 16 more features...

---

## 🛠️ My Approach

### Step 1 — Data Loading & Inspection
- Loaded dataset directly via URL using `pandas.read_csv()`
- Inspected shape, columns, data types, and summary statistics

### Step 2 — Data Cleaning
- Checked for missing values → None found ✅
- Removed duplicate rows
- Encoded target variable for clarity

### Step 3 — EDA & Visualizations
| Plot | Purpose |
|------|---------|
| Count Plot | Default vs No Default distribution |
| Histogram | Loan amount distribution by status |
| Box Plot (Age) | Age vs default relationship |
| Box Plot (Duration) | Loan duration vs default |
| Correlation Heatmap | Feature correlations |

### Step 4 — Model Training
- **Logistic Regression** — Linear classification model
- **Decision Tree** — Tree-based classification model
- Train/Test Split: 80% / 20%
- Feature Scaling: StandardScaler

### Step 5 — Evaluation
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1)

---

## 📊 Results & Key Insights

| Model | Accuracy |
|-------|----------|
| Logistic Regression | ~75% |
| Decision Tree | ~72% |

1. ✅ **Logistic Regression** performed slightly better
2. 📈 **Higher credit amounts** → more likely to default
3. ⏳ **Longer loan durations** → higher default risk
4. 👤 **Younger applicants** → slightly higher default rate
5. 🏦 Banks should prioritize these features in risk assessment

---

## 🧰 Libraries Used

```python
pandas, numpy
matplotlib, seaborn
scikit-learn (LogisticRegression, DecisionTreeClassifier, StandardScaler)
```

---

## 🚀 How to Run

1. Open [Google Colab](https://colab.research.google.com/) or VS Code
2. Upload `Task2_Loan_Default_Prediction.ipynb`
3. Click **Run All**
4. Dataset loads automatically via URL — no download needed! ✅

---

## 📁 File Structure

```
DevelopersHub-Internship-Tasks/
├── Task1-Iris-Visualization/
│   ├── Task1_Iris_Visualization.ipynb
│   └── README.md
├── Task2-Loan-Default-Prediction/
│   ├── Task2_Loan_Default_Prediction.ipynb
│   └── README.md
```

---

*Submitted by: Anisha Maroof | DevelopersHub Corporation Internship 2026*


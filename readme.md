# Student Course Completion Prediction Model

## 📌 Project Overview
This project focuses on predicting whether a student will successfully complete an online course based on their engagement, performance, and behavioral data. The goal is to identify key factors that influence course completion and build a robust classification model that can help detect at-risk students early.

The dataset contains detailed student activity logs, academic performance indicators, and course-related attributes, making it suitable for real-world educational analytics use cases.

---

## 🎯 Problem Statement
Online learning platforms often face high dropout rates. By analyzing student behavior and performance patterns, this project aims to:
- Predict course completion outcomes
- Understand factors contributing to student success or dropout
- Support early intervention strategies

---

## 🧠 Approach & Workflow

1. **Data Cleaning**
   - Removed identifier and leakage columns
   - Handled missing values and data type inconsistencies

2. **Exploratory Data Analysis (EDA)**
   - Analyzed completion rate distribution
   - Studied engagement, progress, and performance patterns
   - Used professional visualizations such as violin plots, ECDFs, and normalized bar charts

3. **Feature Engineering**
   - Extracted date-based features from enrollment data
   - Created behavioral buckets (inactivity, course length, payment level)
   - Designed composite features like `Engagement_Score` and `Performance_Score`

4. **Preprocessing**
   - Encoded categorical features
   - Scaled numerical features
   - Reduced feature dimensionality to avoid noise

5. **Handling Class Imbalance**
   - Evaluated class distribution
   - Applied balancing techniques where necessary

6. **Model Building**
   - Logistic Regression (baseline)
   - Random Forest
   - XGBoost (final model)

7. **Evaluation**
   - Precision, Recall, F1-score
   - Confusion Matrix
   - ROC-AUC Score

---

## 📊 Key Insights
- Student engagement metrics (progress percentage, login frequency, time spent) strongly influence course completion.
- Engineered features like `Engagement_Score` significantly improved class separation.
- Academic performance indicators (quiz scores, project grades) are strong predictors of completion.
- Behavioral inactivity is an early signal of dropout risk.

---

## 🛠️ Tech Stack
- **Language:** Python  
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn  
- **ML:** Scikit-learn, XGBoost, Imbalanced-learn  
- **Environment:** Jupyter Notebook, Virtual Environment  

---

## 🚀 How to Run the Project

```
python -m venv venv
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run training script
python src/train_model.py
```

---

### 📌 Future Improvements
- Deploy model as a web application

- Add early-warning system for dropout detection

- Perform SHAP-based feature importance analysis

---

## 👤 Author

**Shivam Singh**
Aspiring Data Scientist | Machine Learning Enthusiast

🔗 GitHub: [https://github.com/shivamsingh-itds]
🔗 LinkedIn: [www.linkedin.com/in/shivamsinghds]

---

⭐ If you find this project helpful, feel free to star the repository!gi
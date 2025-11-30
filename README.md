# AI-project-sentiment-analyzer-


# 📘 Employee Sentiment & Engagement Analysis  
**Author:** Kirthika R S
**Internship Project Submission**

---

## 📌 Project Overview  
This project analyzes employee email messages to understand sentiment, engagement, communication behavior, and potential flight risks.  
Using NLP and data science techniques, the project performs:

- Sentiment Labeling  
- Exploratory Data Analysis (EDA)  
- Monthly Sentiment Scoring  
- Employee Ranking  
- Flight Risk Identification  
- Predictive Modeling (Linear Regression)

All tasks are implemented end-to-end inside **main.ipynb**.

---

## 🧠 Technologies Used
- Python  
- Pandas / NumPy  
- Matplotlib / Seaborn  
- NLTK (VADER)  
- TextBlob (validation only)  
- WordCloud  
- Scikit-learn (Linear Regression)  
- Jupyter Notebook  

---

# ✅ **Project Tasks Summary**

## **Task 1: Sentiment Labeling**
- Cleaned email text (subject + body)
- Applied **VADER** to label sentiment (Positive / Neutral / Negative)
- Validated using TextBlob (Agreement ≈ 63%)
- Final model chosen: **VADER**
- Output: `labeled_with_vader.csv`

---

## **Task 2: EDA (Exploratory Data Analysis)**
Key insights:
- Distribution of sentiment categories  
- Monthly communication trends  
- Employee-level activity patterns  
- Word count distribution  
- Positive/Negative WordClouds  

All charts saved in the `visualizations/` folder.

---

## **Task 3: Monthly Sentiment Scoring**
Using scoring rules:
- Positive = +1  
- Neutral = 0  
- Negative = –1  

Produced sentiment score per employee per month.  
Output: `employee_monthly_sentiment_scores.csv`

---

## **Task 4: Employee Ranking**
Based on monthly scores:
- **Top 3 Positive employees**  
- **Top 3 Negative employees**  
Sorted by score → then alphabetical order  
Outputs:
- `top3_positive_employees.csv`
- `top3_negative_employees.csv`

---

## **Task 5: Flight Risk Identification**
Rule:  
An employee is a **flight risk** if they send **≥ 4 negative emails** within any **rolling 30-day window**.

Output: `flight_risk_employees.csv`

---

## **Task 6: Predictive Modeling**
Built a **Linear Regression model** to predict monthly sentiment scores.

### Features Used:
- Monthly message count  
- Avg message length  
- Word count  
- Positive/Negative/Neutral message counts  

### Evaluation Metrics:
- **R² Score:** (ADD YOUR VALUE HERE)  
- **MAE:** (ADD YOUR VALUE)  
- **RMSE:** (ADD YOUR VALUE)  

Model saved as:
- `linear_regression_sentiment_model.joblib`
- `scaler.joblib`

---



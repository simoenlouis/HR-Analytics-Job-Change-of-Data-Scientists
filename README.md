# HR-Analytics-Job-Change-of-Data-Scientists
Kaggle Link: (https://www.kaggle.com/datasets/arashnic/hr-analytics-job-change-of-data-scientists)

##📌 Project Overview
This project aims to predict whether a data science candidate will look for a new job after completing company training. The goal is to help companies optimize training costs and focus on candidates who are more likely to stay.

##🛠️ Tools & Technologies
- Python
- Pandas & NumPy
- Scikit-learn
- XGBoost
- Matplotlib / Seaborn

##🎯 Business Problem

Companies invest heavily in training candidates, but not all trainees intend to stay.
Being able to predict who is likely to leave helps in:
- Reducing training costs
- Improving retention strategies
- Better candidate targeting

##📂 Dataset Description

The dataset contains:

- Demographics (gender, city, etc.)
- Education level
- Work experience
- Company-related features

- Target variable:

- target = 1 → Candidate is looking for a job change
- target = 0 → Candidate will stay

##⚙️ Data Preprocessing
- Handling missing values
- Encoding categorical variables (One-Hot Encoding)
- Feature scaling (StandardScaler)
- Train-test split

##🤖 Models Used

I trained and compared multiple machine learning models:

- Logistic Regression (LG)
- Random Forest
- XGBoost (XG)

##📊 Model Evaluation

-🔹 XGBoost
- Accuracy: 0.7829
- Precision: 0.5477
- Recall: 0.7237
- F1 Score: 0.6235
-🔹 Logistic Regression
- Accuracy: 0.7717
- Precision: 0.5283
- Recall: 0.7542
- F1 Score: 0.6214

##🧠 Key Insight
- Although XGBoost achieved slightly higher F1 Score, Logistic Regression was selected as the best model because:
It achieved higher Recall (0.7542)
Difference in F1 Score is very small (~0.02)
Higher recall means better detection of candidates likely to leave
- In this business case, Recall is more important because missing a candidate who intends to leave is more costly than incorrectly predicting someone will leave.

##✅ Final Model Choice

✔️ Logistic Regression

Because it:

- Maximizes detection of potential leavers
- Provides simpler and more interpretable results
- Performs competitively with more complex models

##📈 Conclusion

This project demonstrates that:

Simpler models like Logistic Regression can outperform complex models depending on the business objective
Choosing the right metric (Recall vs F1 vs Accuracy) is critical
Model selection should always align with business goals, not just raw performance

## Author
- Simoen Louis

- GitHub: simoenlouis

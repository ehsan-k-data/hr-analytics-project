# HR Analytics Project – Employee Satisfaction

## 📌 Business Problem
ServiceFirst is facing high employee turnover and rising recruitment costs.  
This project analyses employee data to identify key drivers of satisfaction and predict retention risk.

## 🧰 Tools Used
Python (Pandas, NumPy), Scikit-learn, Matplotlib, Seaborn, NLP (TextBlob, NLTK)

## 🔍 What I Did
- Performed Exploratory Data Analysis (EDA)
- Built regression models to predict satisfaction
- Applied K-Means clustering to segment employees
- Developed a Decision Tree classifier
- Conducted sentiment analysis on employee reviews

## 📊 Key Results
- Autonomy, training, and work pressure are strongest drivers of satisfaction  
- Salary is NOT a strong predictor (confirmed across models)  
- Identified high-risk employee segments using clustering  
- Achieved ~97% accuracy with pruned Decision Tree model  

## 💡 Business Impact
- Helps HR identify employees at risk of leaving  
- Supports better decision-making on retention strategies  
- Highlights key areas to improve workplace satisfaction  

---







# Service-First-Employee-Satisfaction-
Employee Satisfaction Analytics — Machine Learning & NLP Case Study
A Two-Part Analytical Project Using CRISP-DM, Regression Models, Clustering, Decision Trees & NLP

This repository contains two different analytical projects, both focused on understanding and predicting employee satisfaction using statistical techniques and machine learning.

Although both projects use the same overall business problem, they analyse different datasets and use different modelling approaches.

-- PROJECT SET 1 — Regression Models (Linear & Multiple Regression)

“Designing Machine Learning Model Framework for ServiceFirst Employee Satisfaction — Linear & Multi-Linear Regression”

-- Overview — Project Set 1

This project uses supervised learning and classical statistics to identify the key drivers of employee satisfaction and to build predictive regression models.

This section focuses on:

Exploratory Data Analysis (EDA)

Correlation Analysis

Hypothesis Testing (t-tests & Chi-Square)

Simple Linear Regression

Multiple Linear Regression with VIF

Model evaluation using MAE, MSE, and RMSE

- Business Context

ServiceFirst is a national equipment servicing company facing:

High turnover

Increased recruitment cost

Loss of experienced staff

Reduced productivity

Goal: Use analytics to identify key satisfaction drivers and predict future risk.

(See pages 1–4 of report) →

- Dataset Summary (Project 1)

The dataset includes:

10 Standardised Satisfaction Factors

Overall Satisfaction Score

Intention to Quit

Sentiment codes

Work Location / Length / Managerial Role
(See pages 2–12) →

- Modelling Methods (Project 1)
- Simple Linear Regression

X = Autonomy

Y = Overall Satisfaction Score

R² ≈ 0.25–0.32 → Weak model

Interpretation: Autonomy explains ~25% of variability
(See pages 20–22) →

- Multiple Linear Regression

Predictors: Autonomy, Training, Welfare, Direct Manager, Work Pressure…

R² = 0.99 → Very high accuracy

VIF used to remove multicollinearity

MAE, MSE, RMSE extremely low
(See pages 23–28) →

- Hypothesis Testing Results

All 4 hypothesis tests show no significant difference:

Remote vs Office

Managers vs Non-managers

Intention to Quit vs Satisfaction

Work Location vs Quit Intention
(See pages 19–20) →

- Key Insights from Project 1

Top predictors of satisfaction:
✔ Autonomy
✔ Training
✔ Integration
✔ Work Pressure (negative)

Salary, work location & managerial role = not strong predictors

Multiple Regression is highly predictive (R² = 0.99)

-----------------------------------------------------------

-- PROJECT SET B — Clustering, Decision Tree & Sentiment Analysis


“Designing Machine Learning Model Framework — Clustering, Decision Trees & Sentiment Analysis”

-- Overview — Project Set B

This part of the repository expands the analysis into:

Unsupervised Learning (K-Means Clustering)

Classification (Decision Tree)

Natural Language Processing (Sentiment Analysis)

Word frequency analysis, word clouds & polarity scoring

This dataset is different from Project A and contains:
✔ Employee demographics
✔ Income
✔ Total working years
✔ Review text
✔ Satisfaction score
(See pages 6–11) →

- MODELLING METHODS (PROJECT B)
- K-Means Clustering

Performed using:

Income

Satisfaction Score

Visualisation & cluster selection using:

Elbow Method → K = 3

Silhouette Score → K = 4

Final K = 4 clusters, validated visually
(See pages 18–20) →

Cluster Interpretation (Page 32)

Cluster 0: High income + high satisfaction (loyal)

Cluster 1: Medium satisfaction + low income

Cluster 2: Low income + low satisfaction (turnover risk)

Cluster 3: High income + low satisfaction (critical segment)

- Decision Tree Classifier

Predicts:

Satisfied (1) vs Dissatisfied (0)

Techniques used:

Train/test split 80/20

Pruning (max_depth=3, balanced classes)
(See pages 21–24) →

Results

Unpruned Accuracy: 100% (overfitting)

Pruned Accuracy: 97%

Top Predictors:
✔ Business Travel
✔ Age
✔ Working Years

- Sentiment Analysis (NLP)

Using NLTK, WordCloud, FreqDist, TextBlob

Processing steps:

Text cleaning

Tokenisation

Stopword removal

Polarity scoring

Frequency distribution

WordCloud
(See pages 23–30) →

Findings

Most common words:

work

good

pay

Positive sentiment:

Good pay

Great experience

Friendly environment

Negative sentiment:

Management issues

Workload

Outdated equipment

Low recognition

Work-life imbalance

-Key Insights from Project B

Salary DOES NOT strongly predict satisfaction (reinforces Project A findings)

High travel frequency = strong dissatisfaction indicator

Younger employees are more satisfied

Some high-income employees show low satisfaction → high value risk group

NLP reveals internal friction around management, pay & workload

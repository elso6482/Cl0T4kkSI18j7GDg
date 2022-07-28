# Term-deposit

This project aims to predict the subscription on term deposit and finds out what key factors lead to the subscription. At the end of the projest. We can determine the segment of customer the marketing team should focus on.

The term deposit data has 13 attributes: 

age, balance, last contact day of the month, last contact duration, number of contacts performed during campagin (numeric)

job, marital, education, contact communication type, last contact month of year (categorical)

credit default history, housing loan, personal loan (binary)

# Feature selection

Categoral features are selected based on Chi-square. Credit default history is dropped due to statistical insignificane.

![image](https://user-images.githubusercontent.com/62399559/180721223-0c62316d-7ed0-42e0-a448-0e54864f9c46.png)

Ordinal features are all selected. 

After dropping unrelated features, 10 remaining features are used to find out the best prediction model.

# Model selection

Pycaret is used to build multiple models. For term deposit marketing purpose, we focus on capturing potential customers who are willing to subscribe. Therefore, we would like to examine both models with higher precision rate and models with higher recall rate. 

# SHAP analysis

To understand how features contribute to the prediction. SHAP package is used to explain the output of machine learning models.

![image](https://user-images.githubusercontent.com/62399559/181434645-d969f4b5-2a24-42a5-9f63-875a1364afb8.png)

![image](https://user-images.githubusercontent.com/62399559/181434700-eb6ff7c2-32db-45fc-a349-2ace289e18e2.png)

![image](https://user-images.githubusercontent.com/62399559/181434728-7687cbc9-5f5b-49a5-8e8b-dc36897b5407.png)

![image](https://user-images.githubusercontent.com/62399559/181434763-d53b2b1c-8033-45d6-b6b3-c14d29c7ae20.png)

![image](https://user-images.githubusercontent.com/62399559/181434795-0b75f759-b810-4566-b10d-ea60a8dab0ce.png)


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

![image](https://user-images.githubusercontent.com/62399559/180723867-f1ff5f21-6414-4310-95db-d90585f478ba.png)



![image](https://user-images.githubusercontent.com/62399559/180721361-8a5630a6-5670-47bd-b382-db30d4d1dd87.png)


![image](https://user-images.githubusercontent.com/62399559/180720986-6d240cfe-34b5-427b-91a2-a2c7c98803bd.png)

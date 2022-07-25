# Term-deposit

This project aims to predict the subscription on term deposit and finds out what key factors lead to the subscription. At the end of the projest. We can determine the segment of customer the marketing team should focus on.

The term deposit data has 13 attributes: 

age, balance, last contact day of the month, duration, number of contacts performed during campagin (numeric)

job, marital, education, contact communication type, last contact month of year (categorical)

credit default history, housing loan, personal loan (binary)



Categoral features are selected based on Chi-square

![image](https://user-images.githubusercontent.com/62399559/180721223-0c62316d-7ed0-42e0-a448-0e54864f9c46.png)

After dropping unrelated features, 10 remaining features are used to find out the best prediction model.


Model	Accuracy	AUC	Recall	Prec.	F1	Kappa	MCC	TT (Sec)
catboost	CatBoost Classifier	0.9380	0.9471	0.4150	0.6111	0.4938	0.4621	0.4721	12.0470
lightgbm	Light Gradient Boosting Machine	0.9371	0.9466	0.4145	0.6015	0.4900	0.4578	0.4672	2.3740
gbc	Gradient Boosting Classifier	0.9364	0.9404	0.3470	0.6151	0.4429	0.4120	0.4314	2.6380
xgboost	Extreme Gradient Boosting	0.9349	0.9421	0.4120	0.5757	0.4800	0.4463	0.4535	4.8430
rf	Random Forest Classifier	0.9339	0.9359	0.3060	0.5923	0.4025	0.3714	0.3946	1.4770
lr	Logistic Regression	0.9330	0.9213	0.2532	0.6005	0.3549	0.3257	0.3604	5.0420
lda	Linear Discriminant Analysis	0.9329	0.9255	0.4306	0.5532	0.4835	0.4483	0.4527	0.2160
ada	Ada Boost Classifier	0.9310	0.9279	0.3275	0.5469	0.4087	0.3745	0.3889	0.7610
ridge	Ridge Classifier	0.9305	0.0000	0.1476	0.6006	0.2363	0.2137	0.2734	0.0780
et	Extra Trees Classifier	0.9300	0.9170	0.2292	0.5494	0.3227	0.2925	0.3242	1.4800
dummy	Dummy Classifier	0.9269	0.5000	0.0000	0.0000	0.0000	0.0000	0.0000	0.0540
knn	K Neighbors Classifier	0.9244	0.7632	0.2454	0.4664	0.3209	0.2850	0.3019	0.4910
dt	Decision Tree Classifier	0.9148	0.7008	0.4502	0.4224	0.4353	0.3893	0.3898	0.1670
svm	SVM - Linear Kernel	0.9073	0.0000	0.2068	0.3816	0.2467	0.2027	0.2230	0.2320
nb	Naive Bayes	0.8963	0.8448	0.4780	0.3503	0.4035	0.3484	0.3539	0.0710
qda	Quadratic Discriminant Analysis	0.5187	0.5196	0.5206	0.0802	0.1367	0.0136	0.0212	0.1660


![image](https://user-images.githubusercontent.com/62399559/180721361-8a5630a6-5670-47bd-b382-db30d4d1dd87.png)


![image](https://user-images.githubusercontent.com/62399559/180720986-6d240cfe-34b5-427b-91a2-a2c7c98803bd.png)

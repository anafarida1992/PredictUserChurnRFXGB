**Project Waze aims to prevent or at least reduce churn, hence improving retention and driving business growth by analyzing a dataset with 14,999 rows and 13 columns:**\
A. Predicting customer churn using logistic regression, random forest and xgboost.\
B. Identifying key predictors of customer churn using correlation heatmap and feature importance from logistic regression and xgboost.\
C. Comparing iphone and android as users' device types using A/B test.\
\
**A. Predicting customer churn using logistic regression, random forest and xgboost.**\
•	The XGB model fits the data better than the random forest model. Its recall score (0.13) is higher than the logistic regression (0.05) and random forest model's (0.12), while keeping similar accuracy (0.18) and precision (0.45).\
•	The XGB model's recall and precision slightly declined, indicating a performance discrepancy between the validation and test scores.\
•	The XGB model predicted four times as many false negatives (439) than it did false positives (82).\
\
**B. Identifying key predictors of customer churn using correlation heatmap and feature importance from logistic regression and xgboost.**\
•	In the exploratory data analysis, km_per_driving_day had the strongest positive correlation with user churn while activity_days and driving_days had the most negative.\
•	Feature importance may vary across different models. Never abandon a feature without full insight into its relationship with the target variable. Different results can be caused by complex interactions between features.\
•	Whereas XGBoost incorporated more features in its use, logistic regression did rely highly on the activity_days feature in most of the predictions.\
•	In the logistic regression model, activity_days was the most important feature, and it had a negative correlation with user churn. A new feature called professional_driver ranked third regarding predictive power.\
\
**C. Comparing iphone and android as users' device types using A/B test.**\
•	Descriptive statistics compare average number of drivers for each device type, showing that drivers who use an iPhone device to interact with the application have a higher number of drives on average. However, this difference could be due to random chance.\
•	To confirm the difference, a two-sample t-hypothesis test (independent t-test) with significance level 5% performed as part of the A/B test.\
•	It concludes that there is not a statistically significant difference in the average number of drives between drivers who use iPhones and drivers who use Androids.

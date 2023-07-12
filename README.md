# Employee-turnover-analysis_and_prediction
In this repository, I analysed the employee turnover dataset using pandas and tried various supervised ML models, using scikit-learn, to predict the occurrence of a turnover. Finally, I compared the accuracy obtained from each model and trained the model which provided the highest accuracy. 

In the repository [Employee-turnover-analysis-using-SQL](https://github.com/AREEBAKAMIL/Employee-turnover-analyis-using-SQL/tree/main), I had analysed the employee turnover dataset, at a high-level, using SQL. However, the analysis using SQL did not provide sufficient information to determine the relationship between the occurrence of the turnover('event') and the remaining variables.

In this repository, I used pandas and scikit-learn to analyze and predict the occurrence of a turnover. The results showed that the ExtraTreesClassifier performed the best, albeit, the accuracy score is still quite low.

# About the dataset
The Employee Turnover dataset is a real dataset taken from [Edward Babushkin's blog](https://edwvb.blogspot.com/2017/10/employee-turnover-how-to-predict-individual-risks-of-quitting.html). The dataset contains data about Employee's risk of quitting based on various factors. <br />

Columns: <br />
"stag" - experience <br />
"event" - event      
"gender"       
"age"          
"industry"     
"profession"  
"traffic" - From what pipelene candidate came to the company <br />
"coach" - presence of a coach on probation <br />
"head_gender" - Gender of the head
"greywage" -  The salary does not seem to the tax authorities <br />
"way" -   how an employee gets to workplace (by feet, by bus etc) <br />
"extraversion" - One of Big5 test scales <br />
"independ" - One of Big5 test scales <br />
"selfcontrol" - One of Big5 test scales <br />
"anxiety" - One of Big5 test scales <br />
"novator" - One of Big5 test scales <br />

# Steps:
1. Download the csv file.
2. Load the csv into pandas dataframe
3. Check for missing/null values
4. Encode categorical columns using Label-Encoding
5. Check for correlation using a heatmap
6. split the dataset into test and train
7. Train supervised ML models and compare results
8. Perform another training of the model which had provided the highest accuracy (in this case - ExtraTreesClassifier)

# Conclusion
The results obtained using the ExtraTreesClassifier are as follows:

              precision    recall  f1-score   support

           0       0.68      0.65      0.67       112
           1       0.67      0.70      0.69       114
           
Considering the above, we can see that the accuracy is not that high. This is not surprising as the correlation map does not show a strong relation between turnover (i.e. 'event') and the other variables in the data.

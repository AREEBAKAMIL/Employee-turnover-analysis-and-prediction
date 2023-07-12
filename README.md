# Employee-turnover-analysis_and_prediction
In this repository, I analysed the employee turnover dataset using pandas and tried various supervised ML models to predict the occurrence of a turnover. Finally, I compared the accuracy obtained from each model and trained the model which provided the highest accuracy. 

In the repository Employee-turnover-analysis-using-SQL, i had analysed the employee turnover dataset, at a high-level, using SQL. However, the analysis using SQL did not provide sufficient information to determine the relationship between the occurrence of the turnover('event') and the remaining variables.

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
2. Import the file to MySQL (you can use an SQL GUI such as [MySQL Workbench](https://www.mysql.com/products/workbench/))
3. Check distinct values to look for any null values
4. Perform anaysis using SQL
5. Visualize it using using Google Looker Studio


# Netflix 
The purpose of this project is to demonstrate data cleaning and visualization skills using a Netflix dataset. The dataset includes content from 2008 to 2021, with content dating back as far as 1925.
Data Preparation and Cleaning
1.
Importing Libraries: Python libraries like pandas, numpy, and seaborn were imported to handle data manipulation and visualization.
2.
Handling Null Values: No null values were found in the dataset, simplifying the cleaning process.
3.
Duplicate Removal: Three duplicate movie titles were identified and removed.
4.
Splitting Duration: The 'duration' column was split into two: 'Duration1' for movie length in minutes and 'Seasons1' for TV show seasons.
5.
Breaking Listed Genres: The 'listed_in' column was split into multiple genre columns to enhance visualization and analysis of Netflix content by genre.
Exploratory Data Analysis (EDA)
•
Movies vs TV Shows: Netflix has a larger collection of movies compared to TV shows, reflecting its strong focus on film content.
•
Directors: A significant portion of content lacks director information. Rajiv Chilaka has the most content on Netflix, and over 3,600 directors have contributed only one piece of content each.
Country-wise Insights:
•
Top Countries: The United States has the most content on Netflix (3,240 titles), followed by India (1,084 titles).
•
Single-Content Countries: Some countries, like Paraguay and Somalia, have only one piece of content available.
Date Insights:
•
Content Growth: The majority of Netflix's content was added between 2016 and 2021, with notable spikes in 2018, 2019, and 2020, especially during the COVID-19 pandemic.
•
Monthly Trends: Content additions tend to increase toward the end of the year, particularly in October through December.
Yearly and Monthly Content Insights:
•
Content Release: Most content was released between 2016 and 2020, with a slight dip in 2021, possibly due to the pandemic.
•
Ratings Focus: TV-MA and TV-14 ratings are the most common, showing a focus on adult audiences. There’s a rise in family-friendly content like TV-Y and TV-G rating.
Duration and Seasons Insights:
•
Movie Duration: Most Netflix movies are between 90 and 105 minutes long.
•
TV Shows: Many titles labelled as TV shows actually have zero seasons, indicating they might be stand-alone specials or miniseries.
Country-Specific Analysis
•
United States: Dramas, comedies, and documentaries dominate Netflix's US catalog, with consistent additions across months.
•
India: Consistent movie additions, with more focus on international films and dramas.
•
Brazil, UK, Germany: All show an upward trend in TV show additions, particularly after 2018.
•
Pakistan, Japan, Nigeria: Each country’s focus shifts between movies and TV shows, with notable increases in content additions post-2016.

Conclusion :-
1.
Content Growth: Netflix's content catalog has grown significantly, especially between 2016 and 2020, with a focus on adding more movies than TV shows.
2.
Country-specific Insights: The United States and India are the largest contributors to Netflix’s library, with the U.S. dominating in terms of sheer volume. Other countries like the UK, Brazil, and Japan have also shown a steady increase in content.
3.
Genres and Ratings: Netflix caters to a wide audience, but there's a clear focus on adult-oriented content (TV-MA, TV-14), while family-friendly content has seen a slight increase since 2020.

# Iris Model
Building a Machine Learning Model using the Iris Dataset
1. Introduction
The Iris dataset is a popular dataset used for classification tasks. It contains 150 observations of iris flowers, with 50 samples each from three species: Iris setosa, Iris versicolor, and Iris virginica. Each observation consists of four features: sepal length, sepal width, petal length, and petal width. The goal of this project is to build and evaluate multiple machine learning models to classify the species of an iris flower based on these features.
2. Dataset Overview
•
Features:
o
Sepal Length (cm)
o
Sepal Width (cm)
o
Petal Length (cm)
o
Petal Width (cm)
•
Target: Species (Iris setosa, Iris versicolor, Iris virginica)
3. Data Cleaning and Preprocessing
3.1 Null Value Check
Upon examining the dataset, it was found that:
•
No null values were present in any of the features or target columns.
3.2 Duplicate Value Check
•
3 duplicate records were identified and subsequently removed to ensure the dataset contained unique observations.
3.3 Outlier Detection and Removal
•
Outliers were checked using statistical methods. For each feature, outliers were detected based on the interquartile range (IQR).
•
Outlier Removal:
o
Upper limit = Q3 + 1.5 * IQR
o
Lower limit = Q1 - 1.5 * IQR
o
Outliers that exceeded these thresholds were removed to improve the quality of the data.
3.4 Label Encoding
•
The target column, species, was a categorical variable and needed to be encoded. Label Encoding was applied, where the three species were converted into numerical labels:
o
Iris setosa → 0
o
Iris versicolor → 1
o
Iris virginica → 2
4. Model Building
To find the best model for classifying iris species, we explored six different machine learning algorithms:
1.
Logistic Regression
2.
K-Nearest Neighbors (KNN)
3.
Support Vector Classifier (SVC)
4.
Gaussian Naive Bayes (GaussianNB)
5.
Decision Tree Classifier
6.
Random Forest Classifier
4.1 Cross-Validation
Each model was evaluated using cross-validation to ensure the model’s generalization capability. We used K-Fold Cross-Validation with k=5 to split the data into 5 parts, where each fold was used once as the test set while the remaining 4 were used for training.
4.2 Hyperparameter Tuning
To further improve model performance, GridSearchCV was employed for hyperparameter tuning. This method helps in finding the optimal combination of hyperparameters for each model.
5. Model Comparison and Results
The performance of each model was evaluated based on the accuracy score. The following table summarizes the results:
Model
Accuracy
Cross-Validation
Best Hyperparameters
Logistic Regression
100
97
{'C': 10, 'penalty': 'l2', 'solver': 'saga'}
K-Nearest Neighbors (KNN)
96
97
{'algorithm': 'auto', 'n_neighbors': 5, 'weights': 'distance'}
Support Vector Classifier
97
96
{'C': 0.1, 'gamma': 1, 'kernel': 'poly'}
GaussianNB
97
96
{'var_smoothing': 1e-09}
Decision Tree Classifier
86
93
{'criterion': 'gini', 'max_depth': 4, 'min_samples_leaf': 3, 'min_samples_split': 3, 'splitter': 'random'}
Random Forest Classifier
100
94
{'criterion': 'gini', 'n_estimators': 500, 'n_jobs': -1, 'oob_score': True}
6. Conclusion
•
Best Performing Model: Based on cross-validation accuracy, the best model for this dataset was found to be Logistic Regression, which outperformed others in terms of accuracy and generalization capability.
•
Hyperparameter Tuning Impact: Hyperparameter tuning significantly improved the model performance, especially for complex models like Random Forest.
7. Future Work
Future improvements could include:
•
Testing on different datasets or using other classification algorithms (e.g., Neural Networks).
•
Deeper hyperparameter optimization using RandomizedSearchCV for faster results.
4.
Duration Trends: Most movies on Netflix are about 90-105 minutes long. For TV shows, a significant number of titles listed actually have zero seasons, likely representing one-off specials or miniseries.
5.
Global Reach: Netflix's strategy includes adding content from diverse countries and genres, which helps it cater to a global audience.

# IBM HR ANALYTICS EMPLOYEE ATTITION & PERFORMANCE

1
IBM HR Analytics Employee Attrition
&
Performance
Name:- Maurya Mayank
ID:- UM2024829
Gmail:- mmayank3585@gmail.com
Date:- DD/MM/YYYY
2
Abstract:
Employee attrition, or turnover, presents a substantial challenge to organizations, impacting productivity, financial stability, and team cohesion. This project seeks to address this issue by analyzing employee data to identify key factors influencing turnover and develop predictive models for early identification of high-risk employees.
Utilizing a fictional dataset, the analysis examines attrition rates across demographic and job-related categories, such as age, gender, education, job role, and department. By understanding the most significant contributors to turnover, including job satisfaction, work-life balance, and salary, this project aims to provide actionable insights for HR teams.
Leveraging machine learning techniques, predictive models are developed to forecast employee attrition. These models offer organizations the opportunity to implement proactive retention strategies, thereby reducing turnover rates and improving employee satisfaction.
3
Table of Contents
S.No.
Sub.S.No.
Topics
Page no.
4
INTRODUCTION
Employee Attrition: A Critical Challenge and a Data-Driven Solution
Employee attrition, or turnover, poses a significant threat to organizational success. High turnover rates can lead to increased recruitment and training costs, disrupted team dynamics, and a loss of valuable institutional knowledge. Understanding the underlying factors that contribute to attrition is essential for HR departments to implement effective retention strategies.
This project aims to address the critical issue of employee attrition by leveraging data analytics and machine learning. By analyzing employee data, we seek to:
•
Identify key drivers of attrition: Uncover the primary factors that influence employees' decisions to leave the organization, such as job satisfaction, work-life balance, and compensation.
•
Develop predictive models: Create machine learning models that can accurately forecast which employees are at high risk of attrition, enabling proactive interventions.
•
Provide actionable insights: Offer HR teams valuable recommendations to improve employee retention and reduce turnover rates.
This project utilizes a dataset on employee attrition obtained from a public source provided by Unified Mentor.
Link :- “ https://drive.google.com/file/d/1tv2dfgghMKzN_mKmdn0ymCUrkwVvBk3w/view “
5
Methodology
The objective of this analysis is twofold: first, to understand the current turnover rates within the organization by identifying key factors that influence employee attrition, and second, to develop predictive models to forecast which employees are at the highest risk of leaving the company. This methodology outlines the steps taken to achieve these objectives.
A.
Dataset Description
The dataset comprises various employee-related features, which will be analyzed to understand turnover rates and to build a predictive attrition model. The dataset captures demographic, job-related, and satisfaction-based factors that may contribute to employee attrition. Our primary focus is on examining key variables such as job satisfaction, compensation, work-life balance, and job role in relation to employee attrition.
Features in the Dataset:
1.
Age (int): Represents the age of the employee in years.
2.
Attrition (object): Indicates whether the employee has left the company ("Yes") or is still employed ("No"). This is the target variable.
3.
BusinessTravel (object): Describes the employee's travel frequency. Categories include "Travel_Rarely," "Travel_Frequently," and "Non-Travel."
4.
DailyRate (int): The daily rate paid to the employee.
5.
Department (object): The department where the employee works, such as "Sales," "Research & Development," or "Human Resources."
6.
DistanceFromHome (int64): The distance, in miles, between the employee's home and the workplace.
7.
Education (int64): The education level achieved by the employee (1-5 scale).
8.
EducationField (object): The field in which the employee received their education (e.g., "Life Sciences," "Medical," "Marketing").
9.
EmployeeCount (int64): A constant value indicating the number of employees in the dataset.
6
10.
EmployeeNumber (int64): A unique identifier for each employee.
11.
EnvironmentSatisfaction (int64): Satisfaction with the work environment, rated on a scale from 1 (low) to 4 (high).
12.
Gender (object): The gender of the employee ("Male" or "Female").
13.
HourlyRate (int64): The hourly wage of the employee.
14.
JobInvolvement (int64): The level of job involvement, rated on a scale from 1 (low) to 4 (high). A key factor to understand commitment to the role.
15.
JobLevel (int64): The employee’s job level within the organization (e.g., entry-level, senior).
16.
JobRole (object): The employee’s job role, such as "Sales Executive," "Manager," or "Research Scientist." Job role will be explored to determine how certain roles correlate with attrition.
17.
JobSatisfaction (int64): Satisfaction with the job, rated from 1 to 4. This will be a critical factor in understanding employee attrition.
18.
MaritalStatus (object): The employee’s marital status (e.g., "Married," "Single," "Divorced").
19.
MonthlyIncome (int64): The fixed monthly salary of the employee. Salary is a key factor in understanding its correlation with turnover.
20.
MonthlyRate (int64): The varying monthly rate based on hours worked.
21.
NumCompaniesWorked (int64): The total number of companies the employee has previously worked for, potentially indicating job stability.
22.
Over18 (object): A constant value indicating if the employee is over 18 years old (all values are "Yes").
23.
OverTime (object): Indicates whether the employee works overtime ("Yes" or "No"). Work-life balance will be analyzed through this variable.
24.
PercentSalaryHike (int64): The percentage increase in salary that the employee received last year.
25.
PerformanceRating (int64): The employee’s performance rating on a scale from 1 to 4.
26.
RelationshipSatisfaction (int64): Satisfaction with workplace relationships, rated from 1 to 4.
27.
StandardHours (int64): The standard number of working hours (constant value of 80).
7
28.
StockOptionLevel (int64): The level of stock options available to the employee (0-3 scale).
29.
TotalWorkingYears (int64): The total number of years the employee has been working across all companies.
30.
TrainingTimesLastYear (int64): The number of training sessions the employee attended last year.
31.
WorkLifeBalance (int64): Satisfaction with work-life balance, rated on a scale from 1 (low) to 4 (high). Work-life balance is expected to be a strong indicator of attrition.
32.
YearsAtCompany (int64): The number of years the employee has spent at the current company.
33.
YearsInCurrentRole (int64): The number of years the employee has worked in their current role.
34.
YearsSinceLastPromotion (int64): The number of years since the employee’s last promotion, a potential driver of dissatisfaction.
35.
YearsWithCurrManager (int64): The number of years the employee has been working with their current manager.
B.
Exploratory Data Analysis (EDA)
The exploratory data analysis (EDA) focused on understanding the distribution and relationships between variables within the dataset. This section is divided into univariate, bivariate, and multivariate analyses to provide a comprehensive view of the data.
I. Univariate Analysis Insights
In the univariate analysis, we examined individual variables to identify trends, distributions, and potential areas of investigation. Key findings include:
1. Demographic and Role-Related Insights:
•
Age:
o
The age distribution is slightly right-skewed, suggesting that older employees are underrepresented or leave the company earlier.
8
This points to potential issues related to the retention of older
employees, which should be further investigated.
o
The majority of employees fall between the ages of 25 to 45, with the highest concentration between 30 to 37 years.
o
There is a noticeable decline in employee numbers after the age of 40, which may reflect recruitment trends favoring younger employees or challenges in retaining older employees.
•
Daily Rate:
o
The distribution of daily rates is fairly uniform, indicating consistent pay across different job roles, with slight variation possibly tied to seniority or specialization.
•
Distance from Home:
o
Most employees live close to the company, which may be due to its location in a densely populated area, or employees’ preference for shorter commutes. Factors such as traffic, transportation costs, and personal preferences could be contributing to this trend.
•
Education:
o
Education levels, treated as discrete variables, show that most employees have educational qualifications between levels 2 and 4, with a peak at level 3. This likely reflects a workforce with college or undergraduate degrees, which aligns with the company’s hiring focus on specialized expertise.
•
Employee Count:
o
This variable is constant across all employees and does not provide meaningful information for further analysis. It was excluded from predictive modeling.
2. Work Environment and Satisfaction:
•
Environment Satisfaction:
o
Most employees report being satisfied with their work environment. However, a small portion expresses significant dissatisfaction, indicating the need for targeted improvements in workplace conditions for this group.
•
Hourly Rate:
9
o
Hourly wages are distributed fairly evenly across employees, though variations likely correspond to differences in job levels or performance. This suggests that pay rates are well-structured but vary appropriately based on roles.
•
Job Involvement:
o
A majority of employees report moderate involvement in their roles. However, there is a small subset with low job involvement, which could be a point of concern for employee engagement and productivity.
•
Job Level:
o
Most employees are positioned in lower job levels, indicating limited upward mobility or a hierarchical company structure. This could potentially create challenges for career progression.
•
Job Satisfaction:
o
The distribution is left-skewed, with most employees expressing satisfaction with their jobs. However, there is a minority of dissatisfied employees, highlighting potential areas for improving job satisfaction.
3. Compensation and Career Progression:
•
Monthly Income:
o
The income distribution is right-skewed, indicating income inequality within the organization. While a significant proportion of employees earn between $2500 and $5000 per month, a smaller group earns considerably higher salaries.
•
Monthly Rate:
o
The monthly rate is evenly distributed among employees, reflecting a standardized compensation structure, with minor variations potentially tied to job performance and level.
•
Number of Companies Worked:
o
Most employees have worked for only one company, suggesting either strong employee loyalty or a focus on hiring new graduates with limited prior experience.
•
Percent Salary Hike:
10
o
The distribution is right-skewed, with only a few high performers receiving significant salary hikes. Most employees receive modest salary increases, typically in the range of 10% to 15%.
•
Performance Rating:
o
Performance ratings cluster around 3, with only a few employees receiving the highest rating of 4, reflecting a performance distribution that aligns with salary hikes.
4. Tenure and Career Development Insights:
•
Work-Life Balance:
o
The majority of employees rate their work-life balance as average (3), though a small group reports either extreme satisfaction or dissatisfaction, reflecting varied experiences across the workforce.
•
Years at Company:
o
The distribution is right-skewed, with employees tending to leave the company after 10 years. This may indicate that the company needs to focus on retaining long-term employees and addressing the reasons for their departure.
•
Years in Current Role:
o
Most employees change roles within 5 years, though a small portion remains in the same role for over 12 years. This may suggest limited opportunities for role changes or career growth for some employees.
•
Years Since Last Promotion:
o
The data reveals that most employees have been promoted within the past 1 to 2 years, indicating an active promotion structure. Further analysis is needed to assess whether promotions are distributed fairly.
•
Years with Current Manager:
o
The majority of employees have been with their current manager for a short period, while a small group has maintained longer-term relationships. These relationships may influence employee satisfaction and performance.
11
5. Other Factors:
•
Stock Option Level:
o
The stock option distribution is right-skewed, with most employees receiving 0 or 1 stock option. This suggests that stock options are limited to a select group of employees.
•
Total Working Years:
o
The right-skewed distribution indicates that most employees have between 5 and 12 years of experience. As total working years increase, employees are more likely to leave the company, highlighting the need for effective retention strategies for experienced workers.
•
Training Times Last Year:
o
The majority of employees underwent 2-3 training sessions in the previous year, while a few did not receive any training. This emphasizes the need for more comprehensive training programs to ensure continuous employee development.
II.
Bivariate Analysis Insights
Bivariate analysis was used to explore the relationships between pairs of variables. The following key insights were derived from this analysis:
•
Age vs. Attrition:
o
Younger employees (under 30) have a higher attrition rate, suggesting that the company may need to focus on retention strategies for this demographic. Conversely, employees above 35 are more likely to stay, indicating better stability in older age groups.
•
Gender and Job Level vs. Attrition:
•
Attrition rates are high in Job Level 1 for both genders. However, Job Level 4 shows much lower attrition rates, particularly among females, indicating that higher job levels contribute to greater employee retention.
•
Job Role vs. Attrition:
12
•
Roles such as Sales Representatives, Human Resources, and Laboratory Technicians experience high attrition, likely due to lower income levels. In contrast, roles such as Research Directors, Managers, and Healthcare Representatives demonstrate greater stability.
•
Education vs. Attrition:
•
Employees with degrees in Marketing, Human Resources, and Technical fields show higher attrition rates, suggesting that certain academic backgrounds may correlate with higher turnover.
III.
Multivariate Analysis Insights
•
Multivariate analysis explores the interaction between multiple variables, revealing complex patterns and insights that go beyond simple pairwise relationships:
•
Age, Gender, and Attrition:
•
Females over 35 exhibit significantly lower attrition rates compared to younger employees, suggesting that older female employees tend to have stronger loyalty to the company. Interestingly, divorced females over 35 show even stronger company loyalty, indicating a stable workforce within this demographic.
•
Job Role, Income, and Attrition:
•
Higher income is associated with lower attrition across most job roles, especially for employees in Job Level 4 and above. Non-traveling employees also tend to have lower attrition rates, further suggesting that stability is greater among employees who do not frequently travel for work.
•
Experience and Gender vs. Attrition:
•
Males with more work experience (i.e., those who have worked at multiple companies) show higher attrition rates, indicating that males with diverse work backgrounds may be more likely to leave, perhaps seeking better opportunities elsewhere. Note:- Demographic Positive and Negative Insight
• Negative Insights:
13
• Younger employees (under 30) and certain job roles such as Sales Representatives, Human Resources, and Laboratory Technicians have higher attrition rates, likely due to lower income levels and job satisfaction. • Males with more work experience show higher attrition, potentially reflecting a trend of job-hopping in pursuit of better opportunities.
• Positive Insights:
• Employees above 35, particularly females, tend to remain more loyal to the company.
• Higher job levels, especially Job Level 4, are associated with lower attrition, and roles such as Research Directors, Managers, and Healthcare Representatives show more stability.
• Non-traveling employees and divorced females over 35 demonstrate strong company loyalty.
Key Factors Influencing Turnover
Through a detailed analysis of employee behavior and organizational attributes, we identified various factors that either promote retention or contribute to higher attrition rates. These insights offer a clear view of areas where the company excels in retaining employees and where improvement is necessary.
Positive Factors Reducing Attrition:
•
Job Involvement:
o
Higher job involvement (levels 3 and 4) significantly correlates with lower attrition rates. This suggests that employees who are more engaged in their roles are more likely to stay with the company, underlining the importance of fostering active engagement.
•
Job Satisfaction:
o
Increased job satisfaction (levels 3 and 4) is linked to lower turnover. Employees who find fulfillment in their roles are far less likely to leave, indicating that addressing employee needs and satisfaction is key to retention.
14
•
Work-Life Balance:
o
A healthy work-life balance (levels 3 and 4) is a major driver of retention. Employees who feel that their workload allows for personal time are less inclined to leave, stressing the need for policies that support work-life equilibrium.
•
Environment Satisfaction:
o
Higher satisfaction with the workplace environment (levels 3 and 4) reduces the likelihood of attrition, emphasizing the importance of creating a positive and supportive work atmosphere.
•
Relationship Satisfaction:
o
Strong workplace relationships (levels 3 and 4) also contribute to lower attrition rates. Building supportive team dynamics and fostering positive relationships between employees and supervisors can help retain talent.
•
Monthly Income:
o
Employees with higher median monthly incomes are less likely to leave, highlighting the role that competitive salaries play in employee retention. Compensation is a significant motivating factor for loyalty.
•
Stock Options:
o
Employees who are offered stock options, particularly at higher levels (up to level 4), are more likely to stay with the company. Stock options align employees' financial interests with the company’s long-term success, incentivizing retention.
•
Job Levels:
o
Senior employees, particularly those in Job Levels 4 and 5, show lower attrition rates. This suggests that experienced employees are generally more satisfied and that advancing employees into higher job levels can foster long-term commitment.
•
Retention of Experienced Employees:
o
Employees with more total working years, especially those who are married or divorced, demonstrate better retention. This indicates that experienced employees tend to stay longer, and focusing on retaining this group can be beneficial for the company’s long-term stability.
15
Negative Factors Increasing Attrition:
•
Low Job Involvement:
o
Employees with low job involvement (level 1) have the highest attrition rate, at 33.7%. This suggests that those who are not engaged in their roles are more likely to leave, indicating the need for initiatives that increase employee engagement.
•
Low Job Satisfaction:
o
Low satisfaction (level 1) drives a 22.8% attrition rate. Dissatisfaction with job responsibilities, opportunities, or the work environment is a significant factor in employees leaving the company.
•
Poor Work-Life Balance:
o
Poor work-life balance (level 1) results in the highest attrition rate, at 31.25%. Employees who struggle to balance work with their personal lives are much more likely to leave, making work-life balance a critical area for improvement.
•
Low Environment Satisfaction:
o
Employees with low satisfaction regarding their work environment (level 1) have a 25.35% attrition rate. Addressing factors such as workplace conditions, management practices, and overall culture is crucial to retaining these employees.
•
Low Relationship Satisfaction:
o
Poor workplace relationships (level 1) result in a 20.65% attrition rate, showing that conflicts, lack of support, or poor communication are significant drivers of turnover.
•
No Stock Options:
o
Employees without stock options (level 0) show an attrition rate of 24.40%. Offering more stock options can help align employees with the company’s long-term goals and reduce turnover.
•
Early Career Attrition:
o
Employees who are in the early stages of their careers, particularly those who are single and have fewer total working years, are
16
more likely to leave. This indicates a need to focus on career
development and engagement for younger or less experienced
employees.
• Years Since Last Promotion:
o Employees who have gone a long time without a promotion and
who frequently work overtime are more likely to leave. This
suggests that career stagnation, combined with high workloads,
contributes to higher attrition.
• Multiple Companies Worked:
o Employees who have worked for several companies prior to their
current role, particularly males, show higher attrition rates. This
may reflect a lack of long-term commitment and suggests that
these employees are more likely to leave in pursuit of better
opportunities.
• Distance from Home:
o Employees living farther from the workplace, particularly those in
lower job levels, are more likely to leave. Commute times and
related factors such as transportation costs and stress may impact
their decision to stay with the company.
o
These are one – one graph of univariate ,bivariate and multivariate analysis :-
Univariate Analaysis graph
17
Bivariate Analysis Graph
18
Highlights key areas where the company can focus its efforts to improve
employee retention, particularly by enhancing job involvement, satisfaction,
work-life balance, and career progression opportunities.
Model Development
1. Problem Statement and Objective
The objective of this project is to develop a machine learning model to predict
employee attrition using the IBM HR dataset. The model will help the
organization identify which employees are at the highest risk of leaving the
company, allowing for proactive measures to retain them.
2. Data Preprocessing
a. Missing Value Detection
The dataset was initially analyzed for missing values using isnull() and basic
summary statistics. Since the IBM dataset is relatively clean, no missing values
were found. However, checks were performed to ensure the dataset's
integrity.
Multivariate Analysis Graph
19
b. Duplicate Value Checking
To ensure the dataset was clean, a check for duplicates using the duplicated() function was performed. No duplicate records were found, confirming the uniqueness of the data.
c. Outlier Detection and Handling
Outliers in continuous features such as MonthlyIncome and YearsAtCompany were detected using histograms and boxplots:
•
Trimming: Initially, outliers were removed using the trimming method. However, this led to a significant loss of data.
•
Capping: To minimize data loss, extreme values were capped at the 1st and 99th percentiles to limit their influence while retaining the majority of the dataset.
d. Feature Transformation
Since some variables exhibited skewness, Power Transformation was applied to improve data distribution and model performance:
•
Both Box-Cox and Yeo-Johnson transformations were tested.
•
Q-Q plots were used to compare the effects of these transformations, and Yeo-Johnson performed better, as it handles negative and zero values, which were present in the dataset.
e. Encoding Categorical Variables
The dataset contained categorical variables like JobRole, Department, and EducationField, which were encoded using OneHotEncoding. This transformed these categorical features into numerical representations that could be processed by machine learning algorithms.
20
f. Scaling
Continuous variables were scaled using StandardScaler to ensure that all features were on the same scale, which is particularly important for models like Logistic Regression and Support Vector Machines (SVM).
g. Handling Imbalanced Dataset
The dataset exhibited an imbalance between employees who left the company (attrition = 1) and those who stayed (attrition = 0). To address this imbalance, SMOTE (Synthetic Minority Over-sampling Technique) was applied. This technique generates synthetic samples for the minority class (attrition = 1), thus balancing the dataset.
3. Feature Selection
Feature selection was conducted iteratively to improve model performance:
•
Recursive Feature Elimination (RFE) was applied to identify the most important features.
•
Feature importance from tree-based models like Random Forest was also used to assess the relevance of different features.
•
Multiple rounds of feature selection were conducted, and after each round, the models were retrained and evaluated to check for improvements in accuracy, recall, and other metrics.
4. Model Selection and Training
Several machine learning models were trained, evaluated, and compared. The following models were tested:
•
Logistic Regression
•
DecisionTreeClassifier
•
Naive Bayes (GaussianNB)
•
Support Vector Classifier (SVC)
•
K-Nearest Neighbors (KNN)
•
Voting Classifier
21
•
Bagging Classifier
•
Random Forest
•
AdaBoost Classifier
•
Gradient Boosting Classifier
•
XGBoost
5. Cross-Validation and Hyperparameter Tuning
To improve model generalization and avoid overfitting, Cross-Validation was applied:
•
RandomizedSearchCV was initially used to explore a wide range of hyperparameter combinations.
•
GridSearchCV was then applied for fine-tuning the hyperparameters to find the best possible combination.
•
For each model, multiple sets of features were tested in combination with different hyperparameter values, and cross-validation scores were compared.
6. Model Evaluation
Each model was evaluated based on the following performance metrics:
•
Accuracy: Measures the overall correctness of the model.
•
Recall: Given the importance of identifying employees at risk of attrition, recall was prioritized to reduce false negatives.
•
Precision: Measures the proportion of correct positive predictions (employees predicted to leave) out of all positive predictions.
•
Confusion Matrix: Used to provide a detailed breakdown of true positives, false positives, true negatives, and false negatives.
7. Model Results
The performance of each model is summarized below:
22
Logistic Regression:
•
Accuracy: 0.80
•
Cross Validation Score: 0.80
•
Recall: 0.77
•
Precision: 0.41
•
Confusion Matrix: [ [202 48]
[10 34] ]
Support vector classifier (SVC):
•
Accuracy: 0.84
•
Cross Validation Score: 0.94
•
Recall: 0.34
•
Precision: 0.44
•
Confusion Matrix: [ [221 19]
[29 15] ]
KNeighbors Classifier (KNN): Here we give two best rest one best of accuracy and one on recall score.
•
Accuracy: 0.74
•
Cross Validation Score: 0.84
•
Recall: 0.64
•
Precision: 0.32
•
Confusion Matrix: [ [191 59]
[16 28] ]
GaussianNB :
•
Accuracy: 0.74
•
Cross Validation Score: 0.73
•
Recall: 0.72
•
Precision: 0.33
23
•
Confusion Matrix: [ [186 64]
[16 32] ]
DecisionTreeClassifier:
•
Accuracy: 0.80 | 0.59
•
Cross Validation Score: 0.82 | 0.75
•
Recall: 0.48 | 0.70
•
Precision: 0.37 | 0.22
•
Confusion Matrix: [[214 36]]
[23 21]]
Voting Ensemble:
•
Accuracy: 0.86
•
Cross Validation Score:
•
Recall: 0.48
•
Precision: 0.55
•
Confusion Matrix: [[233, 17],[23, 21]]
Bagging:
•
Accuracy: 54
•
Cross Validation Score:
•
Recall: 73
•
Precision: 20
Random Forest:
•
Accuracy:0. 87
•
Cross Validation Score:
•
Recall: 0.59
•
Precision: 0.43
24
•
Confusion Matrix: [[215,35][18,26]]
Adaboost Classifier:
•
Accuracy: 0.88
•
Cross Validation Score:
•
Recall: 0.55
•
Precision: 0.63
•
Confusion Matrix: [[236,14][20,14]]
Gradient Boosting:
•
Accuracy: 0.87
•
Cross Validation Score:0.92
•
Recall: 0.45
•
Precision: 0.60
•
Confusion Matrix: [[237 13][24 20]]
XGBoost:
•
Accuracy: 87
•
Cross Validation Score:
•
Recall: 36
•
Precision:
•
Confusion Matrix:
8. Final Model Selection
The final model selected for this project is Adaboost Classifier. It was chosen due to its superior balance between accuracy, recall, and precision. The final metrics of the selected model are as follows:
•
Accuracy: 0.88
•
Cross Validation Score:
25
•
Recall: 0.55
•
Precision: 0.63
•
Confusion Matrix: [[236,14][20,14]]
9. Conclusion
The final model successfully predicts employee attrition, allowing the organization to take proactive steps in employee retention. The model was fine-tuned and optimized through feature selection, cross-validation, and hyperparameter tuning, resulting in a model that performs well in identifying employees at risk of attrition.

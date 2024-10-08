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

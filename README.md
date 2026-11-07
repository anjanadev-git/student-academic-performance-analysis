Student Academic Performance & Learning Risk Analysis

A Data Science Take-Home Project | IIT Madras CODE – School Connect

📌 Project Overview

This project explores student academic performance and learning-related patterns using Exploratory Data Analysis (EDA), K-Means Clustering, and Decision Tree Classification.

Using a dataset of 200 student records, the project investigates relationships between academic performance, study habits, attendance, sleep duration, and internet usage. It also applies machine learning techniques to identify student groups and examine patterns associated with different academic risk categories.

This project was completed as a Take Home Project for the Introduction to Data Science and AI course offered by the Centre for Outreach and Digital Education (CODE), Indian Institute of Technology Madras.

🎯 Objectives

- Explore student academic and behavioural characteristics.
- Identify relationships between learning habits and academic performance.
- Apply K-Means Clustering to identify groups of students with similar characteristics.
- Develop a Decision Tree Classification model to examine academic risk categories.
- Evaluate model performance and interpret the resulting patterns.

📊 Dataset Description

The dataset consists of 200 student records and the following variables:

Feature  Description 

StudentID - Unique student identifier
Age - Student age
Gender - Student gender
StudyHoursPerWeek - Weekly study hours
AttendancePercentage - Attendance percentage
AssignmentScore - Assignment performance
PreviousExamScore - Previous examination score
SleepHours - Average sleep hours 
InternetUsageHours - Internet usage hours
AcademicRisk - Academic risk category

Academic risk categories:
- Low: 80 students
- Medium: 70 students
- High: 50 students

🛠️ Tools & Technologies

Orange Data Mining: Data analysis, clustering, classification and model evaluation.
Spreadsheet Software: Initial data inspection and validation.
Machine Learning: K-Means Clustering and Decision Tree Classification.

🔍 Methodology

1. Data Cleaning and Exploratory Data Analysis (EDA)

Initial data inspection was conducted to check for missing values, duplicate records and suspicious entries.

Descriptive statistics were calculated to understand the distribution of the dataset.

A correlation analysis identified a positive relationship between weekly study hours and previous examination scores (correlation coefficient: 0.7283).
 Key observations:

- Weekly study hours and previous examination scores showed a strong positive correlation (Pearson correlation coefficient: 0.7283).
- Students in the High-risk category had lower median attendance than those in the Low-risk category.
- Median sleep duration was lower in the High-risk category than in the Low-risk category.
- Internet usage was highest in the High-risk category and lowest in the Low-risk category.

2. K-Means Clustering

K-Means Clustering was applied to identify patterns among students based on their academic and learning-related characteristics.

- Number of clusters (K): 3
- Features were normalised before clustering.
- StudentID, Age and Gender were excluded from the clustering analysis.

Key observations:

- Cluster 1 predominantly consisted of students in the Medium academic risk category.
- Cluster 2 contained a high proportion of students classified as High risk (47 out of 50).
- Cluster 3 predominantly consisted of Low-risk students (80 out of 81).

These clusters revealed distinct patterns in the dataset.

3. Decision Tree Classification

A Decision Tree Classification model was developed to analyse the relationship between student characteristics and academic risk categories.

Model evaluation was conducted using 10-fold stratified cross-validation.

The model achieved:

Evaluation Metric        |        Result
Classification Accuracy           77.0% 
Precision                         77.1% 
Recall                            77.0% 
F1-Score                          75.4% 

Assignment Score and Attendance Percentage were identified as important splitting features in the resulting decision tree.

Confusion Matrix Findings:
- High risk: 42 out of 50 correctly classified.
- Low risk: 78 out of 80 correctly classified.
- Medium risk: 34 out of 70 correctly classified.
The model classified Low-risk students most effectively, while Medium-risk students were more difficult to distinguish.

Important Decision Tree features:

- AssignmentScore was selected as the root node, followed by AttendancePercentage.
- The resulting tree used normalized thresholds of 0.58982 for AssignmentScore and 0.47333 for AttendancePercentage.
- These thresholds represent normalized feature values rather than original marks or percentages.

📈 Key Findings

- Study habits and academic performance: Weekly study hours showed a positive association with previous examination scores.
- Attendance and academic risk: Higher attendance was associated with lower academic risk in the dataset.
- Lifestyle patterns: Sleep duration and internet usage differed across academic risk categories.
- Unsupervised learning: K-Means identified three groups that aligned strongly with the original academic risk labels.
- Classification: The Decision Tree achieved 77% accuracy, with AssignmentScore and AttendancePercentage forming its first two decision splits.
- Model interpretability: Decision Tree rules provided an understandable way to examine how predictions were formed.
  
  Limitations
- The dataset contains 200 student records and may not represent broader student populations.
- The findings may not generalize to other student populations.
- The models identify associations and patterns, not causal relationships.
- The Decision Tree had difficulty distinguishing Medium-risk students.
- Future work could investigate larger datasets, additional learning-related variables, alternative classification algorithms and systematic cluster evaluation using methods such as silhouette analysis.

Project Documentation

The repository includes:

- report/ – Detailed project report.
- presentation/ – Project presentation.
- screenshots/ – Visualisations and results from Orange Data Mining.
- data/ – Dataset, if permitted for public distribution.

🎓 Acknowledgement

This project was completed as part of the "Introduction to Data Science and AI" course offered by IIT Madras CODE through the School Connect programme.

I was awarded a Certificate of Appreciation by IIT Madras CODE in recognition of my work on this Take Home Project.


Author: A. Anjana Sanjeshree

Institution: Indian Institute of Technology Madras – CODE (School Connect)

Project Category: Data Science & Machine Learning

Year: 2026

This project is an educational exploration of data science and machine learning techniques using student academic performance data.

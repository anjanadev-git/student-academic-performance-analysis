Student Academic Performance & Learning Risk Analysis

A Data Science Take-Home Project | IIT Madras CODE – School Connect

📌 Project Overview

This project explores student academic performance using data analysis and machine learning techniques. The objective is to identify patterns in academic performance, understand relationships between different learning-related factors, and examine how students can be grouped according to their academic risk levels.

The project was completed as a Take Home Project for the **Introduction to Data Science and AI** course offered by the Centre for Outreach and Digital Education (CODE), Indian Institute of Technology Madras.

🎯 Objectives

- Analyse student academic performance using relevant academic and lifestyle-related variables.
- Identify relationships between study habits, attendance, examination performance, and other factors.
- Apply K-Means Clustering to discover patterns among student groups.
- Develop a Decision Tree Classification model to analyse academic risk categories.
- Evaluate model performance and interpret the findings.

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
Spreadsheet Software :Initial data inspection and validation.
Machine Learning: K-Means Clustering and Decision Tree Classification.

🔍 Methodology

1. Data Cleaning and Exploratory Data Analysis (EDA)

Initial data inspection was conducted to check for missing values, duplicate records and suspicious entries.

Descriptive statistics were calculated to understand the distribution of the dataset.

A correlation analysis identified a positive relationship between weekly study hours and previous examination scores (correlation coefficient: 0.7283).

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

📈 Key Findings

- Weekly study hours demonstrated a positive correlation with previous examination scores.
- K-Means clustering revealed distinguishable patterns among the three academic risk categories.
- Assignment performance and attendance were important features in the Decision Tree model.
- The classification model achieved 77% accuracy, demonstrating its ability to identify academic risk patterns within this dataset.

Limitations

- The dataset contains 200 student records and may not represent broader student populations.
- Observed relationships do not necessarily establish causation.
- Model performance may vary with different datasets and student populations.
- The model is intended for educational analysis and exploration, not as a standalone system for making decisions about individual students.

Project Documentation

The repository includes:

- report/ – Detailed project report.
- presentation/ – Project presentation.
- screenshots/ – Visualisations and results from Orange Data Mining.
- data/ – Dataset, if permitted for public distribution.

## 🎓 Acknowledgement

This project was completed as part of the "Introduction to Data Science and AI" course offered by IIT Madras CODE through the School Connect programme.

I was awarded a Certificate of Appreciation by IIT Madras CODE in recognition of my work on this Take Home Project.



Author: A. Anjana Sanjeshree

Institution: Indian Institute of Technology Madras – CODE (School Connect)

Project Category: Data Science & Machine Learning

Year: 2026

# Hiring Prediction Model

## Project Overview
This repository contains a machine learning project that compares different binary classification algorithms to predict whether an interviewed job candidate will be hired based on various features. The project was completed as part of the IBM Machine Learning Professional Certificate on Coursera.

## Project Description
Using a dataset from Kaggle ("Predicting Hiring Decisions in Recruitment Data"), this project explores which factors are most important in determining whether a candidate is hired. The analysis implements and compares four different classification algorithms:

- K-Nearest Neighbors
- Logistic Regression (with polynomial features)
- Support Vector Classification (with RBF kernel)
- Decision Tree

Each model was optimized through hyperparameter tuning using grid search cross-validation with the F1-score as the evaluation metric.

## Key Findings
- The decision tree classifier was identified as the best-performing model with an out-of-sample F1-score of 0.84 and accuracy of 0.91
- The recruitment strategy emerged as the most important feature in determining hiring outcomes
- Candidates were found to be more successful during aggressive hiring campaigns compared to moderate ones
- Personality score was the second most important feature (about half as important as recruitment strategy)
- Experience years, interview score, and skill score had similar importance levels (about 40% of the recruitment strategy importance)
- Education level was the least important among the selected features (about 25% of the recruitment strategy importance)

## Features
The dataset includes the following features:
1. Age - Age of the candidate in years
2. Gender - 0 = Male, 1 = Female
3. EducationLevel - 1 = Bachelor's Type 1, 2 = Bachelor's Type 2, 3 = Master's, 4 = Ph.D.
4. ExperienceYears - Candidate's professional experience in years
5. PreviousCompanies - Number of companies the candidate has worked for previously
6. DistanceFromCompany - Distance in kilometers from candidate's residence to the company
7. InterviewScore - Score between 0 and 100 assigned based on the interview
8. SkillScore - Score between 0 and 100 assigned based on technical skills
9. PersonalityScore - Score between 0 and 100 assigned based on personality traits
10. RecruitmentStrategy - 1 = Aggressive, 2 = Moderate, 3 = Conservative
11. HiringDecision - 0 = Not Hired, 1 = Hired (target variable)

## Repository Structure
- `project-document/`: Contains the full project report with detailed analysis and methodology
- `notebook/`: Contains the Jupyter notebook with all code and visualizations
- `figures/`: Visualizations generated during the analysis

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Future Work
Potential areas for further investigation include:
- Analyzing why the recruitment strategy is the most important factor in hiring decisions
- Exploring the factors that lead to success conditioned on specific recruitment strategies
- Deeper analysis of the decision tree structure to gain additional insights

## Author
Anthony R. Poggioli

## Date
July 3, 2024

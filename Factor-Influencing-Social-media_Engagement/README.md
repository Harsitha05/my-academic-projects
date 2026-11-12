## 📚 Project Background
This is my First Academic Project, completed as part of my Master of Data Science programme.
It is a foundational data science project that helped me gain practical experience in data collection, data preprocessing, exploratory data analysis, statistical analysis, and machine learning using Multiple Linear Regression.

# Factors Influencing Social Media Engagement
### A Multiple Linear Regression Approach

## 📌 Project Overview
This project analyzes the factors that influence social media engagement and user satisfaction using Multiple Linear Regression.
It explores how user behaviour, posting frequency, interaction patterns, and other factors are related to satisfaction with social media engagement.

## 🎯 Objectives
- Identify the major factors influencing social media engagement.
- Analyze user behaviour and interaction patterns.
- Understand the relationship between social media activities and satisfaction.
- Predict user satisfaction using Multiple Linear Regression.

## 📊 Dataset
- **Data Source:** Google Forms Survey
- **Number of Respondents:** 51
- **Data Format:** CSV
- **Data Collection:** Google Forms and Google Sheets

The dataset includes information such as:
- Age and Gender
- Occupation
- Daily time spent on social media
- Posting frequency
- Types of content shared
- Number of social media platforms used
- Reaction and sharing frequency
- Importance given to likes and reactions
- Time spent creating posts
- Social media satisfaction score

## 🛠️ Technologies Used
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

## ⚙️ Project Workflow

1. **Data Collection:** Collected responses through a Google Forms survey.
2. **Data Preprocessing:** Loaded the dataset, handled categorical variables, and prepared the data for analysis.
3. **Exploratory Data Analysis:** Analyzed user behaviour and visualized patterns using charts and graphs.
4. **Feature Encoding:** Converted categorical variables into numerical values using one-hot encoding.
5. **Model Building:** Applied Multiple Linear Regression to predict satisfaction scores.
6. **Model Evaluation:** Evaluated model performance using R², Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
7. **Statistical Analysis:** Examined regression coefficients and p-values to identify significant factors.

## 🤖 Machine Learning Algorithm
**Multiple Linear Regression**

Multiple Linear Regression was used because the project aims to predict a continuous dependent variable (Satisfaction Score) using multiple independent variables.

## 📈 Model Performance

| Evaluation Metric | Result |
|---|---:|
| R² Score | 0.68 |
| Adjusted R² Score | 0.62 |
| Mean Squared Error (MSE) | 2.87 |
| Root Mean Squared Error (RMSE) | 1.69 |
| F-statistic | 11.45 |

## 🔍 Key Findings
- Caring about likes and reactions showed a strong positive relationship with satisfaction.
- Posting frequency positively influenced satisfaction.
- Interacting with others through reactions and comments was also an important factor.
- Age showed a small positive influence.
- Daily time spent and content type were not statistically significant predictors in the analysis.

## 💡 Conclusion
The project identifies important behavioural factors associated with social media engagement and user satisfaction.
The Multiple Linear Regression model achieved an R² score of 0.68, indicating that it explains 68% of the variation in satisfaction scores within the analyzed dataset.

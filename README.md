# Employee-Performance-Prediction

## Project Summary

### 1. Requirement

The objective of this project was to analyze employee performance data for INX Future Inc. and develop a predictive model that can accurately classify employee performance ratings. The organization aims to understand the major factors influencing employee performance so that management can make informed decisions regarding employee development, performance improvement, and workforce planning.

The project was designed to achieve the following objectives:

* Analyze employee performance across different departments.
* Identify the most influential factors affecting employee performance.
* Build and compare multiple machine learning classification models.
* Select the best-performing model for predicting employee performance.
* Provide practical recommendations that can help improve employee productivity and overall organizational performance.

### 2. Analysis

The dataset contained **1,200 employee records with 28 attributes**, including employee demographics, job-related factors, satisfaction metrics, experience details, and the target variable **PerformanceRating**.

The analysis included:

* Performed data exploration and identified **19 numerical and 9 categorical variables** with **no missing values**.
* Conducted department-wise performance analysis to compare employee ratings across departments.
* Applied **Label Encoding** to convert categorical variables into numerical format for machine learning.
* Used correlation analysis and business relevance to select **9 important features** for model development.
* Split the data into **70% training and 30% testing sets** and applied **StandardScaler** for feature normalization.
* Built and evaluated eight classification models:
  
    * Logistic Regression
    * K-Nearest Neighbor
    * Decision Tree
    * Random Forest
    * Support Vector Machine
    * Gaussian Naive Bayes
    * Artificial Neural Network
    * XGBoost
  
* Evaluated model performance using **Accuracy**, **Precision**, **Recall**, **F1-score**, and **Confusion Matrix**.

### 3. Summary

This project successfully developed a machine learning solution for predicting employee performance while identifying the organizational factors that contribute most significantly to performance ratings.

The overall workflow included:

* Loading and exploring the employee dataset.
* Performing data quality checks and understanding the dataset structure.
* Analyzing department-wise employee performance.
* Encoding categorical variables into numerical values.
* Performing correlation analysis to identify important predictors.
* Selecting the most relevant features for model building.
* Splitting the dataset into training and testing subsets.
* Applying feature scaling where appropriate.
* Training and evaluating eight different machine learning classification algorithms.
* Selecting the best-performing model and saving it for future predictions.

### 4. Results

Dataset Overview
  * Total Employee Records: 1,200
  * Total Features: 28
  * Numerical Features: 19
  * Categorical Features: 9
  * Missing Values: None


**Department-wise Average Performance**       
| Department | Average Performance Rating |
| :--- | :---: |
| Development | 3.08 |
| Data Science | 3.05 |
| Human Resources | 2.93 |
| Research & Development | 2.92 |
| Sales | 2.86 |
| Finance | 2.78 |


* Among all departments, Development recorded the highest average employee performance, while Finance recorded the lowest average performance rating.

**Model Performance Comparison** 
| Model | Accuracy |
| :--- | :---: |
| K-Nearest Neighbor | 81.9% |
| Gaussian Naive Bayes | 82.5% |
| Logistic Regression | 82.5% |
| Artificial Neural Network | 85.6% |
| Support Vector Machine | 86.4% |
| Decision Tree | 90.0% |  
| XGBoost | 91.4% |
| Random Forest (GridSearchCV) | 94.4% |


* The **Random Forest classifier** optimized using **GridSearchCV** achieved the highest prediction accuracy of **94.4%**, making it the most suitable model for predicting employee performance in this study.


### 5. Analysis and Insights
* The dataset contained **1,200 employee records with no missing values**, enabling reliable analysis and model development.
* Department-wise analysis showed that **Development** and **Data Science** had the highest average performance ratings, while **Finance** had the lowest.
* **Random Forest** achieved the **highest prediction accuracy (94.44%)**, followed by **XGBoost (91.4%)** and **Decision Tree (90.00%)**, indicating that tree-based models were the most effective for predicting employee performance.
* Feature importance analysis identified **Employee Last Salary Hike Percent**, **Employee Environment Satisfaction**, and **Years Since Last Promotion** as the three most influential factors affecting employee performance.
* The results indicate that employee performance is strongly influenced by **recognition through salary growth**, **a positive work environment**, and **timely career progression**, while factors such as job role, department, work-life balance, and experience also contribute to prediction accuracy.

  
### 6. Recommendations
* Implement **performance-based salary increments**, as **Last Salary Hike Percent** was identified as the most important factor influencing employee performance.
* Improve employee satisfaction by fostering a supportive work environment, encouraging employee engagement, and strengthening leadership practices.
* Establish **clear promotion and career development pathways** to reduce long promotion gaps and maintain employee motivation.
* Continue supporting **work-life balance** through flexible work policies and employee wellness initiatives.
* Use the **Random Forest prediction** model to identify employees who may require additional training, mentoring, or performance support.
* Give additional attention to departments with comparatively lower average performance, particularly Finance, by implementing targeted improvement strategies.

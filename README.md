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
| Development | 3.09 |
| Data Science | 3.05 |
| Human Resources | 2.93 |
| Research & Development | 2.92 |
| Sales | 2.86 |
| Finance | 2.78 |


* Among all departments, Development recorded the highest average employee performance, while Finance recorded the lowest average performance rating.

**Model Performance Comparison** 
| Model | Accuracy |
| :--- | :---: |
| Gaussian Naive Bayes | 81.7% |
| Logistic Regression | 82.2% |
| K-Nearest Neighbor | 83.1% |
| Artificial Neural Network | 86.1% |
| Support Vector Machine | 87.8% |
| Decision Tree | 88.6% |
| XGBoost | 89.7% |
| Random Forest (GridSearchCV) | 92.8% |


* The **Random Forest classifier** optimized using **GridSearchCV** achieved the highest prediction accuracy of **92.8%**, making it the most suitable model for predicting employee performance in this study.


### 5. Analysis and Insights
* The dataset contained **1,200 records with no missing values**, allowing reliable analysis and model development without extensive data cleaning.
* Department-wise analysis showed that **Development** and **Data Science** had the highest average performance ratings, while **Finance** and **Sales** showed comparatively lower performance.
* Correlation analysis identified **Employee Environment Satisfaction (0.396)** as the strongest factor influencing performance, followed by **Employee Last Salary Hike Percent (0.334)** and **Employee Work-Life Balance (0.124)**.
* Factors such as **Years Since Last Promotion, Experience Years in Current Role, Years With Current Manager, and Experience Years at This Company** showed negative relationships with performance, which may indicate reduced motivation due to limited career growth or prolonged role duration.
* Tree-based ensemble models performed best among all algorithms tested. **Random Forest achieved the highest accuracy (92.8%), followed by XGBoost (89.7%)**, showing their effectiveness for employee performance prediction.
* Model evaluation showed that predictions were more accurate for the majority performance class (Rating 3), while identifying employees with Ratings 2 and 4 was more challenging due to fewer records in those categories.

### 6. Recommendations
* Improve **employee environment satisfaction** by promoting a positive workplace culture, employee engagement, and supportive leadership.
* Implement **performance-based rewards and salary growth opportunities** to encourage higher productivity.
* Support **work-life balance** through flexible policies and manageable workloads.
* Provide clearer **career growth and promotion opportunities** to reduce employee dissatisfaction.
* Review **managerial assignments and leadership practices** to maintain employee engagement.
* Use the **Random Forest prediction model** to identify employees needing additional support or development.
* Focus improvement efforts on lower-performing departments such as **Finance and Sales** through targeted interventions.

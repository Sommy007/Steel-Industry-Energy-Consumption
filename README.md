PROJECT OVERVIEW:
This project aims to develop and evaluate machine learning classification algorithms to predict the power load type in a smart steel manufacturing industry. The dataset, obtained from DAEWOO Steel Co. Ltd. in Gwangyang, South Korea, contains electricity consumption and operational data collected from a cloud-based energy monitoring system. The company manufactures various steel products, including coils, steel plates, and iron plates, while its energy consumption records are managed through the Korea Electric Power Corporation's energy management platform.

The dataset consists of 35,040 observations and 10 variables (9 predictor variables and 1 target variable), with no missing values. The predictor variables include energy consumption (kWh), lagging and leading reactive power (kVarh), CO₂ emissions, lagging and leading power factors, the number of seconds from midnight (NSM), week status (weekday or weekend), and day of the week. The target variable, Load_Type, categorizes electricity demand into three classes: Light Load, Medium Load, and Maximum Load.

The primary objective of this project is to compare the performance of different classification algorithms and identify the model that most accurately predicts the load type based on the operational and electrical characteristics of the steel manufacturing process. Accurate load type prediction can improve energy management, optimize electricity usage, reduce operational costs, and support more efficient decision-making in industrial environments. This study also demonstrates the application of data analytics and machine learning techniques to smart manufacturing and sustainable energy management systems.


PROJECT GOAL:
This project aims to use supervised machine learning (classification) to predict the Load Type (Light, Medium, or Maximum Load) of energy consumption in a smart steel manufacturing industry using operational and electrical data.

VARIABLES:
Target(Output): Load_Type

Features (Input):
Usage_kWh(kWh), Lagging_Current_Reactive.Power_kVarh(kVarh), Leading_Current_Reactive_Power_kVarh (kVarh), CO2(tCO2) (ppm), Lagging_Current_Power_Factor (%), Leading_Current_Power_Factor (%), Number of Seconds from midnight, NSM (s), Day_of_week, WeekStatus.

DATA SOURCE:
This project uses a publicly available dataset that follows standard academic citation practices.

Dataset Name: Steel Industry Energy Consumption
Source: UCI Machine Learning Repository
Authors: Sathishkumar V. E., Changsun Shin, and Yongyun Cho
Year: 2021
DOI / Reference: https://doi.org/10.24432/C52G8C


METHODOLOGY:
The project follows a structured machine learning workflow:
- Data Overview/collection
- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Feature Analysis
- Model Evaluation
- Model Selection

KEY FINDINGS:
* Contrary to expectations, Medium_load poses a greater carbon management challenge than Maximum_load due to its high variable, unpredictable emission distribution.
* The energy consumption follows a clear bimodal daily pattern, two distinct ~ 4 to 5 hours high-usage windows (~7:46 AM - 12:30 PM and ~ 5:13 PM - 8:00 PM) separated by a midday dip strongly suggesting double-shift industrial operations. 
* Sunday stoodout as a near-complete shutdown day, almost all power readings are Light_Load.
* The facility's biggest inefficiency is during Light_Load and Weekday heavy operations, where reactive power demand is disproportionately high relative to useful energy consumed.
* Random Forest outperformed Logistic Regression, SVC, and KNN by leveraging its ensemble of decision trees to robustly capture nonlinear feature interactions that single or distance-based models could not effectively learn.
* The feature importance analysis indicates that NSM is the most influential predictor, contributing approximately 43.6% of the model's predictive power.

TECH STACK:
Programming Language: Python
Libraries: NumPy, Pandas, Matplotlib, Seaborn
Machine Learning: Scikit-Learn
Model Used: Logistic Regression, RandomForest, K-Nearest Neighbors (KNN) Classifier, Support Vector Machine (SVC)
Environment: Jupyter Notebook

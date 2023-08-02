
# Laptop Price Predictor

**Problem Statement**

Laptops have become an essential tool for numerous occupations in the modern age, from business and school to entertainment and communication. As the demand for laptops continues to grow, both consumers and manufacturers seek insights into the factors that influence laptop prices. The goal of this project is to develop a prediction model that leverages regression algorithms to provide accurate estimates of laptop prices based on various features.

**Objective**
The primary objective of this project is to build a robust and accurate laptop price prediction model . By analyzing factors such as brand, specifications, hardware components, and operating system, we aim to create a model that can predict laptop prices with a high degree of precision. The insights gained from this model can aid in making informed decisions about pricing, purchasing, and market strategies.

**Prerequisite**

* Anaconda 3
* Python 3

**Dataset Description**

| Feature | Description |
|---------|-------------|
| laptop_ID | A unique identifier for each laptop in the dataset. |
| Company | The manufacturer or brand of the laptop. |
| Product | The specific model or name of the laptop product. |
| TypeName | The general category or type of the laptop (e.g., Ultrabook, Notebook, Gaming, etc.). |
| Inches | The size of the laptop screen in inches. |
| ScreenResolution | The resolution of the laptop screen, including details about the panel type (e.g., IPS Panel, Touchscreen) and resolution (e.g., Full HD 1920x1080). |
| Cpu | The Central Processing Unit (CPU) of the laptop, including details about the processor's brand and speed. |
| Ram | The amount of Random Access Memory (RAM) in gigabytes (GB) available in the laptop. |
| Memory | The storage capacity of the laptop, typically specifying the type and size of storage (e.g., SSD, HDD) and any combination. |
| Gpu | The Graphics Processing Unit (GPU) of the laptop, including details about the graphics card. |
| OpSys | The operating system installed on the laptop (e.g., Windows, macOS, Linux). |
| Weight | The weight of the laptop in kilograms (kg). |
| Price | The price of the laptop in Rupees. |


**Working Flow**

 **1.Import Libraries** : Import necessary Python libraries, including scikit-learn, pandas, numpy, seaborn, and matplotlib.

**2.Load Dataset**: Load the dataset into a pandas DataFrame to work with the data.

**3.Univariate and Bivariate Analysis**

**4.Feature Engineering**

* During the data preprocessing phase, I recognized that categorical columns such as "cpu" and "memory" etc. contained valuable information that could impact the laptop price prediction.To harness this information, I performed feature engineering by creating new features based on the distinct categories within these columns.
* One-Hot Encoding: Convert categorical variables into numerical representation using one-hot encoding.

**5.Correlation Analysis**: Checked for correlations between features using a heatmap to identify potential linear relationships with the target variable.

**6.Model Selection**: Selected multiple regression models to evaluate their performance on the given dataset. The algorithms used are Linear Ridge and Lasso Regression, K-Nearest Neighbors (KNN), Support Vector Machine (SVM), Decision Trees, Random Forest, Gradient Boosting, XGBoost, and AdaBoost."

**7.Model Evaluation**: Trained each selected model, evaluated its performanceand compared the results based on r^2 and MAE.

**8.Hyperparameter tuning**:Hyperparameter tuning was performed for Random Forest, XGBoost, and Gradient Boosting algorithms to optimize their model performance.]

**9.Voting Classifier**:A Voting Classifier was implemented by combining the Random Forest, Gradient Boosting, and XGBoost algorithms to collectively make predictions and enhance overall model performance.

10.The ultimate outcome revealed that the **Random Forest model** achieved the highest accuracy of **88.2%**

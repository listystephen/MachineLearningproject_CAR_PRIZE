# MachineLearningproject_CAR_PRIZE

**Problem Description:**

A Chinese automobile company aspires to enter the US market by setting up their manufacturing unit there and producing cars locally to give competition to their US and European counterparts. They have contracted an automobile consulting company to understand the factors on which the pricing of cars depends. Specifically, they want to understand the factors affecting the pricing of cars in the American market, since those may be very different from the Chinese market. Essentially, the company wants to know:
Which variables are significant in predicting the price of a car
How well those variables describe the price of a car
Based on various market surveys, the consulting firm has gathered a large dataset of different types of cars across the American market.

**Business Goal:**

You are required to model the price of cars with the available independent variables. It will be used by the management to understand how exactly the prices vary with the independent variables. They can accordingly manipulate the design of the cars, the business strategy etc. to meet certain price levels. Further, the model will be a good way for the management to
understand the pricing dynamics of a new market.

Dataset:  https://drive.google.com/file/d/1FHmYNLs9v0Enc-UExEMpitOFGsWvB2dP/view?usp=drive_link

**Steps performed**

1. Data Preprocessing - Data Cleaning:
- Handle missing values using appropriate imputation techniques.
- Check for and remove outliers using statistical methods.
- Address skewed data in numerical features through transformations.
2. Exploratory Data Analysis (EDA):
- Gain insights into the data distribution, relationships, and potential patterns.
- Visualizations: Histogram, Boxplot, Pair Plot, Heatmap Correlation, Pie Diagram, Bar Plot, Count Plot, Line Plot, Kernel Density Estimation (KDE).
3. Feature Engineering:
- Identify and encode categorical features using techniques like one-hot encoding or label encoding.
4. Feature Selection:
- Use algorithms like Random Forest and Select K Best to identify relevant features.
- Remove redundant or irrelevant features.
5. Split Data into Training and Testing Sets:
- Divide the dataset into training and testing subsets.
6. Feature Scaling:
- Scale numerical features if necessary to ensure uniform magnitude using techniques like Min-Max scaling or Standardization.
7. Build the ML Model: (at least 5)
- Regression: SVR, MLP Regressor, Random Forest Regressor, Linear Regression, Gradient Boost, Adaboost.
8. Model Evaluation:
- Regression Metrics: MAE, MSE, RMSE, R2 Score.
- Classification Metrics: Confusion Matrix, Accuracy, Precision, Recall, F1-Score, ROC Curve.
9. Hyperparameter Tuning:
- Optimize model performance by tuning hyperparameters.



**Model Comparison:**
                                 R-squared           MSE           MAE
Linear Regression           -3.010657e+22  7.030837e+21  5.285946e+10
Decision Tree Regressor      9.027328e-01  2.271497e-02  1.155396e-01
Random Forest Regressor      9.413123e-01  1.370543e-02  9.497274e-02
Gradient Boosting Regressor  9.318582e-01  1.591327e-02  9.950090e-02
Support Vector Regressor     7.879981e-01  4.950915e-02  1.769465e-01

Best Performing Model Based on R-squared: Random Forest Regressor

**Performance Comparison**
Random Forest Regressor: Before Hyperparameter Tuning: R-squared: 0.9413 MSE: 0.0137 MAE: 0.0949 After Hyperparameter Tuning: R-squared: 0.9212 MSE: 0.0184 MAE: 0.1068 Observations: R-squared:

Before tuning: 0.9413 After tuning: 0.9212 The R-squared slightly decreased after hyperparameter tuning. However, this change is minimal and still indicates that the model is performing very well. The performance still explains 92% of the variance in the data, which is strong. MSE:

Before tuning: 0.0137 After tuning: 0.0184 The Mean Squared Error (MSE) has increased slightly after tuning, indicating that the tuned model might have a slightly higher average squared error. However, the difference is small, and the model remains quite accurate. MAE:

Before tuning: 0.0949 After tuning: 0.1068 The Mean Absolute Error (MAE) has increased after tuning, but again, the difference is minimal. This suggests that the model still makes relatively small average errors. Conclusion: The Random Forest Regressor before hyperparameter tuning performed slightly better than the tuned model in terms of R-squared and MSE. However, the improvement after hyperparameter tuning was minimal, and the performance remains very strong. Hyperparameter tuning helped fine-tune the model for better generalization, but the overall performance difference between the two is not significant. Best Performing Model: Random Forest Regressor still remains the best performing model even after tuning, with its high R-squared value and low error metrics.



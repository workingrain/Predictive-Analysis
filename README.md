# Predictive-Analysis

#### PROPOSAL OF QUESTION
What factors contribute significantly to the variability in additional charges incurred by the patients using the random forest method based on the available data?
#### DEFINE GOAL
The research aims to uncover the variables that have a significant impact on the variability in additional charges by analyzing various factors such as demographics, medical history, and medical conditions. Identifying factors contributing to additional charges can help healthcare providers develop strategies to optimize healthcare costs effectively. 

#### EXPLANATION OF PREDICTION METHOD
Random Forest regression is an “ensemble learning method” that operates by constructing multiple decision trees during training and mean regression of the individual trees (Shafi, 2023). Each decision tree works independently and does not talk to the others. They all look at different parts of the problem and come up with their own solution. Once every decision tree has made its decision, they are gathered to see what the majority of them think. For regression, the average is taken of all their decisions. 
Expected outcomes of Random Forest are accurate predictions and feature importance. Random Forest typically produces accurate predictions because it combines the predictions of multiple decision trees. Random Forest also provides a measure of feature importance. This indicates the contribution of each feature to the model’s prediction. The result is further insight into the underlying patterns in the data and identifying important features. 
#### SUMMARY OF METHOD ASSUMPTION
Random Forest regression assumes that there is some meaningful relationship between the feature variables and the target variable that can be captured by constructing decision trees. This assumption implies that Random Forest performs best when there is sufficient variation in the input features that allows the algorithm to make accurate predictions. Therefore, it is important to carefully select and preprocess the input features to ensure they contain relevant information for predicting the target variable. 

#### ACCURACY AND MSE
Mean Squared Error (MSE) is a measure of the average squared difference between the actual values and the predicted values. In my analysis, the MSE is 24852901.37 which means that on average, the squared difference between the actual and predicted additional charges incurred by patients is approximately 24852901.37. 
Root Mean Squared Error (RMSE) is the square root of the MSE. It provides a measure of the average magnitude of the errors in the predicted values. In my analysis, the RMSE is 4985.27 which means that on average, the difference between the actual and predicted additional charges incurred by patients is approximately 4985.27.
R-Squared (R^2) is a measure of how well the independent variables explain the variability of the dependent variable. It indicates the proportion of the variance in the dependent variable that is predictable from the independent variable. In my analysis, this means that an R^2 of approximately 42.98% of the variability in additional charges incurred by patients is explained by the independent variables in the model. The low R^2 indicates that this model is not an ideal fit for the data. 
Mean Squared Error (MSE) is a measure of the average squared difference between the actual values and the predicted values. In my analysis, the MSE is 24852901.37 which means that on average, the squared difference between the actual and predicted additional charges incurred by patients is approximately 24852901.37. 
Root Mean Squared Error (RMSE) is the square root of the MSE. It provides a measure of the average magnitude of the errors in the predicted values. In my analysis, the RMSE is 4985.27 which means that on average, the difference between the actual and predicted additional charges incurred by patients is approximately 4985.27.
R-Squared (R^2) is a measure of how well the independent variables explain the variability of the dependent variable. It indicates the proportion of the variance in the dependent variable that is predictable from the independent variable. In my analysis, this means that an R^2 of approximately 42.98% of the variability in additional charges incurred by patients is explained by the independent variables in the model. The low R^2 indicates that this model is not an ideal fit for the data. 

#### LIMITATIONS
A limitation of the random forest model is the lack of interpretability of individual predictions. Since it uses ensemble decision-making, it is challenging to understand the reasoning behind each specific prediction. In exchange, random forest prediction is robust at making accurate predictions. This prediction method provides feature importance scores at the global level, but it does not offer direct insight into how each feature contributes to an individual prediction. This lack of interpretability may be a drawback in scenarios where understanding the underlying factors driving specific predictions is crucial, such as in medical domains. 
#### COURSE OF ACTION
While hyperparameter tuning improved the model’s performance, I would not recommend this model to predict additional charges incurred by patients. Further refinements are necessary to achieve better predictive accuracy. This could involve experimenting with different algorithms to capture more nuanced relationships within the data. 
Before deploying the model in a healthcare setting, it is crucial to validate its performance through prospective testing in clinical settings rigorously. Validation helps ensure the model generalizes well to unseen data and reliably predicts additional charges across diverse patient populations.
Finally, the model should be continuously monitored and evaluated for performance, fairness, and accuracy. Regular updates and refinements based on feedback from patients, healthcare staff, and stakeholders can ensure that the model remains relevant.


# Cardiovascular-Risk-Prediction
Heart disease is a major health concern globally, and accurate prediction of the risk of future heart disease is crucial in preventative healthcare. The Framingham dataset, an ongoing cardiovascular study in Massachusetts, provides valuable patient information for predicting the 10-year risk of future coronary heart disease (CHD). The dataset includes over 3,000 records and 15 potential risk factors, including demographic, behavioral, and medical risk factors.

The objective of this machine learning classification project was to predict the risk of CHD in patients using the dataset. Classification algorithms employed were: [Logistic Regression, Logistic Regression with Grid Search Cross Validation, Decision Tree, Decision Tree with Randomized Search Cross Validation, Random Forest, Random Forest with Randomized Search Cross Validation, XG Boost, XG Boost with Randomized Search Cross Validation]. Each of these models have unique strengths that can be exploited to obtain good predictive performance.

Before training and testing the algorithms, the dataset was observed to have class imbalance, where the negative class was dominant over the positive one.

It was also observed that the dataset had several null values some of which I imputed using [mean, median, mode] and some of which I dropped. The null values which were dropped were from the negative class, as the purpose of doing this was to reduce the class imbalance.

It was also observed that the dataset had several outliers as well. Some of which I imputed using the Inter Quartile Range method in which the observations which were above the upper limit which is equal to q3 + (1.5 * iqr), were replaced by the upper limit value. Where as those which were below the lower limit which is equal to q1 - (1.5 * iqr), were replaced by the lower limit value. While, some of the outliers were dropped. The outliers which were dropped were from the negative class, as the purpose of doing this was to reduce the class imbalance.

Class imbalance is a common issue in classification tasks and can lead to biased model performance. To address this issue I used two techniques: Tomek Links and SMOTE. Tomek links removes the majority obersvations that are very close to the minority ones, facilitating a smoother classification process, while Synthetic Minority Oversampling Technique (SMOTE) creates synthetic samples of the minority class to balance the dataset.

After balancing the dataset, the models were trained and tested. The cross validation parameter in Grid Search and Randomized Search was given as 5.

The evaluation metrics used were precision, F1 score, specificity, recall and accuracy.Accuracy score tells us the total accuracy of the model. Precision score tells us how many observations out of the predicted positive observations did we get right. Recall score tells us how many observations out of the actual positive observations did we get right. F1 score is the harmonic mean of precision and recall. Specificity score tells us how many observations out of the actual negative observations did we get right. .

XGBoost Randomized Search Cross Validation model was the last algorithm tested, and it outperformed the other algorithms.

The XGBoost model's performance can be attributed to its ability to handle large datasets and nonlinear relationships between the predictors and the target. The model works by creating an ensemble of decision trees and minimizing the loss function. Randomized search cross-validation was used to tune the model's hyperparameters, which led to a better-performing model.

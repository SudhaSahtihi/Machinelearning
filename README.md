# Abalone Dataset Analysis for Age Prediction
This Assignment is a part of our coursework which involves predicting the age of abalones using their physical measurements. The dataset contains eight variables, with the first seven serving as predictors and the eighth as the response. The results are averaged over 20 random splits of the data, where each split divides the data into 90% for training and 10% for testing. For each split, models are trained on the training set, and the training and test MSE (or R²) are calculated. These results are averaged across the splits and reported. Below is a summary of the results for the different models used:

a) Null Model
The null model serves as the baseline by always predicting the average training response ( ̄y). The average training and test MSE for the null model were computed over 20 random splits, providing a reference point for evaluating other models.

b) Ordinary Least Squares (OLS) Regression
OLS regression was computed analytically by solving the normal equations with a regularization parameter λ = 0.001. The average training and test R² and MSE were calculated along with their standard deviations across the splits. Additionally, the average value and standard deviation of the logarithm of the determinant of (X^T)*X + lambda*(I) were reported to understand the stability of the matrix inversion.

c) Regression Trees
Regression trees with maximum depths ranging from 1 to 7 were trained and evaluated. For each tree depth, the average training and test R² and MSE were computed. These metrics were plotted against the tree depth to visualize the trade-off between model complexity and performance. The null model MSE was also displayed as a horizontal line for comparison.

d) Random Forest Regression
Random forest regressors were trained with 10, 30, 100, and 300 trees. For each configuration, the average training and test R² and MSE were calculated along with their standard deviations. This analysis highlights the impact of increasing the number of trees on both training and test performance.

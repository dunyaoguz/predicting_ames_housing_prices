# predicting_ames_housing_prices

The objective of this exercise was to develop a model to predict the price of houses in Ames, Iowa for the [House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview/evaluation) competition on Kaggle.

- Data was cleaned thoroughly: nulls were imputed, redundant columns and outliers were dropped, wrong values were fixed, ordinal and ranked attributes were encoded as numbers.
- 70+ new features were engineered: interaction features were created for quality and condition related attributes, polynomial features were added for attributes that had the strongest correlation with the target variable, completely new features were designed.
- Multiple Linear Regression, Lasso, Ridge, Elastic Net and K Neighbours Regression models were tried. Optimal hyperparameters were found and used in the latter 4 models through Cross Validation and Grid Search.
- ANOVA and k-best feature selection were utilized, however it was seen that the more features were included, the better was the performance. Though the number of features was high, the model did not seem to suffer from overfitting.
- In the end, Multiple Linear Regression with 95% of top performing attributes had the highest predictability.
- Model built had 94.28% accuracy on the test data set and was on average ~18500 dollars off from actual prices.
- Feature engineering was the biggest component of this project. The coefficients of the resulting model prove that these efforts paid off. The features that had the biggest coefficients were nearly all engineered features!
- Predictions were submitted to Kaggle and achieved a root mean squared error of 0.14 between the logarithm of the predicted value and the logarithm of the observed sales price.

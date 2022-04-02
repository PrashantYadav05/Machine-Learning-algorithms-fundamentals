# Machine Learning algorithms fundamentals
## Understand Data with "Descriptive Statistics":
* Review the dimensions of your dataset.
* Review the data types of attributes in your data.
* Summarize the distribution of instances across classes in your dataset. `class_counts = data.groupby('class').size()`
* Summarize your data using descriptive statistics.
* Understand the relationships in your data using correlations. `correlations = data.corr(method='pearson')`
* Review the skew of the distributions of each attribute.

## Understand Data With Visualization:
* Histograms.
* Density Plots.
* Box and Whisker Plots.
* Correlation Matrix Plot.
* Scatter Plot Matrix.

## "Feature Scaling" for Machine Learning:
* Rescale data.
* Standardize data. (0,1)
* Normalize data. [0,1]
* Binarize data: All values above the threshold are marked 1 and all equal to or below are marked as 0

## "Feature Selection" for Machine Learning: 
Feature selection is a process where you automatically select those features in your data that contribute most to the prediction variable or output in which you are interested. Having irrelevant features in your data can decrease the accuracy of many models, especially linear algorithms like linear and logistic regression. Three benefits of performing feature selection before modeling your data are:
1. **Reduces Overfitting**: Less redundant data means less opportunity to make decisions based on noise.
2. **Improves Accuracy**: Less misleading data means modeling accuracy improves.
3. **Reduces Training Time**: Less data means that algorithms train faster.

* Univariate Selection. `SelectKBest`
* Recursive Feature Elimination. `RFE`
* Principle Component Analysis.
* Feature Importance.

## Evaluate the performance of Machine Learning algorithms with Resampling:
* Train and Test Sets: A downside of this technique is that it can have a high variance. This means that differences in the training and test dataset can result in meaningful differences in the estimate of accuracy.(Model learning capacity decreses)
* k-fold Cross Validation (Each sample gets included in test, Model variance of accuracy will come down, Ratio of classification data may not be maintained)
* Leave One Out Cross Validation (Model may have high variance, High computation time)
* Bootstrap or Repeated Random Test-Train Splits.
Note: Caution while applying these validation techniques in Time Series data.

## Machine Learning algorithm "Performance Metrics":
* Classification Metrics
  * Classification Accuracy.
  * Logarithmic Loss.
  * Area Under ROC Curve.
  * Confusion Matrix.
  * Classification Report.
* Regression Metrics
## Spot-Check classification algorithms

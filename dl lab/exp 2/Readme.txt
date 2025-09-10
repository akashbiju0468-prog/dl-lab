Objective of the Study

The objective of this study is to understand outlier detection in a dataset using two methods:
Z-score method (standard deviation approach)
Interquartile Range (IQR) method (statistical percentile-based approach).
Outliers are unusual values that differ significantly from the majority of the dataset and may affect the performance of data analysis or machine learning models.

Dataset Used and Description
The dataset used here is a small custom dataset:
Data
=
[10,12,13,15,20,28,29,102,90]
Data=[10,12,13,15,20,28,29,102,90]

Size: 9 values
Type: Numeric, 1-dimensional

Description: Most of the values lie between 10 and 30, but a few large values (90 and 102) seem unusual.
Goal: Detect whether these large values are outliers.
Deep Learning Method Applied
This experiment does not apply a deep learning model, since it is a basic data preprocessing step.
Instead, two statistical methods were applied for outlier detection:
Z-score method – calculates how far each point is from the mean in terms of standard deviations.
IQR method – calculates outliers based on the spread of the middle 50% of data.
These methods are often applied before training deep learning models, to clean data and improve accuracy.

Results / Output

Z-score Method:
Any value with |Z| > 1 was considered an outlier.
→ Detected outliers: [90, 102]

IQR Method:

Q1 (25th percentile) = 13
Q3 (75th percentile) = 28
IQR = Q3 – Q1 = 15
Upper Limit = 28 + 1.5 × 15 = 50.5
Lower Limit = 13 – 1.5 × 15 = -9.5
→ Detected outliers: [90, 102]
Both methods correctly identified 90 and 102 as outliers.
📊 A boxplot visualization also shows these two values as points outside the whiskers.

Conclusion

Outlier detection is essential before applying machine learning or deep learning models.
Both Z-score and IQR methods successfully detected the outliers in this dataset.
Removing such values can help improve the performance of predictive models by reducing noise and bias.
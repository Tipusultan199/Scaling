# Scaling
The choice of which normalization technique to use depends on the characteristics of your data and the requirements of your specific machine learning problem. Here are some guidelines for when to use different normalization techniques:

Normalization:
Use normalization, such as Min-Max scaling, when you want to scale your features to a specific range (e.g., between 0 and 1). This technique is useful when you have features with different scales and you want to preserve the original distribution and range of the data. Normalization is commonly used in algorithms that rely on distance calculations, such as k-nearest neighbors (KNN) or support vector machines (SVM).

Standardization:
Use standardization (z-score standardization) when you want to transform your data to have zero mean and unit variance. Standardization is useful when you have features that are normally distributed or when you want to compare different features on a similar scale. It can help in cases where your data has outliers or when you want to use algorithms that assume normally distributed data, such as linear regression or logistic regression.

Log Transformation:
Use log transformation when your data exhibits a skewed distribution, such as exponential or power-law distributions. Log transformation can help in reducing the impact of extreme values and making the data conform more closely to normality. It is commonly used in cases where the data has a wide dynamic range, such as financial data or population counts.

Robust Scaler:
Use robust scaling, such as the RobustScaler in scikit-learn, when your data contains outliers and you want to scale the data while being less affected by the outliers. Robust scaling is based on the median and interquartile range, making it more robust to extreme values. It is a good choice when you have features with a non-Gaussian distribution or when you want to reduce the influence of outliers on your models.

Max Absolute Scaler:
Use max absolute scaling when you want to scale your features based on the maximum absolute value, without shifting the data distribution. This technique can be useful when you want to preserve the sparsity of sparse data or when you have features that are already centered at zero.

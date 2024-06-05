# Metrics from the ML code

- **Accuracy**: The proportion of true results (both true positives and true negatives) among the total number of cases examined. It measures how often the classifier is correct overall.
- **Kappa**: A statistic that measures inter-rater agreement for qualitative (categorical) items. It is generally thought to be a more robust measure than simple percent agreement calculation since it takes into account the agreement occurring by chance.
- **AccuracyLower**: The lower bound of the confidence interval for accuracy. It represents the lowest value of accuracy that is consistent with the observed data, given a specified confidence level (typically 95%).
- **AccuracyUpper**: The upper bound of the confidence interval for accuracy. It represents the highest value of accuracy that is consistent with the observed data, given a specified confidence level (typically 95%).
- **AccuracyNull**: The accuracy of a naive classifier that always predicts the majority class. It serves as a baseline to compare the actual model's performance.
- **AccuracyPValue**: The p-value associated with the test of whether the model's accuracy is significantly better than the accuracy of a random classifier. A low p-value indicates that the model's accuracy is significantly better than random chance.
- **McnemarPValue**: The p-value from McNemar's test, which is used to determine if there are significant differences in the prediction performance of two classifiers on the same dataset.
- **F1**: The harmonic mean of precision and recall, providing a single metric that balances both concerns in binary classification. It is particularly useful when the class distribution is imbalanced.

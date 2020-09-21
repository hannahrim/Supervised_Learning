# Supervised_Learning
In this repository, I conducted and evaluated several machine learning models to asses loan risk. I implemented machine learning models, used resampling to address the class imbalance, and evaluated the performance of these models. 

I used three techniques to address class imbalance: oversampling, undersampling, and a combination approach. The minority class in this case is high_risk loan status with a count of 347, while high risk count was 68470. 

By randomly oversampling the data, I calculated a balanced accuracy score of .67. This model resulted in a precision rate of .01, a recall rate of .74, and precision score (f1) of .02. I then conducted a SMOTE oversampling test. The metrics of the minority class using a SMOTE oversampling model resulted in an accuracy score of .66 with the same precision rate, a recall rate of .63, and a f1 rate of .02. The SMOTE test was even worse than random oversampling at calculating loan risk.

I then conducted an undersampling cluster centroid test. This resulted in an accuracy score of .55 with a precision score of .01, a recall rate of .68, and a f1 score of .01. The undersampling test is not an accurate way to predict loan risk.

When using a combination method of both undersampling and oversampling, it resulted in an accuracy score of .64. I found that resampling with SMOTEENN did not work miracles, but some of the metrics show an improvement over undersampling.

The model that performed the best was random oversampling. Because the F1 score is closer to 0, a random oversampling test is not the best method to determine accuracy on this dataset. In the future, I would try to use another model for this dataset.

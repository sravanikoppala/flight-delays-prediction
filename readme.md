# Predicting Flight Delays

Using different classifiers and selecting the best one in predicting the departure delay of a flight in USA by using the origin, flight carrier, date and time information.

## Project discussion:
Using a dataset from Kaggle which has 100,000 records on flight data has an output column of whether a flight is delayed by 15 minutes (Yes or No). 
This is chosen for the output having binary classes (Delayed by 15mins? Yes or No). It has various attributes like flight carrier, origin, destination, distance, departure time, month, day of week and day of month. Here, different types of classifiers are used and prediction accuracy is compared for various methods using various training sizes ranging from 10% to 50%. At the end the highest accuracy model is selected for the prediction. Various data visualizations are also done for the analysis of data.

## Hypothesis outline:
The maximum number of flight delays should occur during the holiday season and at the busiest airports.

## What were the outcomes?
It was observed that SVM gave the highest accuracy for PCA n=2 reduced data. But, SVM takes a lot of time like atleast 20 mins to run my dataset. Most of the classifiers except KNN performed well and gave around 80-81% accuracy. KNN may have not performed well in the initial stages because of less training sizes as it needs similar data to get trained, thus by increasing the training size, it performed better. The random forest classifier also had an increasing curve for the accuracy where as other classifiers didn’t give a smooth curve when the training sizes increased. It can be inferred that as the training size is increasing the data can get overfitted in these models. 
The important thing noticed here is that PCA reduced data has a high variance of about 98% and when this data is fed into the classifiers, it performed almost equally well compared to the original data. It can be inferred that for high number of dimensions, if I reduce the dataset’s components to 2 or 3 using PCA, it still performs well. This is very helpful in reducing the training time and avoiding overfitting with irrelevant features. This is a boon to save time!
I can conclude that if you have time and need more accuracy, SVM can be used to get a stable classification, but it gets overfitted for high training sizes which must be kept in mind. If small amounts of data, Logistic regression can be used as this dataset has binary classes as it is simple, easy and quick. Naïve Bayes classifier can be used for PCA reduced data. Depending on the features and the size of the dataset, classifier has to be chosen.
And, from the data visualizations, I can infer that the holiday season in December and July have the highest number of delays as stated in the hypothesis. Hypothesis has been proven right. Also, as Friday is the time when more passengers fly, even that day has highest number of delays. Another factor observed was the more the number of flights per carrier, more they have delays and vice versa. The delays are directly proportional to the number of flights per carrier. Finally, using heatmaps it can be seen that East Coast has the highest number of airports with highest number of flights flying from each airport.
This project has been very interesting and engaging to me. I have learnt mainly how to do the data analysis. I had lots of fun trying to visualize data assuming different circumstances and playing around with data. Starting from scratch, without knowing before the class started, now I understand a lot about data science and data analysis.

### Note: Please refer the Project report for more details.


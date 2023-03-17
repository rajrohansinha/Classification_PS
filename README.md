# Classification_PS
Problem statement - Predicting if income exceeds 50,000 per year based on 1994 US Census Data with Simple Classification Techniques.

Insights found -

1.People of the age group of 20 to 50 were the majority of the people who participated in the survey.
People who earn >50k are moreover of age 40 to 50 years & those who earn <50k are moreover of age 20 to 35 years.

2.we can see that there is almost double the sample size of males in comparison to females in the dataset. 
The percentage of males who make greater than 50,000 is much greater than the percentage of females that 
make the same amount. This will certainly be a significant factor considered as an important in our prediction model.

3.majority of the individuals work in the private sector.Federal government is seen as the most elite
in the public sector, which most likely explains the higher chance of earning more than 50,000.

4.For the most part, a higher level of education is correlated to a higher percentage of
individuals with the label >50k. One interesting statistic to note is the ratio of 
individuals labeled >50k to <=50k is almost the same between those that have a doctorate and those that
went to a professional school.

5.Since we want to Predict if income exceeds 50,000 per year so in this case we can focus on "RECALL" 
as a metric of our model because in our problem we want to predict as many actual positive we can. 
Since misclassification of any person who actually earns more than 50,000 might loose the essence 
of the entire survey if the model starts predicting that person's income as less than 50,000.

The positive drivers towards predicting if income exceeds 50,000 for any survey taker are as follows -

This was identified using SHAP.
Marital_status , young age survey takers , occupation , Higher/Lower education degree, working hours of that person , gender of that person ,if he is an own child.

Question - Assess the performance of your models using appropriate metrics. Discuss which model is best and why.

Answer - Since we want to Predict if income exceeds 50,000 per year so in this case we can focus on "RECALL" as a metric of our model because in our problem we want to predict as many actual positive we can. Since misclassification of any person who actually earns more than 50,000 might loose the essence of the entire survey if the model starts predicting that person's income as less than 50,000.

Hence as per my understanding & analysis taking RECALL as a final metric might work & definitely gradient boosting gives us the highest recall score with lowest false negative value in the confusion matrix so it needs to be optimized further for better results.

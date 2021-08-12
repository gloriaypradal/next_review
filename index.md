## Predicting Next Review Sentiment

The following project is based on the sentiment analysis of reviews of more than 19000 clients of a clothes store, these reviews have corresponding ratings according to the client experience, and the goal of the following work is based on these reviews, to build a model to predict sentiment of the next review, and check if this model can be used with reviews of other line of business. The clothes store review is also classified by product and department, this time graph analysis was done over some of the variables giving us as a general result that the store has more positive reviews than negative, Vader from the NLTK library was used to determine sentiment of the reviews, these results were translated to positive, negative and neutral results, and used as labels to build a naïve bayes model to classify and predict probability of the sentiment of the next review



### EDA

the data set was read and transform to a data frame were the reviews were under the “ reviews”  column, following this, missing values were check, finding around 2000 missing reviews, these observations were dropped, ending with a data frame of 19662 rows. Graph analysis was done for some of the variables:

![image](https://user-images.githubusercontent.com/58094203/129120932-13d2f6d4-d36b-4e29-ad6a-e71c1073edf8.png)

From this histogram of our target variables, we can see a skewed distribution showing that this store have more positive reviews than negative

Following the number of reviews by department, division and class name


![image](https://user-images.githubusercontent.com/58094203/129120978-fb95b3c6-fcca-42d8-9c86-4beff0235e54.png)

![image](https://user-images.githubusercontent.com/58094203/129120989-f278a126-e236-42e4-94cd-0a24cd256ac9.png)


![image](https://user-images.githubusercontent.com/58094203/129120996-4dc9cdf3-6bd9-4358-bc72-548aa5a273bd.png)


### Correlation

![image](https://user-images.githubusercontent.com/58094203/129121029-f5ad0327-b756-4176-9772-06014328659c.png)



### Sentiment Analysis Results

![image](https://user-images.githubusercontent.com/58094203/129121063-6e314811-1560-43fc-9c71-391311f1eb74.png)

![image](https://user-images.githubusercontent.com/58094203/129121069-70d0dcdb-c393-4f74-93cb-d7fc00b963e7.png)


![image](https://user-images.githubusercontent.com/58094203/129121079-605de22d-ca00-48e7-8740-1c2290733bbf.png)


Accuracy of Naive Bayes classifier = 91.78 %

### Author
 GLoria Moore
 
### References
 
 [1] Kepple. E (2020). Simple Sentiment Analysis for NLP Beginners and Everyone Else using VADER and TextBlob. Retrieved August 07, 2021. from https://www.watermelonwebworks.com/google-analytics-users-vs-sessions-vs-pageviews/ 
[2] MOnkeyLearn. Sentiment Analysis: A Definitive Guide. Retrieve on August 03, 2021 from: Sentiment Analysis: The Go-To Guide (monkeylearn.com)
https://www.kaggle.com/nicapotato/womens-ecommerce-clothing-reviews 
https://towardsdatascience.com/a-beginners-guide-to-sentiment-analysis-in-python-95e354ea84f6  
https://medium.com/swlh/simple-sentiment-analysis-for-nlp-beginners-and-everyone-else-using-vader-and-textblob-728da3dbe33d 
https://www.kaggle.com/andrewmvd/trip-advisor-hotel-reviews 
https://www.kaggle.com/therohk/million-headlines 
https://www.kaggle.com/sid321axn/amazon-alexa-reviews 


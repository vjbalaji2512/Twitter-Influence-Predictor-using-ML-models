# Twitter Influence Predictor using ML models

### OBJECTIVE
Our project aims to determine the top k predictors of social influence from a given Twitter [dataset](https://www.kaggle.com/competitions/predict-who-is-more-influential-in-a-social-network/data). Using the top k predictors, the most influential person for each data point is predicted. Each data point describes two individuals A and B. The discrete target label - choice represents a human judgment about which one of the two individuals is
more influential. This binary label choice has a label ’1’ if A is more influential than B and a label ‘0’ if B is more influential than A. As a further extension, we also hope to find the association between the predicted features to help us understand how the given feature influences the popularity of the person using clustering and data visualization.


### DATASET

The Twitter dataset that we have chosen was provided
by PeerIndex in the year 2013. The dataset consists of a standard, pair-wise preference learning task [1]. Each data point describes two individuals A and B. For each person, there are 11 pre-computed, non-negative numeric features based on Twitter activity provided, which include:

• # followers: Number of followers of the person on Twitter <br>
• # followings: 1. Number of Twitter users the person follows <br>
• # listed: Number of people that have added the person to a list <br>
• # mentions received: Number of times people have mentioned (@) the person <br>
• # retweets received: Number of times a tweet was retweeted <br>
• # mentions sent: Number of times the person mentioned (@) someone <br>
• # retweets sent: Number of times the person retweet a tweet <br>
• # posts: Number of posts <br>
• # network feature 1, 2, 3: Local follower networks of the person <br>

### ML MODELS:
● Four machine learning models, namely Logistic Regression, Random Forest, K-Nearest Neighbours, and XGBoost were implemented using Python on the training set.

### KEY PREDICTORS:
● The top predictors of social influence are identified as follows: A/B_listed_count, A/B_follower_count, A/B_network_feature_3, A/B_retweets_received, and A/B_network_feature_2.

## ANALYSIS 

![image](https://github.com/vjbalaji2512/Predicting-Influencers-using-ML-Models/assets/124394195/77b12250-bd87-42c6-8d5d-baa28ed6411f)

![image](https://github.com/vjbalaji2512/Predicting-Influencers-using-ML-Models/assets/124394195/46be190c-d8a1-4b88-a78d-cbf72f31027d)

![image](https://github.com/vjbalaji2512/Predicting-Influencers-using-ML-Models/assets/124394195/2a76c6d8-f231-4f7e-847c-9b46b6e71f1f)

![image](https://github.com/vjbalaji2512/Predicting-Influencers-using-ML-Models/assets/124394195/37175fef-cb06-4628-9959-9f3d9d6fed8f)

![image](https://github.com/vjbalaji2512/Predicting-Influencers-using-ML-Models/assets/124394195/ffcaad8f-0aed-4498-a650-da423c66da98)

### CONCLUSION

We can see that the XGBoost Classifier gives us maximum testing accuracy of 78.6% compared to other classifiers. We can extend this work by improving the accuracy by using the Deep Learning algorithm which can give us better insights into the features that contribute
to finding the most influencing account on Twitter. If known, network_feature_1, network_feature_2, network_feature_3 could lead to better results. The combination of features can be used as a feature to improve the results. From the results of checking the influencing accounts, we can tell that most of the accounts that used this hashtag are news channels’ official Twitter accounts. It is safe to say that news channels influence people’s daily life in many ways and this is one such situation. 

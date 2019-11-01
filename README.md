# Board-game-rating-prediction
Predicting Board Game rating using Linaer Regression Model and Random Forest Classifier.
The dataset used is games.csv.It has been imported from : https://github.com/ThaWeatherman/scrapers/tree/master/boardgamegeek<br>
A total of 20 columns exist in the dataset namely :
'id', 'type', 'name', 'yearpublished', 'minplayers', 'maxplayers','playingtime', 'minplaytime', 'maxplaytime', 'minage', 'users_rated', 'average_rating', 'bayes_average_rating', 'total_owners', 'total_traders', 'total_wanters', 'total_wishers', 'total_comments', 'total_weights', 'average_weight'<br>
Out of this samples having 0 user rating has been removed. Also samples having missing values has been removed.<br>
The columns 'id','name','type' have been removed as they have no corelation with rating.
The columns 'average_rating' and 'bayes_average_rating' have been removed as they are what we want to predict.
<br>
After this we split the data into training and testing set.<br>
After this the modela(Linear Regression,Random Forest Classifier) was trained on the training data and the predictions were made on the testing data.
Following MSE(mean squared error) score was obtained.(Results might slightly vary on different runs.)<br>
1. Linear Regression: 2.078819032629326
2. Random Forest Classifier: 1.4458560046071653

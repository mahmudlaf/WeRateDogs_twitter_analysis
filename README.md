# WeRateDogs Exploration

## Dataset

The dataset (twitter_archive_enhanced) contains about 5000 tweet archive of Twitter user of WeRateDogs. It is a Twitter account 
that rates people’s dog by making some comments. Most of the ratings have denominator 
of 10. The images in the dataset were ran in an image prediction neural network and a new 
dataset was generated from [here](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv) 
A third dataset was assessed through Twitters’ API.


## Summary of Findings

Most tweets of the tweets analyzed were from iPhone (about 98%). A few are from Web 
Client (about 1%) while very few are from TweetDeck (less than 1%).

Dogs were rated on a scale of 10, although may be greater than 10. This depends on 
impressive people rating the dogs are. About 76% of the dogs were rated between 10 and 13. 
However, more than 50% of the total ratings were above 10 and few were above 100.

111 breeds of dogs were predicted by the image prediction neural network. Top 10 breeds 
were analyzed and Labrador Retriever top the list.

Out of 913 names of dogs in the dataset, Cooper, Lucy and Oliver are the top common 
names of dogs. Other name in the list of top 10 are: Penny, Tucker, Winston, Sadie, Toby, 
Lola and Daisy.

The number of tweets in 2015 was high, about 30% of the total tweets analyzed. This trend, 
however, reduced drastically after 2015. The trend was almost uniform between 2016 and 
2017 but later reduced further. 


## Key Insights

Three sources were used to garther data;
1. A CSV file (twitter_archive_enhanced.csv) was downloaded and imported into dataframe.
2. Request library of pandas was used to download the tweet image prediction as 
image_predictions.tsv. this was also imported into a dataframe.
3. Pandas Tweepy was used to query data via Twitter API as tweet.json.txt. This was also 
imported into a dataframe.

The Dataset was assessed visually and programatically for quality and tidiness issues.
The dataset was then cleaned and saved in a csv file named twitter_archive_master.csv

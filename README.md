# NLP on Tweets to forecast fluctuations in the Nasdaq index

The objective of this project was to forecast fluctuations on a daily basis in the Nasdaq Index using Natural Language processing on Twitter data.

The data was obtained with Octoparse, which was programed to collect tweets from the profiles of Barack Obama, Donald Trump, Elon Musk, Hilary Clinton, The Economist, Bloomberg Economics and Bill Gates, between 04/01/2020 to 10/01/2020. 

To perform the analysis, Bag of Words was used. This way of extracting features consists in creating a vector which contains the frequencies of each word that they appear on the sentence. Thus, only the word frequencies matter, not the order that the word appear in the sentence. To improve the analysis, different minimum frequencies were tested, to avoid words with no relevance. 

Because of this approach, the tweets from the same day were merged in one text. In this way we can label less data and join all the "daily information".

As classifier, Complement Naive Bayes was used. 

The best forecast, 76% accuracy, was achieved after spliting the data to obtain a dataset with balanced classes. 

This means that the classifier can predict with 76% accuracy if the Nasdaq Index will increase or decrease in the next day just by reading the tweets from the day before.

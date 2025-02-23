Sentiment analysis of app reviews is an important aspect in understanding user perception of a product. In this research, sentiment analysis of app reviews obtained through scraping using the `google_play_scraper` library is performed. The initial dataset contains 50,000 rows of data which then undergoes a series of preprocessing stages, including duplicate removal, text cleaning (removing emoticons, numbers, and symbols), case folding, normalization using a slag dictionary, tokenization, stopword removal, and stemming using Sastrawi. In addition, data visualization is done using WordCloud before and after preprocessing to see the distribution of words in user reviews.

The labeling process is done automatically using InSet (Indonesia Sentiment Lexicon), which allows each review to be classified as positive or negative based on the sentiment score of the words contained in it. After that, feature extraction is performed using two popular techniques, namely Bag of Words (BoW) and Term Frequency-Inverse Document Frequency (TF-IDF).

For modeling, the Logistic Regression algorithm is used, which is one of the lightweight and effective classification models for text analysis. The evaluation results showed that the model with BoW achieved an accuracy of 85.48%, while the model with TF-IDF had a slightly higher accuracy of 85.93%. Further analysis using confusion matrix shows that the model with TF-IDF is able to reduce the number of False Positives, thus providing better classification results compared to BoW.

The results of this study show that the TF-IDF method is superior to BoW in sentiment analysis of app reviews. In the future, this research can be developed by trying other classification models such as SVM or Neural Networks, as well as improving the quality of preprocessing to produce a more accurate model.

[Slag dict](https://www.kaggle.com/datasets/fornigulo/kamus-slag)\
[InSet (Indonesia Sentiment Lexicon)](https://github.com/fajri91/InSet)

# **Sentiment Analysis of GetContact App Reviews Using NLP**

## **About the Project**
This project performs a sentiment analysis on user reviews of the GetContact application from the Google Play Store. By leveraging Natural Language Processing (NLP) techniques, this project aims to automatically understand user perception and sentiment (positive or negative) to gain valuable insights for product development.

## **Objectives**
* To collect review data for the GetContact application from the Google Play Store.
* To clean and prepare the text data through a series of preprocessing stages.
* To automatically label the sentiment (positive/negative) of each review using a lexicon.
* To build and train a classification model to predict review sentiment.
* To compare the performance of two popular feature extraction methods: **Bag of Words (BoW)** and **TF-IDF**.

## **Dataset**
The dataset consists of **50,000 user reviews** of the GetContact application, collected from the Google Play Store through a scraping process. The sentiment labels for the training data were automatically generated using the **InSet (Indonesia Sentiment Lexicon)**.

## **Tools & Libraries**
* **google_play_scraper:** For scraping review data.
* **Pandas:** For data manipulation and analysis.
* **Sastrawi:** For the Indonesian language stemming process.
* **Scikit-learn:** For feature extraction (BoW & TF-IDF), modeling (Logistic Regression), and evaluation.
* **WordCloud:** For visualizing word distribution.
* **Matplotlib & Seaborn:** For data visualization.

## **Methodology**
The analysis was conducted through several main stages:
1.  **Data Collection:** Scraping 50,000 reviews from the Google Play Store.
2.  **Data Preprocessing:**
    - Removing duplicates.
    - Cleaning text from emojis, numbers, and symbols.
    - Case Folding (converting text to lowercase).
    - Normalization (correcting non-standard/slang words).
    - Tokenization (splitting sentences into words).
    - Stopword Removal (removing common words).
    - Stemming (reducing words to their base form).
3.  **Automatic Labeling:** Determining the sentiment score of each review using **InSet**.
4.  **Feature Extraction:** Converting text into numerical data using **Bag of Words (BoW)** and **TF-IDF**.
5.  **Modeling:** Training a **Logistic Regression** classification model.
6.  **Evaluation:** Measuring model performance using accuracy and a *Confusion Matrix*.

## **Results**
* The model using **Bag of Words (BoW)** achieved an accuracy of **85.48%**.
* The model using **TF-IDF** achieved a slightly higher accuracy of **85.93%**.
* Based on the *Confusion Matrix* analysis, the **TF-IDF** model proved to be better at reducing the number of *False Positives*, making it a more reliable model.

## **Conclusion**
The **TF-IDF** feature extraction method demonstrated superior performance compared to **Bag of Words (BoW)** for the sentiment analysis of GetContact app reviews. This research successfully proves that the NLP approach is effective for classifying sentiment and can provide deep insights into user perception of an application.

## **Sources**
* **Slang Word Dictionary:** https://www.kaggle.com/datasets/fornigulo/kamus-slag
* **InSet (Indonesia Sentiment Lexicon):** https://github.com/fajri91/InSet

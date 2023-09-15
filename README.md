# Apple and Google NLP Twitter Sentiment Analysis
<img src="image\Untitled-3.png"/>

# Table of contents
1. [Business Understanding](#Business Understanding)
2. [Data Understanding](#Data Understanding)
3. [Data preparation](#Data preparation)
4. [Modeling](#Modeling)
5. [Evaluation](#Evaluation)

-----
## Business understanding
## Introduction
Apple and Google are two of the most prominent companies in the tech industry, producing a wide range of products that have a significant impact on people's lives. Monitoring the sentiment expressed by Twitter users towards these companies and their products can help businesses make informed decisions. This sentiment analysis can inform product development, marketing strategies, and customer relations.
## Business Problem
The primary business problem that will be addressed is the need for a systematic and automated way to gauge the sentiment of tweets related to Apple and Google products. Twitter is a platform where millions of users express their opinions and experiences daily. Manual analysis of these tweets is not feasible due to the sheer volume of data. Therefore, there's need for a reliable NLP model that can classify tweets into positive, negative, or neutral sentiment categories.

## Research Question
* How do consumers perceive one company relative to the other?

## Main Objective
The main objective of this project is to build a proof-of-concept NLP model that can accurately rate the sentiment of tweets about Apple and Google products. This model will enable businesses to gain real-time insights into how their products are perceived by the Twitter community.

## Specific Objectives
* **Data Collection:** A dataset of tweets related to Apple and Google products will be gathered. This dataset should include tweets that express both positive and negative sentiments.

* **Data Preprocessing:** Cleaning and preprocessing the collected data to prepare it for NLP analysis. This includes tasks like text normalization, tokenization, and handling of missing or irrelevant data.

* **Model Development:** Developing a baseline NLP model for binary sentiment classification, categorizing tweets as either positive or negative. This model will serve as a starting point for further improvements.

* **Model Evaluation:** Evaluating the binary sentiment classifier using appropriate metrics like accuracy, precision, recall, and F1-score. This will help assess the model's performance and identify areas for improvement.

* **Multiclass Classification:** Extending the binary classifier to a multiclass classifier by incorporating a neutral sentiment category. This will provide a more nuanced understanding of sentiment.

* **Business Insights:** Interpret the results and provide actionable insights to businesses.

## Data Understanding
The data was sourced from [here](https://data.world/crowdflower/brands-and-product-emotions). Contributors evaluated tweets about multiple brands and products. The crowd was asked if the tweet expressed positive, negative, or no emotion towards a brand and/or product. If some emotion was expressed they were also asked to say which brand or product was the target of that emotion.

-----
## 3. Data preparation
Within our data preparation phase, we performed the following tasks:
* Clean Data
* Checking Duplicates
* Dealt with missing values

-----
## 4. EDA
The following analysis was performed on the data:
* Analysis of keywords in positive tweets.
<img src='image\output 1.png'/>
* Analysis of keywords in negative tweets.
<img src="image/output 2.png"/>
* Distribution of sentiments in Apple-related tweets.
<img src="image/output 3.png"/>
* Distribution of sentiments in Google-related tweets.
<img src="image/output 4.png"/>

-----
## 5. Modeling & Evaluation
The models include;
* Logistic Regression model.
* Naive Bayes Classifier (NB).
* Random Forest Classifier.

Binary classification to predict whether a tweet falls under the "Positive" or "Negative" category was done.  multiclass classification, where the "Neutral" category will be introduced, expanding the classification task into a three-way categorization.
* Binary classification: Hyperparameter-tuned Multinomial Naive Bayes classifier exhibited enhabced 0.87 accuracy score, precision (89.76%) and recall (79%) for negative sentiments.
<img src="image/output 5.png"/>

* Multiclass classification: The untuned Random Forest classifier displayed the highest precision (66.27%) and exhibited promising results.
<img src="image/output 6.png"/>

-----
## 6. Conclusions
* Both Apple and Google enjoy predominantly positive sentiments on Twitter, indicating strong brand perception.
* Key positive topics for Apple include retail stores, product launches, and community engagement. Negative sentiments often relate to app and autocorrect issues.
* For Google, positive discussions center around Google+, mapping services, and mobile apps. Negative sentiments occasionally touch upon Google Maps and location-based services.

-----
## 7. Recommendations
* Capitalize on the overwhelmingly positive sentiment around your brand and products. Highlight successful product launches, engage with the community, and promote events.

* Pay close attention to common pain points mentioned in negative tweets. Continuously improve app functionality, battery performance, iPad's design, and autocorrect features for Apple. For Google, address concerns related to mapping services and location-based features.

* Emphasize innovation in your product offerings, as this generates positive discussions. Encourage excitement around new features and updates.

* For both companies, maintain a strong presence on social platforms like Google+ and actively engage with users to foster positive sentiment.
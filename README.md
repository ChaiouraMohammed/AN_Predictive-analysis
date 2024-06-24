# AN_Predictive-analysis
 Sentiment Analysis and Product Trend Analysis

## Predictive analysis 
Predictive analysis is a method derived from statistics, knowledge extraction from data and game theory, analyzing present and past facts to make predictive hypotheses.

![download](https://github.com/ChaiouraMohammed/AN_Predictive-analysis/assets/91562298/16b546eb-7f9a-4ee0-af1a-231774b1c751)


## Data visualization 
Data visualization transforms complex data into accessible representations that enhance understanding. It enables management teams to integrate a message and act quickly when making decisions.

## Technologies 
### Sentiment analysis
Sentiment analysis is the process of analyzing digital text to determine whether the emotional tone of the message is positive, negative or neutral. Today, companies have large volumes of textual data at their disposal, such as e-mails, transcripts of conversations with customer support, comments on social networks and reviews. Sentiment analysis tools can analyze this text to automatically determine the author's attitude towards a subject. Companies use sentiment analysis information to improve customer service and enhance brand reputation. 
## Why sentiment analysis ?
L'analyse des sentiments, également connue sous le nom d'exploration d'opinion, est un outil important d'informatique décisionnelle qui aide les entreprises à améliorer leurs produits et leurs services. Nous présentons ci-dessous certains avantages de l'analyse des sentiments.

## Results and Outcomes 
![image](https://github.com/ChaiouraMohammed/AN_Predictive-analysis/assets/91562298/f4315ea9-60ba-4cb8-b94e-5425b99e86ba)

## Data visualized 
![image](https://github.com/ChaiouraMohammed/AN_Predictive-analysis/assets/91562298/e6e71af0-9112-41c2-b720-3d9a3ee47d92)

![image](https://github.com/ChaiouraMohammed/AN_Predictive-analysis/assets/91562298/be985550-9bba-4972-8801-4b8c32c5f023)

![image](https://github.com/ChaiouraMohammed/AN_Predictive-analysis/assets/91562298/c6ce8ca9-8bca-43e2-9e90-012a21eebdc8)

## Columns 
```
Index(['Product Name', 'Price', 'Rating', 'Reviews', 'Review Votes'], dtype='object')
```
## Function for extracting feedbacks 
```
def get_sentiment_vader(review):
    scores = analyzer.polarity_scores(review)
    if scores['compound'] > 0.05:
        return 'Positive'
    elif scores['compound'] < -0.05:
        return 'Negative'
    else:
        return 'Neutral'
```
This function get_sentiment_vader(review) takes a text review as input, uses VADER to analyze the sentiment of the review, and returns a sentiment label ('Positive', 'Negative', or 'Neutral') based on the sentiment score calculated by VADER.






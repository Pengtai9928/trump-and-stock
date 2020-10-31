# trump-and-stock

BT4222 Group Project

## 30/10/2020
- verified EST dates, no chance to the raw data
- added IXIC ticker
- merged sentiment analysis code with the rest of the preprocessing file
- added EDA; will continue to work on it over the weekends
- removed old preprocessed files
- the latest preprocessed file is `tweets&sentiments&logreturns.csv`. Please import this file and use it as the start point for subsequent NLP/ML tasks

## 27/10/2020
- fixed csv parsing issue in row 4629 (thx Yu De!)
- merged preprocessing codes from multiple sources into a single file
- modified `text_processing()`: added input arguments `remove_numbers`, `remove_handles`, `remove hashtags` and `additional_stopwords`; changed `keep_stopwords` to an input argument
    * LDA: `lower` and `remove_punctuations` should be set to `True`
    * sentiment analysis: consider setting `lower` and `remove_punctuations` to `False` (esp. using algorithms such as VADER), as they play a role in determining the sentiment of a tweet
    * added "RT" to the list of additional_stopwords as this simply indicates retweet
- extracted meta information from the tweets as additional features for EDA and prediction
    * Word Count
    * Character Count
    * Average Word Density
    * Punctuation Frequency
    * Upper Case Frequency
# trump-and-stock

BT4222 Group Project

## 27/10/2020 (Ziyue)
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
<br>
**the new preprocessed file is at `data/tweets&logreturns.csv`. This overwrites the original file of the same name. Please import this file and use it as the start point for subsequent NLP/ML tasks.**

# trump-and-stock

This project explores possible implementations of text mining such as topic modelling and sentiment analysis on President Donald Trump’s tweets to predict the impact on various indices of the US stock market such as S&P 500, DJIA and VIX. This repository contains the back-end code, data, and the results for the analysis. 


<br>

[![Screenshot-2020-12-21-at-4-35-09-PM.png](https://i.postimg.cc/PqRKcK3Q/Screenshot-2020-12-21-at-4-35-09-PM.png)](https://postimg.cc/t1FhndHs)

</br>


# Directories in this repository

This Repository includes 4 directories: "code", "data", "model", and "plots". 

## Code

-   Coherence score search.ipynb: Code of coherence score search of the degree of semantic similarity of a topic
- EDA.ipynb: Include the exploratory data analysis codes and results
- data preprocessing (final test set).ipynb: Code for data preprocessing on the final test set, comprising 1-month of tweets data from 1 Oct to 31 Oct
- data preprocessing.ipynb: Code for data preprocessing on the training data set from 2016 Jan to 2020 Sep.
- final_model_dnn.ipynb: Code for dnn model prediction
- final_model_xgboost.ipynb: Code for XGBoost model with prediction results
- final_model_dnn_tuning.ipynb: Code of model tuning with dnn model
-  word embedding.ipynb: Code of generating word2vec word embedding data
## Data

This folder contains mainly the data used in the modelling and prediction. It includes the raw data, pre-processed data, and the test data used for prediction in .csv format.
-   Folder of Coherence Model: contains the test tuning for coherence score
- EDA_Sweetviz_report.html: Exploratory Data Analysis’s Sweetvis report generated
- FinalTest_tweets&sentiment&absoluteprices.csv
-  FinalTest_tweets&sentiment&logreturns.csv
-  RAW_trump_tweets_20160101_20200930.csv
-  RAW_trump_tweets_20201001_20201031.csv
- aggregated_metadata_sentiment_frequency_by_topics.csv
- test_data_tweets&sentiment&topic&absoluteprices.csv
- test_grouped_by_day.csv
- train_validation_grouped_by_day.csv
- tweets&logreturns&topic.csv
- tweets&sentiment&absoluteprices&topics.csv
-  tweets&sentiment&absoluteprices.csv
-  tweets&sentiment&logreturns.csv
    
## Model
-  XGBoost folder: Contains pickle file that includes the loss figures
- Word2Vec folder: Contains the .csv files for Word2Vec train and test data and results
## Plots
- Feature 1,2,3 folder: Contains the plots for SHAP analysis, feature importance results, and correlation plots for the 3 different feature sets
- RMSE_MAPE_prediction.png
- RMSE_MAPE_training.png
- XGBoost_validation_test_MAPE.png
- XGBoost_validation_test_RMSE.png
- time_series_prediction.png

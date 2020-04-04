
# Financial News Sentiment Trading Strategy using FinBERT
## Background
This Project is a part of Data Science 4 All(DS4A) Women's Summit 2020, sponsored by Correlation One https://www.correlation-one.com/ds4a . Poject owners are five summit participants: __Anastasia Tatarenko, Daria Yurova , Ningyuan Zhang, Yang Su and Rohini Shimpatwar__.
The project aims to answer three questions: 
1. Which NLP model is the best for sentiment factor extraction on financial news? 
2. Does the news sentiment factor help predict stock returns? 
3. Does this strategy beat other benchmark trading strategies, e.g. buying the market portfolio?

## Dataset
1. ‘US Financial News Articles’ from Kaggle: https://www.kaggle.com/jeet2016/us-financial-news-articles
2. S&P 500 companies and industries from Wikipedia: https://en.wikipedia.org/wiki/List_of_S%26P_500_companies
3. S&P 500 daily stock prices from Yahoo Finance:

## Project Logic

1. __Data Cleaning & Labelling__<br />
  1) reformat and clean the news we get from kaggle website  <br />
  2) put industry and company labels on all news(~40,000)  <br />
  3) manually label sentiments for a small sample of news(800)
2. __EDA & Data Preprocessing__ <br /> 
  Analyze word counts, top insutries mentioned in news, top n-grams by industries and sentiment.
3. __News Sentiment Factor Extracion using Vader/FinBERT models(NLP)__  <br />
  1) use rule-based model Vader to directly predict sentiments for all news, achieve ~0.56 accuracy on labeled samples  <br />
  2) trained a FinBERT model on labeled samples by conducting trasfer learning on BERT model, achieve ~0.65 accuracy on validation set and ~0.81 on overall labeled dataset.
4. __Factor Model Based Trading Strategy__ <br />

## Poster
![Test Image 1](https://github.com/rohinishimpatwar/The-NLP-News-Sentiment-Trading-Strategy/blob/master/Images/DS4A_NLP_POSTER.png)

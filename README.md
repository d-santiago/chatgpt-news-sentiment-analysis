# Chat GPT News Headline Sentiment Analysis (2023)

The goal of this project goal is to analyze how the news media's sentiment regarding ChatGPT has evolved over a 5-month period from its release on Novermber 30th, 2022 to April 30th, 2023. Specifically, this project will analyze how the sentiment of these headlines have changed over time since its launch and the breakdown of article sentiments (positive, neutral, negative) across each media outlet that has published articles about ChatGPT.

## Technologies
- Python
- Google News API
- Apache Kafka
- Apache Spark
- TextBlob
- MongoDB

## Project Data Pipeline

- Fetched ChatGPT related news articles for each day of the 5-month period using the Google News API.
- Published each daily batch of articles to Apache Kafka for data ingestion.
- Retrieved the data stream from Apache Kafka and converted it into an Apache Spark Structured Streaming dataframe.
- Performed sentiment analysis on the dataframe using TextBlob to categorize article sentiment.
- Stored categorized articles in the output storage sink, MongoDB.
- Created data visualizations using MongoDB Atlas.

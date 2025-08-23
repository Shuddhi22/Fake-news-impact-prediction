# Fake-news-impact-prediction
Fake News Impact Score Prediction using ML. Generates synthetic data with social media metrics, sentiment &amp; source reliability. Applies regression models (Linear, SVR, Gradient Boosting) with EDA &amp; benchmarking to predict article impact.

| Column Name             | Type             | Description                                                                                                                                                                     |
| ----------------------- | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **article\_id**         | Integer          | Unique identifier for each article.                                                                                                                                             |
| **title\_length**       | Integer          | Number of characters in the article title/headline. Longer titles may indicate sensationalism.                                                                                  |
| **text\_length**        | Integer          | Number of characters in the full article body. Helps capture verbosity/detail.                                                                                                  |
| **num\_shares**         | Integer          | Number of times the article was shared on social media.                                                                                                                         |
| **num\_likes**          | Integer          | Number of likes the article received on social media platforms.                                                                                                                 |
| **num\_comments**       | Integer          | Number of user comments the article generated.                                                                                                                                  |
| **sentiment\_score**    | Float (-1 to +1) | Sentiment polarity of the article text: **-1 = very negative, 0 = neutral, +1 = very positive**.                                                                                |
| **subjectivity**        | Float (0 to 1)   | Subjectivity of the article: **0 = objective/factual, 1 = highly opinionated**.                                                                                                 |
| **source\_reliability** | Integer (1–10)   | Credibility rating of the news source: **1 = very unreliable, 10 = highly reliable**.                                                                                           |
| **impact\_score**       | Float (0–100)    |  A computed score representing the potential impact of the fake news article, influenced by engagement (shares, likes, comments), sentiment, and reliability. |


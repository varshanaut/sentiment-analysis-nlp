Sentiment Analysis NLP

Python NLP project using **TextBlob** and **Newspaper3k** for sentiment analysis.

## Example Code

```python
from textblob import TextBlob
from newspaper import Article

# Download and parse an article
url = "https://example.com/news-article"
article = Article(url)
article.download()
article.parse()
article.nlp()

# Perform sentiment analysis
blob = TextBlob(article.text)
print("Sentiment:", blob.sentiment)

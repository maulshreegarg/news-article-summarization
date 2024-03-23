# news-article-summarization
an NLP based project used to summarise given news paper articles in five lines.
Title:
Analyzing Blood Donation Camp News Article

Description:
This code snippet demonstrates how to extract information from a news article about a blood donation camp using the newspaper3k library in Python.

Features:
Downloads and parses the news article using the Article class from the newspaper3k library.
Extracts metadata such as title, authors, publication date, and summary from the article.
Utilizes NLTK for natural language processing tasks such as tokenization.
Displays the extracted information in the console.
Usage:
Install the required libraries:
bash
Copy code
!pip install newspaper3k
Import the necessary modules:
python
Copy code
import tkinter as tk
import nltk
from textblob import TextBlob
from newspaper import Article
Define the URL of the news article:
python
Copy code
url = "https://www.thehindu.com/incoming/blood-donation-camp-organised/article67345971.ece"
Download and parse the article:
python
Copy code
a = Article(url)
a.download()
a.parse()
Perform natural language processing tasks:
python
Copy code
nltk.download("punkt")
a.nlp()
Display the extracted information:
python
Copy code
print(f'Title: {a.title}')
print(f'Author: {a.authors}')
print(f'Publication Date: {a.publish_date}')
print(f'Summary: {a.summary}')
Dependencies:
newspaper3k
nltk
textblob
Usage Instructions:
Run the provided code snippet.
Ensure that the URL points to a valid news article.
Review the extracted information displayed in the console.
References:
Newspaper3k Documentation
NLTK Documentation
TextBlob Documentation
Author:
[Your Name]

License:
[License information]

Feel free to customize the README according to your preferences and requirements.

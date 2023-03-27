# midterm-project
Package Summary:

The TextBlob package offers a user-friendly API for tasks like text categorization, parts of speech tagging, and sentiment analysis, making it easier for Python programmers to work with human language text. It is constructed on top of other well-known NLP libraries, and because it is open-source, anyone can use it and contribute to it. Due to its simplicity and ease of use, TextBlob is a fantastic option for folks who are new to natural language processing.


Install and Run Instructions:

pip install textblob

python -m textblob.download_corpora


Code: 

Open and run textblobsamplecode.py

Edit the Sample text to perform a basic sentiment analysis on that piece of text

The code starts by importing the TextBlob class from the textblob package. We then define a function called get_sentiment() that takes a string as input. This function creates a TextBlob object from the input string and then calls the sentiment.polarity attribute of the object to get the sentiment polarity score of the text. The polarity score is a float value between -1 and 1, with negative values indicating negative sentiment, positive values indicating positive sentiment, and 0 indicating neutral sentiment.
The sentiment of the input text is then classified using an if statement based on the polarity score. When the polarity score is higher than 0, the text is categorized as "Positive." The text is categorized as "Negative" if the polarity score is less than 0. The text is categorized as "Neutral" if the polarity score is exactly 0.
Lastly, we use an example text string to call the get sentiment() function to show how it operates. The sentiment analysis of the supplied text is printed to the console by the code.
Overall, this code shows how to perform simple sentiment analysis on a snippet of text using the TextBlob library. We can rapidly and effectively extract information about the sentiment of text data using the TextBlob package, which can be helpful for a wide range of natural language processing jobs.


Future idea:

You can use the TextBlob package to evaluate customer reviews of a good or service and produce a report on how people feel about it for your final project in class. The report might display the proportion of favorable, unfavorable, and neutral evaluations as well as the most often discussed subjects. This report can be used by businesses to improve their goods and clientele.

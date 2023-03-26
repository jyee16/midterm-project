# midterm-project
textblob sample code


from textblob import TextBlob

def get_sentiment(txt):
    '''
    This function takes a string as input and returns the sentiment of the text using TextBlob package.

    Parameters:
    text (str): A string containing the text whose sentiment needs to be analyzed.

    Returns:
    sentiment (str): A string indicating whether the sentiment of the text is positive, negative or neutral.
    '''
    # Create a TextBlob object
    blob = TextBlob(txt)

    # Get the sentiment polarity (-1 to +1) and subjectivity (0 to 1) of the text
    sentiment_polarity = blob.sentiment.polarity
    sentiment_subjectivity = blob.sentiment.subjectivity

    # Determine the sentiment based on polarity
    if sentiment_polarity > 0:
        sentiment = 'positive'
    elif sentiment_polarity < 0:
        sentiment = 'negative'
    else:
        sentiment = 'neutral'

    return sentiment

# Sample Text To Test The Function
txt = "I dislike this boba, it's the the worst drink I've ever had!"
sentiment = get_sentiment(txt)
print(f"The sentiment of the text '{txt}' is {sentiment}.")

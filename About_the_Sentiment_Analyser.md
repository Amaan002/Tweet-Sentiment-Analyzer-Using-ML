Sentiment Analyser of Tweets


This project analyzes tweets to determine whether the sentiment behind each tweet is positive or negative. It’s useful for understanding public opinion on social media, monitoring reactions to products or brands, or gathering feedback on various topics. The goal is to quickly sort tweets into positive or negative categories based on their content.


How It Works

1. Text Cleaning:

• The first step involves cleaning the tweets by removing unnecessary components like URLs, mentions (e.g., @username), and hashtags (e.g., #topic). This ensures the analysis focuses on the text itself without distractions.

2. Converting Text to Numbers:

• Since computers can’t directly understand text, the cleaned tweets are converted into a numerical format using a technique called TF-IDF. This method helps represent the importance of words in a tweet and allows the machine to analyze it more easily.

3. Training a Model:

• The program uses past examples of labeled tweets (positive or negative) to “learn” the patterns and relationships between the words in the tweets and their sentiment. A Logistic Regression model is used for this training process.

4. Predicting Sentiment:

• Once the model is trained, it can predict whether a new tweet is positive or negative based on the words it contains. For example:

• A tweet like “I love this product!” would be classified as positive.

• A tweet like “This movie was terrible.” would be classified as negative.



Technologies Used

• Python: The programming language used to write the code and implement the sentiment analysis process.

• scikit-learn: A popular library for machine learning, used here to build the model that classifies tweets as positive or negative.

• Joblib: A library that allows you to save and load the trained model, so you don’t have to retrain it every time you want to use it.

• Regular Expressions (Regex): A tool used to clean and process the text data, removing unwanted characters like URLs, mentions, and hashtags.



Why It’s Useful

• Brand Monitoring: By analyzing the sentiment of tweets mentioning a brand or product, you can quickly gauge whether people have a positive or negative perception.

• Social Media Analytics: This project can be used to analyze public opinion on various topics, helping businesses or individuals understand the mood of the public.

• Customer Feedback: The model can automatically categorize feedback (e.g., reviews, comments) as positive or negative, making it easier to handle large volumes of data.
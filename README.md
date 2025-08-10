# Sentiment-Analysis
This project performs sentiment analysis on text data using TextBlob. It processes and cleans the dataset, calculates sentiment polarity, classifies text as positive, negative, or neutral, and visualizes results with bar plots and word clouds to highlight common words across sentiment categories. 

Workflow & Key Steps

    - Importing Required Libraries

        pandas – Data loading and preprocessing.

        matplotlib – Visualization of sentiment distribution.

        TextBlob – Sentiment polarity calculation and classification.

        WordCloud – Visual representation of frequently occurring words.

    - Loading the Dataset

        Reads a CSV file containing text data (3) Sentiment dataset.csv).

        Displays the first few rows to verify the dataset structure.

    - Sentiment Analysis

        Defines a custom function get_sentiment() that:

            Calculates polarity score using TextBlob (range: -1 = very negative, +1 = very positive).

            Classifies sentiment into:

                Positive (polarity > 0.1)

                Negative (polarity < -0.1)

                Neutral (otherwise)

        - Applies this function to all text entries and stores results in new columns:

            Polarity – numeric score.

            Predicted_Sentiment – categorical label.

    - Sentiment Distribution Visualization

        Creates a bar chart showing how many texts fall into Positive, Negative, and Neutral categories.

        Color-coded bars for easy differentiation.
        <img width="791" height="516" alt="image" src="https://github.com/user-attachments/assets/cb586473-65ca-4335-9a5b-8423e8dd66c5" />


        Word Cloud Generation

  #Generates an overall Word Cloud for all text data combined.

    - Creates separate Word Clouds for each sentiment category, revealing:

        Most common words in positive texts.

        Common negative sentiment terms.

        Neutral sentiment vocabulary.

    - Removes stopwords for cleaner visualization.

- Insights & Use Cases

    Quickly identifies dominant sentiment in the dataset.

    Highlights key words contributing to sentiment classification.

    Useful for analyzing social media posts, product reviews, or customer feedback.

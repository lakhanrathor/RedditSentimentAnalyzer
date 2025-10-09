# Reddit Sentiment Analyzer

Reddit Sentiment Analyzer is a web-based application that allows users to analyze the sentiment of Reddit comments in real-time or from pre-analyzed datasets. It provides a comprehensive dashboard with visualizations for sentiment distribution, emotion detection, keyword analysis, and topic extraction.

## Features

  * **Live Analysis:** Analyze Reddit comments for any topic and subreddit in real-time.
  * **Pre-Analyzed Datasets:** Explore sentiment patterns from pre-scraped Reddit comments on various topics.
  * **Sentiment Distribution:** View the breakdown of comments into positive, negative, and neutral sentiments.
  * **Emotion Detection:** Identify emotions such as joy, anger, sadness, fear, and surprise in the comments.
  * **Keyword Analysis:** Discover the most frequently used keywords for each sentiment category.
  * **Topic Extraction:** Automatically extract the main discussion topics from the comments.
  * **Interactive Dashboard:** Visualize the analysis results with interactive charts and graphs.
  * **Dark Mode:** Switch between light and dark themes for better viewing comfort.

## Tech Stack

### Backend

  * **Flask:** A micro web framework for Python.
  * **PRAW (Python Reddit API Wrapper):** For accessing Reddit's API.
  * **NLTK (Natural Language Toolkit):** For sentiment analysis and natural language processing.
  * **Pandas:** For data manipulation and analysis.
  * **Scikit-learn:** For topic extraction using TF-IDF.

### Frontend

  * **HTML, CSS, JavaScript:** For the application's structure, styling, and interactivity.
  * **Bootstrap:** A popular CSS framework for building responsive, mobile-first sites.
  * **Chart.js:** For creating interactive charts and graphs.
  * **Font Awesome:** For icons.

## Installation and Setup

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/RedditSentimentAnalyzer.git
    cd RedditSentimentAnalyzer
    ```

2.  **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

3.  **Set up Reddit API credentials:**

      * Create a Reddit application to get your API credentials.
      * Set the following environment variables:
        ```
        REDDIT_CLIENT_ID=your_client_id
        REDDIT_CLIENT_SECRET=your_client_secret
        REDDIT_USER_AGENT=your_user_agent
        ```

4.  **Run the Flask application:**

    ```bash
    python app.py
    ```

    The application will be running at `http://localhost:5000`.

## Usage

1.  **Choose an analysis mode:**

      * **Live Analysis:** Enter a topic and an optional subreddit to fetch and analyze comments in real-time.
      * **Pre-Analyzed Datasets:** Select a pre-scraped dataset from the dropdown to explore existing analysis.

2.  **View the results:** The dashboard will display various visualizations, including:

      * Sentiment distribution (doughnut chart and table).
      * Sentiment timeline (line chart).
      * Emotion distribution (polar area chart).
      * Key discussion topics.
      * Word clouds for positive, negative, and neutral keywords.
      * Sample comments for each sentiment.

## File Structure

```
├── app.py                  # Main Flask application
├── requirements.txt        # Python package dependencies
├── frontend/
│   ├── index.html          # Main HTML file for the UI
│   ├── css/style.css       # Custom CSS styles
│   └── js/script.js        # JavaScript for frontend logic
├── data/
│   ├── reddit_comments/    # Directory for pre-scraped CSV datasets
│   └── preprocessed_results/ # Directory for cached analysis results
└── ...
```

## Acknowledgements

  * This project utilizes several open-source libraries, including Flask, PRAW, NLTK, Pandas, and Scikit-learn.
  * The frontend is built with Bootstrap and Chart.js.

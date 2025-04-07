# Trustpilot Review Sentiment Analysis of Coca-Cola

## Overview

This project analyzes customer reviews of Coca-Cola on Trustpilot using sentiment analysis techniques. The goal is to extract insights about consumer perceptions of the Coca-Cola brand, identify key factors contributing to positive and negative sentiment, and uncover trends related to customer satisfaction and dissatisfaction. By leveraging Natural Language Processing (NLP) methods, including sentiment analysis, word frequency analysis, and bigram extraction, the project provides a deeper understanding of public opinion about Coca-Cola.

## Steps

### 1. **Review Data Collection**
- The first step is to scrape reviews of Coca-Cola from Trustpilot. This is done using web scraping techniques, specifically with `requests` and `beautifulsoup4`. The reviews are then structured into a clean DataFrame for further analysis.

### 2. **Sentiment Analysis**
- After collecting the reviews, sentiment analysis is performed using Hugging Face’s pre-trained models. Reviews are classified as positive or negative, and sentiment scores (polarity and subjectivity) are calculated and added to the dataset.

### 3. **Word Frequency Analysis**
- The frequency of words in both positive and negative reviews is calculated using `CountVectorizer`. This helps identify the most common words associated with positive and negative sentiments, providing an understanding of customer sentiment through their word choices.

### 4. **Bigram Analysis**
- To gain deeper insights into the context of the reviews, bigrams (two-word combinations) are extracted from the reviews. This highlights key phrases that are often used together, providing clarity about consumer perceptions, including brand loyalty, product quality, and customer concerns.

### 5. **Data Visualization**
- Visualizations such as bar charts and frequency plots are generated to help illustrate the results. These visualizations make the data more accessible and allow for a clear comparison between the most common words and bigrams in positive and negative reviews.

## Usage

To get started with the project, follow these steps:

1. Clone this repository:
    ```bash
    git clone https://github.com/Azneo/trustpilot-coca-cola-sentiment-analysis.git
    ```

2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the sentiment analysis script:
    ```bash
    python trustpilot_analysis.py
    ```

4. View the visualizations that compare word and bigram frequencies, and explore sentiment trends within the reviews.

## Requirements

- Python 3.x
- Libraries:
  - `transformers` (for sentiment analysis models)
  - `nltk` (for text preprocessing and stopword removal)
  - `pandas` (for data manipulation and analysis)
  - `requests` (for scraping reviews)
  - `beautifulsoup4` (for scraping reviews)
  - `matplotlib` (for creating visualizations)

The list of required libraries can be found in the `requirements.txt` file.

## Author

- **Aziz Ishan-Khojaev** - [Your GitHub Profile](https://github.com/Azneo)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

# News Topic Modeling

This repository contains a project focused on analyzing technology news articles using topic modeling techniques, specifically employing the Latent Dirichlet Allocation (LDA) model. The project fetches articles from a news API, processes the text data, and generates visualizations to reveal underlying topics in the news articles.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Code Overview](#code-overview)
- [Visualizations](#visualizations)
- [License](#license)

## Features

- Fetches technology news articles using the News API.
- Cleans and preprocesses text data for analysis.
- Applies LDA to identify topics within the articles.
- Generates a word cloud visualization of frequently occurring words.
- Creates an interactive HTML report with links to related news articles.

## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

Make sure you have the following installed:

- Python 3.x
- pip
- Git (to clone the repository)

### Installation

1. **Clone the Repository:**

   Open your terminal and run:

   ```bash
   git clone https://github.com/yourusername/news-topic-modeling.git
   cd news-topic-modeling
      
  2. Install required libraries:

     ```bash
     pip install wordcloud matplotlib requests nltk gensim pyLDAvis
     
  3. Download necessary NLTK resources:

     ```bash
     import nltk
     nltk.download('stopwords')

## Data Collection

This script uses the News API to fetch the latest articles. Replace API_KEY in the code with your News API key.

    ```bash
    # Querying the API
    url = f'https://newsapi.org/v2/everything?q=technology&apiKey={API_KEY}'
    response = requests.get(url)
    data = response.json()

## Data Cleaning

Each article's content is cleaned by:

  - Removing URLs, mentions, and hashtags
  - Removing punctuation and numbers
  - Converting to lowercase and removing stopwords

    ```python
    def clean_text(text):
    # Your text cleaning function







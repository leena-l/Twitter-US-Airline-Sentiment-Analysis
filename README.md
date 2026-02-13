# Twitter US Airline Sentiment Analysis

This project performs Exploratory Data Analysis (EDA) and Natural Language Processing (NLP) on a dataset of tweets directed at major US airlines. The goal is to understand customer satisfaction and visualize the primary topics within positive, neutral, and negative feedback.

The dataset contains over 14,000 tweets from 2015, classified by sentiment. This project processes the raw text to remove noise (mentions, URLs, special characters) and generates visual insights to identify which airlines struggle most with customer service and what common keywords appear in their mentions

# Technologies Used

Python 3.x

Pandas: Data manipulation and cleaning.

Seaborn/Matplotlib: Data visualization.

WordCloud: Text data visualization.

Re (Regex): Text preprocessing and noise removal.

# Dataset Insights

The dataset includes 15 columns, with the most critical being:

1 - airline_sentiment: The target label (negative, neutral, or positive).

2 - text: The raw tweet content.

3 - airline: The specific airline mentioned (e.g., Virgin America, United, Southwest).

Current Class Distribution:

Negative: 9,178

Neutral: 3,099

Positive: 2,363

# Data Cleaning Process

To prepare the text for analysis, the following steps were implemented:

1 - Lowercasing: All text converted to lowercase.

2 - Noise Removal: Used Regex to strip -Twitter handles (@user) , Hyperlinks (http...) , Special characters and numbers (keeping only a-z)

3 - Whitespace Trimming: Removing leading/trailing spaces.

# Visualizations

1 - Word Clouds by Sentiment
   
We generated Word Clouds for each sentiment category to visualize the most frequent terms. For instance, "thank" and "great" dominate positive tweets, while "flight," "cancelled," and "delayed" are prevalent in negative ones.

2 - Sentiment Distribution per Airline
   
The project includes a grouped bar chart comparing sentiment counts across different carriers.

# Observation: 
Some airlines (like United and US Airways) show a significantly higher volume of negative feedback compared to others.

# How to Run

1 - Clone this repository.

2 - Install dependencies - pandas  , seaborn ,  matplotlib  , wordcloud

3 - Run the Python script or Jupyter Notebook. The data is fetched directly from the source URL provided in the code.




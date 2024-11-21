# Sentiment-Analysis-Default-Behavior-Analysis
This Jupyter Notebook analyzes customer sentiment using textual reviews. It leverages natural language processing (NLP) techniques to preprocess text data and extract sentiment scores. The project visualizes the distribution of sentiments to gain insights into customer opinions.
Synthetic Customer Data Generator
Overview
This Python script generates a synthetic dataset of customer reviews and related information for use in data analysis, machine learning, or any other project requiring sample customer data. The generated data includes random customer IDs, ages, regions, payment statuses, reviews, and timestamps. The dataset is saved to a CSV file.

Features
Random Customer Data: Generates unique customer IDs, ages (18–75), and regions.
Random Reviews: Includes a set of predefined customer reviews reflecting various financial sentiments.
Payment Status: Randomly assigns payment statuses ("Defaulted" or "On Time").
Timestamps: Creates random timestamps within a specified date range (2020–2024).
CSV Output: Saves the generated dataset to a CSV file for easy use in other applications.
Requirements
Python 3.6 or higher
Required Libraries:
pandas
random
datetime
How to Use
Install Required Libraries: Ensure that pandas is installed. If not, install it using:

bash
Copy code
pip install pandas
Run the Script: Execute the script in a Python environment. It generates the dataset with the desired number of records (default is 1,000).

Modify the Number of Records: To generate a different number of records, change the value of num_records:

python
Copy code
num_records = 5000  # Replace 5000 with your desired record count
Output: The dataset is saved as customer_data_with_date.csv in the current working directory.

Dataset Columns
The generated dataset contains the following columns:

Customer ID: A unique identifier for each customer (e.g., CUST12345).
Age: Customer age (randomly chosen between 18 and 75).
Region: Customer's geographical region (North, South, East, West, Central).
Review: A customer review selected randomly from predefined options.
Payment Status: Either "Defaulted" or "On Time."
Date: A random timestamp in the format DD-MM-YYYY HH:MM:SS.

Customization
Add More Reviews: Modify the reviews list in generate_random_review() to include more options.
Change Date Range: Adjust the start_date and end_date variables in the generate_random_date() function.
Customize Columns: Extend or modify the data fields to suit your requirements.
License
This project is open-source and free to use. No warranties are provided.



-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Customer Sentiment Analysis
Overview
This Jupyter Notebook analyzes customer sentiment using textual reviews. It leverages natural language processing (NLP) techniques to preprocess text data and extract sentiment scores. The project visualizes the distribution of sentiments to gain insights into customer opinions.

Key Features
Data Preprocessing:

Converts text to lowercase.
Removes handles, hashtags, URLs, special characters, and single characters.
Cleans up multiple spaces.
Sentiment Analysis:

Uses the nltk SentimentIntensityAnalyzer (SIA) for extracting polarity scores (positive, neutral, negative).
Adds sentiment columns (Positive Sentiment, Neutral Sentiment, Negative Sentiment) to the dataset.
Data Visualization:

Plots Kernel Density Estimates (KDE) to illustrate the distribution and cumulative density of sentiment scores.
Highlights cut-offs for extreme positive and negative responses.
Technologies Used
Programming Language: Python
Libraries:
Data Processing: numpy, pandas
NLP: nltk
Visualization: matplotlib, seaborn, plotly
Sentiment Analysis: SentimentIntensityAnalyzer from nltk
Prerequisites
Ensure the following Python libraries are installed:

bash
Copy code
pip install numpy pandas matplotlib seaborn plotly nltk wordcloud statsmodels
Usage
Load the Notebook: Open the Default_Customer_Sentiment_Analysis.ipynb file in Jupyter Notebook.

Data Input:

Replace the sample CSV path with your own dataset in the following code:
python
Copy code
f_data = pd.read_csv(r'path_to_your_dataset.csv')
Run the Notebook: Execute cells sequentially to preprocess data, perform sentiment analysis, and generate visualizations.

Interpret Results:

Use visualizations to understand the sentiment distribution.
Review statistical cut-offs for extreme responses.
Project Structure
Data Preprocessing:
Cleaning and preparing raw review data for analysis.
Sentiment Scoring:
Assigning polarity scores using SIA.
Visualization:
Graphical representation of sentiment scores for insights.
Output
The analysis results include:

A processed dataset with sentiment scores.
Plots for understanding the sentiment trends.
Acknowledgments
Libraries: nltk, plotly, and seaborn for enabling powerful analysis and visualization.
Dataset: Sample data provided for demonstration purposes.

Author
Rishi Khanna
45-year-old IT professional with 19+ years in BFS.

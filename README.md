# Stock Market Prediction with News Headlines

A machine learning project to predict the daily movement of the Dow Jones Industrial Average (DJIA) based on the sentiment of financial news headlines.

![Final Refined Word Cloud](https://github.com/user-attachments/assets/89716b32-fdee-45e6-a25c-e8ac020ebddb)

## Project Goal
The goal of this project was to build an end-to-end data science pipeline to determine if the sentiment of financial news could be used to predict whether the stock market will close up or down with an accuracy greater than random chance (50%).

## Dataset
The dataset used was the "Daily News for Stock Market Prediction" from Kaggle, containing news headlines from 2008 to 2016.
[Link to dataset](https://www.kaggle.com/datasets/aaron7sun/stocknews)

## Methodology
1.  **Data Cleaning:** Raw text data was cleaned by combining all daily headlines, converting all text to lowercase, and removing all non-alphabetic characters and common stopwords.
2.  **Feature Engineering:** The cleaned headlines were vectorized using `CountVectorizer` with a 2-word ngram range to convert the text into a numerical format.
3.  **Modeling:** The data was split into an 80% training set and a 20% testing set. A **Logistic Regression** model was trained on the training data.
4.  **Evaluation:** The trained model was then tested on the unseen test data. Performance was evaluated using an accuracy score and a confusion matrix.

## Results
The model achieved a final accuracy of **54.27%** on the test set. While modest, this score performs better than a random guess. The project also includes visualizations like word clouds and a confusion matrix to better understand the data and model performance.

## How to Run
1.  Ensure you have Python and Jupyter Notebook installed.
2.  Clone this repository.
3.  Install the required libraries: `pip install -r requirements.txt`
4.  Run the `analysis.ipynb` notebook.

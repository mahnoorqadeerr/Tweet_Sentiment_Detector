#  Tweet Sentiment Detector

This project is a basic sentiment analysis tool built using Python, scikit-learn, and NLP techniques. It classifies tweets as **positive** or **negative** based on their content.

##  Project Overview

- **Dataset**: 1.6 million preprocessed tweets from the `training.1600000.processed.noemoticon.csv` file
- **Goal**: Predict tweet sentiment using a logistic regression model
- **Accuracy Achieved**: 77.36%

##  Workflow Summary

1. **Data Preprocessing**
   - Removed URLs, mentions, hashtags, and punctuation
   - Converted text to lowercase
   - Removed stopwords using NLTK

2. **Label Mapping**
   - Original `target` values (0 = negative, 4 = positive) mapped to binary sentiment (0 or 1)

3. **Feature Extraction**
   - Used `TfidfVectorizer` with 5000 features to convert text into numerical format

4. **Model Training**
   - Trained a `LogisticRegression` model using an 80/20 train-test split
   - Evaluated using accuracy score and confusion matrix

##  Results

- **Accuracy**: `77.36%`
- **Confusion Matrix**: Visualized using Seaborn

##  Technologies Used

- Python
- Pandas, NumPy
- scikit-learn
- NLTK
- Matplotlib, Seaborn

## How to Run

```bash
# Install dependencies
!pip install pandas numpy scikit-learn nltk

# Upload and unzip dataset
from google.colab import files
uploaded = files.upload()
!unzip tweet.zip

# Run all cells in the notebook


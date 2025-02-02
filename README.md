# Sentiment Analysis and Spam Detection

## Live Demo :-

[![Streamlit App](https://img.shields.io/badge/Streamlit-App-blue)](https://sentiment-spam-detection-by-prince.streamlit.app/)

## Best Practices (As Suggested by Krish Naik)

### 1. Preprocessing and Cleaning

- **Text Cleaning**: Remove stop words, punctuation, special characters, and handle case sensitivity.
- **Tokenization**: Split the text into individual words (tokens).
- **Lemmatization**: Reduce words to their base or root form to improve uniformity.
- **Removing Duplicates**: Remove duplicate entries to avoid biases in model training.

### 2. Train Test Split

- **Data Split**: Split the dataset into a training set (typically 80%) and a test set (20%) to evaluate the model's performance on unseen data.

### 3. Feature Extraction: BOW, TF-IDF, Word2Vec

- **Bag of Words (BOW)**: Convert the text into a set of features based on word frequencies.
- **TF-IDF**: Weigh words based on their importance using term frequency and inverse document frequency.
- **Word2Vec**: Generate word vectors that capture semantic relationships between words.

### 4. Training ML Algorithms

- Start with simple and effective models like **Multinomial Naive Bayes (MNB)**, and explore other algorithms like **Support Vector Machines (SVM)**, **Logistic Regression**, or **Random Forest** for more complex tasks.

## Models Used

### Sentiment Analysis

1. **Bag of Words (BoW) with Multinomial Naive Bayes (MNB)**

   - **Accuracy**: 85%
   - This model uses the Bag of Words approach to convert text into feature vectors and then classifies sentiments using Multinomial Naive Bayes.

2. **TF-IDF (Term Frequency-Inverse Document Frequency)**

   - **Accuracy**: 70%
   - TF-IDF evaluates the importance of words based on their frequency and inverse document frequency, and uses a machine learning classifier to predict sentiment.

3. **Average Word2Vec**
   - **Accuracy**: 75%
   - This model uses Word2Vec to convert words into vectors and averages the vectors to classify the sentiment of the text.

### Spam Detection

1. **Bag of Words (BoW) with Multinomial Naive Bayes (MNB)**

   - **Accuracy**: 98%
   - This model uses the Bag of Words approach to convert text into feature vectors and then classifies messages as Spam or Ham using Multinomial Naive Bayes.

2. **TF-IDF**

   - **Accuracy**: 97%
   - This model evaluates the importance of words and classifies messages based on term frequency and inverse document frequency.

3. **Word2Vec**
   - **Accuracy**: 94%
   - This model uses Word2Vec to generate word embeddings and classifies the messages.

## Setup Instructions

### 1. Clone the Repository

To clone the repository, use the following command:

```bash[
git clone https://github.com/prince2004patel/sentiment-spam-detection.git
```

### 2. Install Dependencies

To install the required dependencies for this project, use the following command:

1. Ensure you are in the project directory:

```bash
cd sentiment-spam-detection
```

2. This will install all the necessary Python libraries required for both the Flask back-end and Streamlit front-end to work properly:

```bash
pip install -r requirements.txt
```

### 3. Run the Application

1. Ensure you are in the project directory:

```bash
cd sentiment-spam-detection
```

2. Start the Streamlit app:

```bash
streamlit run app.py
```

## Some Screenshots

![Kindle Sentiment Analysis](img/img1.png)

![SMS Spam Detection](img/img2.png)

![About This Project](img/img3.png)

# Sentiment Analysis with Textblob

This project performs detailed sentiment analysis on tweets using advanced text preprocessing, NLP techniques, and sentiment scoring with `TextBlob`. It includes a robust data import system compatible with Colab/Kaggle, followed by cleaning, feature extraction, and visualization of sentiment polarity and subjectivity.

---

## 📥 Dataset Import (Kaggle-Compatible)

The script begins by importing a dataset from Kaggle via a long download URL. It handles `.zip` or `.tar` files, unpacks them, and places the data in `/kaggle/input`.

---

## 🧹 Text Preprocessing Steps

- Convert to lowercase
- Remove:
  - Stopwords (using NLTK)
  - URLs
  - Punctuation
  - Repeating characters
  - Numbers
  - Short words (length ≤ 2)
- Apply:
  - Tokenization (`TweetTokenizer`)
  - Stemming (`PorterStemmer`)
  - Lemmatization (`WordNetLemmatizer`)

---

## 📊 Sentiment Scoring (TextBlob)

- **Polarity**: float from -1 (negative) to 1 (positive)
- **Subjectivity**: float from 0 (objective) to 1 (subjective)

Each tweet is categorized into:
- `positive`
- `neutral`
- `negative`

---

## 📈 Visualization

Includes:
- WordClouds for:
  - All tweets
  - Positive tweets
  - Negative tweets
  - Neutral tweets
- Scatter plot: `Polarity` vs. `Subjectivity`
- Bar chart: Sentiment distribution

---

## 📌 Results

- **Neutral tweets**: 48.4%
- **Positive tweets**: 44.1%
- **Negative tweets**: 7.5%

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn, WordCloud
- NLTK (stopwords, stemmers, tokenizers)
- TextBlob (sentiment analysis)

---

## 🔗 Colab Access

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/marhum456/data-analysis-portfolio/blob/main/climate-change-sentiment-analysis/Sentiment-Analysis-Using-TextBlob.ipynb)


## 📁 Dataset Format

- Source file: `Sample Data.txt`
- Format: JSON Lines or text
- Converted to CSV inside the notebook

---

## ✅ Conclusion

This project demonstrates a complete end-to-end NLP pipeline for sentiment classification. It emphasizes both linguistic cleaning and visual interpretability. The combination of preprocessing, sentiment scoring, and visual analytics makes this approach ideal for analyzing tweet-based sentiment trends.

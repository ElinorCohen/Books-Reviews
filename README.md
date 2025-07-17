# 📚 Book Reviews Sentiment Analysis

This project predicts whether a person **liked a book or not** based on their written review using Natural Language Processing (NLP) and Machine Learning techniques.

---

## 🔍 Objective

Predict user sentiment about books from free-form text reviews.

![Slide - Objective](images/slide-1.png)

---

## 📊 Dataset

- **Source:** [Goodreads](https://www.goodreads.com)
- **Size:** ~125K reviews after cleaning
- **Fields collected:**  
  Book metadata, review text, ratings, user engagement, genres, etc.
- **Target variable:**  
  - `1` → Like (rating ≥ 4)  
  - `0` → Dislike (rating ≤ 3)

![Slide - Data Crawling](images/slide-3.png)
![Slide - Data Size](images/slide-6.png)

---

## ⚙️ Methodology

### 🧹 Data Cleaning & Preprocessing
- Dropped NaN & duplicates
- Normalized numerical columns
- Grouped genre & cover categories
- Converted years, extracted metadata
- Balanced classes (like/dislike)

![Slide - Preprocessing](images/slide-7.png)
![Slide - Genre Categorization](images/slide-8.png)
![Slide - Class Balance](images/slide-11.png)

---

### 🧠 NLP Feature Engineering

- Tokenization, POS tagging, lemmatization
- Stop words removal
- Positive & negative word lists
- Word counts, vectorized terms (CountVectorizer)
- Custom columns: `num_positive`, `num_negative`, etc.

![Slide - NLP Steps](images/slide-12.png)
![Slide - Common Words](images/slide-18.png)
![Slide - Word Vectors](images/slide-16.png)

---

### 📈 Exploratory Data Analysis

- Correlation heatmap using Spearman
- Word sentiment trends
- Distribution of review types and sentiment

![Slide - Correlation](images/slide-17.png)
![Slide - Positive Words vs Tags](images/slide-19.png)
![Slide - Target Balance](images/slide-21.png)

---

## 🤖 Machine Learning Model

- **Model used:** `AdaBoostClassifier`
- Dropped string and label-leaking columns
- Trained on 80% of the data, tested on 20%
- **Accuracy:** 57%

![Slide - Model Process](images/slide-26.png)
![Slide - Final Score](images/slide-27.png)

---

## 🧪 Technologies Used

- `Python`
- `Selenium` (data scraping)
- `Pandas`, `NumPy`
- `Scikit-learn`
- `NLTK`
- `Matplotlib`, `Seaborn`

---

## 📎 Presentation

🎞️ View the full presentation: [BooksReviews.pdf](BooksReviews.pdf)

# Sentiment Analysis on Product Reviews 🎭

This project was completed as **Task 1** of the Elevvo Pathways NLP Internship.  
The goal was to build an end-to-end sentiment analysis pipeline on product/movie reviews to classify them as **positive** or **negative**.

---

## 📌 Project Description
- Dataset: [IMDb Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews) (50,000 labeled reviews)
- Task: Analyze product reviews to determine sentiment (positive/negative)
- Preprocessing:  
  - Lowercasing text  
  - Removing punctuation and numbers  
  - Lemmatization with **spaCy**  
  - Removed stopwords but kept the word "not" for negation
  - Optimized preprocessing using `nlp.pipe` with batching for efficiency
- Feature Extraction: **TF-IDF vectorization**
- Models:
  - Logistic Regression
  - Multinomial Naive Bayes
- Evaluation: Precision, Recall, F1-score, and Accuracy
- Bonus:
  - Visualized most frequent positive/negative words
  - Compared Logistic Regression vs Naive Bayes performance

---

## ⚙️ Tools & Libraries
- Python  
- Pandas  
- scikit-learn  
- spaCy  
- NLTK  
- Matplotlib / Seaborn  

---

## 📊 Results

### Logistic Regression
- Accuracy: ~0.89  
- Macro F1-score: ~0.89  

### Multinomial Naive Bayes
- Accuracy: ~0.86  
- Macro F1-score: ~0.86  

**Why Logistic Regression performed better:**  
Logistic Regression directly learns feature weights and works naturally with TF-IDF features, while Naive Bayes assumes feature independence and fits raw counts better. With a large dataset, Logistic Regression captures word dependencies more effectively.

---

## 📈 Sample Visualizations
- Top 10 most frequent positive words  
- Top 10 most frequent negative words  


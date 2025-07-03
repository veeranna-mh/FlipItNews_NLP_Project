# 📰 FlipItNews NLP Project

## 🔍 Project Overview

**FlipItNews** is a Gurugram-based startup focused on reinventing financial literacy in India through smart content discovery. This NLP project aims to support that mission by automatically classifying news articles into predefined categories using classical machine learning techniques.

## 🎯 Objective

To classify a collection of news articles into categories like:

- 🏛️ Politics
- 💻 Technology
- ⚽ Sports
- 💼 Business
- 🎬 Entertainment

using Natural Language Processing (NLP) and multi-class classification models.

---

## 📁 Dataset

The dataset consists of two columns:

- `Article`: News article content (text)
- `Category`: Target label (one of the five categories)

---

## 🧠 Concepts Used

### 📌 NLP Preprocessing:
- Text cleaning (non-letters removal)
- Tokenization
- Stopword removal
- Lemmatization

### 📌 Feature Engineering:
- Bag of Words (BoW)
- TF-IDF (Term Frequency–Inverse Document Frequency)

### 📌 Classification Models:
- Naive Bayes
- Decision Tree
- K-Nearest Neighbors (KNN)
- Random Forest

### 📌 Model Evaluation:
- Train/Test accuracy comparison
- Classification report (precision, recall, F1)
- Confusion matrix visualization
- Summary table of all models

---

## 📊 Exploratory Analysis

- Top words per category extracted using `Counter`
- WordClouds plotted for each category using `WordCloud` and `matplotlib`

---

## ✅ Key Results

| Model           | Train Accuracy | Test Accuracy |
|----------------|----------------|---------------|
| Naive Bayes     | *e.g., 93.2%*   | *91.5%*        |
| Decision Tree   | *100.0%*        | *80.2%*        |
| KNN             | *92.6%*         | *90.1%*        |
| Random Forest   | *100.0%*        | *87.0%*        |

> 📌 *Naive Bayes* and *KNN* showed balanced performance without overfitting.  
> 📌 *Random Forest* and *Decision Tree* had overfitting issues (high training accuracy, lower test accuracy).

---

## 🧾 Conclusion

- TF-IDF outperformed BoW in representing textual features effectively.
- Classical models like **Naive Bayes** and **KNN** worked best for this dataset.
- This project demonstrates how simple preprocessing + feature extraction + classical ML can perform competitively on real-world multi-class NLP problems.

---

## 🔄 Future Improvements

- Hyperparameter tuning using GridSearchCV
- Integration with deep learning (e.g., BERT, LSTM)
- Web-based article classification demo using Streamlit

---

## 💻 How to Run

```bash
# 1. Create virtual environment
conda create -n flipitnews python=3.10 -y
conda activate flipitnews

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run Jupyter Notebook
jupyter notebook

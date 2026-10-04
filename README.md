# 📰 Fake News Detection

A beginner-friendly **Machine Learning + NLP** project that predicts whether a news article is **REAL or FAKE**.

## 🧠 How It Works

```text
News Text → TF-IDF → Logistic Regression → REAL / FAKE
```

## 🛠️ Tech Stack

- Python
- Pandas
- Scikit-learn
- TF-IDF
- Logistic Regression
- Streamlit

## ✨ Features

- News text classification
- Prediction confidence
- Model evaluation
- Simple Streamlit interface

## 🚀 Run

```bash
pip install -r requirements.txt
python train.py
streamlit run app.py
```

## 📂 Dataset

Place the dataset at:

```text
data/news.csv
```

Required columns:

```text
text,label
```

Labels: `REAL` / `FAKE`

## 🎓 Project

**1st Year B.Tech — AI & Machine Learning**

> Educational project. Predictions may not always be accurate.

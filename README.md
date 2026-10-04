# 📰 Fake News Detection

Beginner-friendly **NLP + Machine Learning** project for a 1st-year B.Tech student.

## Features
- TF-IDF feature extraction
- Logistic Regression
- REAL / FAKE prediction
- Confidence score
- Streamlit interface
- Training and evaluation script

## Run
```bash
pip install -r requirements.txt
python train.py
streamlit run app.py
```

Put a labeled dataset at `data/news.csv` with `text,label` columns. See `DATASET.md`.

> Educational classifier only. A prediction is not proof that a news story is true or false.

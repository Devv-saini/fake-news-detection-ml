
# 📰 Fake News Detection Using Machine Learning

A beginner-friendly **Natural Language Processing (NLP) and Machine Learning** project that classifies news text as **REAL** or **FAKE** using **TF-IDF** and **Logistic Regression**.

> 🎓 **Academic Project:** 1st Year B.Tech — Artificial Intelligence & Machine Learning

---

## 📌 Overview

The rapid spread of misleading information on the internet makes it difficult to determine whether a news article is genuine.

This project demonstrates how machine learning can be used to identify patterns in news text and classify an article as either **REAL** or **FAKE**.

The system takes a news headline or article as input, converts the text into numerical features using **TF-IDF**, and then uses a **Logistic Regression classifier** to make the prediction.

---

## ✨ Features

- 📰 News headline/article classification
- 🔤 Text preprocessing using TF-IDF
- 🤖 Logistic Regression machine-learning model
- 📊 Model accuracy and evaluation
- 📈 Classification report and confusion matrix
- 🎯 Prediction confidence
- 🖥️ Interactive Streamlit web interface
- 💾 Trained model can be saved and reused
- 👨‍🎓 Beginner-friendly implementation

---

## 🧠 How It Works

```text
             News Article
                  │
                  ▼
        Text Preprocessing
                  │
                  ▼
          TF-IDF Vectorizer
                  │
                  ▼
       Logistic Regression
                  │
          ┌───────┴───────┐
          ▼               ▼
        REAL             FAKE
```

### 1. Input

The user enters a news headline or article.

### 2. TF-IDF

TF-IDF (**Term Frequency–Inverse Document Frequency**) converts text into numerical values based on the importance of words in the dataset.

### 3. Machine Learning

The numerical features are passed to a **Logistic Regression** classifier.

### 4. Prediction

The model predicts:

- ✅ REAL
- ❌ FAKE

The Streamlit application also displays the model's estimated confidence.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Dataset handling |
| NumPy | Numerical operations |
| Scikit-learn | Machine learning |
| TF-IDF | Text feature extraction |
| Logistic Regression | Classification |
| Streamlit | Web interface |
| Joblib | Model saving/loading |

---

## 📂 Project Structure

```text
fake-news-detection/
│
├── data/
│   ├── sample_news.csv
│   └── news.csv              # Your dataset
│
├── models/
│   └── fake_news_model.pkl   # Generated after training
│
├── train.py                  # Model training
├── app.py                    # Streamlit application
├── requirements.txt          # Required libraries
├── DATASET.md                # Dataset instructions
├── README.md
├── LICENSE
└── .gitignore
```

---

## 📊 Dataset

The model requires a labeled CSV dataset.

Expected format:

```csv
text,label
"Scientists publish a new research study",REAL
"Aliens secretly control every bank",FAKE
```

The required columns are:

```text
text
label
```

Labels should be:

```text
REAL
FAKE
```

For a real project, use a properly licensed fake-news dataset rather than relying on the small sample file included in the repository.

> ⚠️ Large datasets should generally not be uploaded directly to GitHub unless their license allows redistribution.

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone <YOUR-GITHUB-REPOSITORY-URL>
cd fake-news-detection
```

### 2. Create a virtual environment

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

macOS/Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🧠 Train the Model

Place your dataset inside:

```text
data/news.csv
```

Then run:

```bash
python train.py
```

The training script will:

1. Load the dataset
2. Clean the data
3. Split it into training and testing data
4. Convert text into TF-IDF features
5. Train the Logistic Regression model
6. Evaluate the model
7. Save the trained model

The model will be saved as:

```text
models/fake_news_model.pkl
```

---

## 🖥️ Run the Application

After training:

```bash
streamlit run app.py
```

A browser window will open with the Fake News Detection interface.

Example:

```text
Enter News
    ↓
Check News
    ↓
Prediction: REAL / FAKE
    ↓
Confidence Score
```

---

## 📈 Model Evaluation

The training script displays:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

Example:

```text
Accuracy: XX.XX%

              precision    recall    f1-score

FAKE             XX         XX         XX
REAL             XX         XX         XX
```

**Actual results depend on the dataset used.**

---

## 🔮 Future Improvements

Possible future improvements include:

- Using advanced NLP models
- Adding multiple news sources
- Better text preprocessing
- Using transformer-based models such as BERT
- Multilingual fake-news detection
- Browser extension for checking articles
- Real-time news verification
- Source credibility analysis
- Explainable AI showing important words/features

---

## ⚠️ Limitations

This project is a **machine-learning classification system**, not a complete fact-checking system.

The model learns patterns from its training dataset and may produce incorrect predictions.

A prediction of **REAL does not prove that an article is true**, and a prediction of **FAKE does not prove that it is false**.

---

## 🎓 Learning Outcomes

Through this project, students can learn:

- Basics of NLP
- Text preprocessing
- TF-IDF
- Supervised machine learning
- Classification
- Model evaluation
- Train/test splitting
- Model persistence
- Building a simple ML web application

---

## 👨‍💻 Author

**Your Name**

B.Tech — Computer Science Engineering  
Specialization: Artificial Intelligence & Machine Learning

---

## 📄 License

This project is available under the **MIT License**.

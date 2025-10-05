# IMDB-sentiment-analysis
This project focuses on Sentiment Analysis using Natural Language Processing (NLP) and Deep Learning with TensorFlow. The primary objective is to automatically classify movie reviews from the IMDB dataset as either positive or negative, based on their textual content. Sentiment analysis is one of the most popular NLP tasks.


🎬 IMDB Movie Review Sentiment Analysis (TensorFlow NLP Project)

A **Deep Learning NLP project** that classifies IMDB movie reviews as **Positive 😀** or **Negative 😞** using **TensorFlow** and **Bidirectional LSTM** networks.

---

## 🧾 Overview

This project performs **Sentiment Analysis** using **Natural Language Processing (NLP)** and **TensorFlow**.  
It aims to automatically predict whether a movie review expresses a positive or negative emotion.  

The model is trained on a cleaned IMDB dataset, where reviews are tokenized, padded, and passed into a **Bidirectional LSTM** neural network for contextual understanding.

---

## ⚙️ Tech Stack

- 🐍 **Language:** Python  
- 🧠 **Libraries:** TensorFlow, Keras, scikit-learn, pandas, numpy, re  
- 🧩 **Model:** Bidirectional LSTM  
- 💻 **Tools:** Jupyter Notebook, Anaconda  

---

## 📂 Dataset Info

- **File:** `IMDB_cleaned.csv`  
- **Columns:**  
  - `cleaned_review` → Preprocessed text data  
  - `sentiment` → Label (`Positive` / `Negative`)  

---

## 🧱 Model Architecture

| Layer | Type | Description |
|-------|------|--------------|
| 1 | Embedding | Word vector representation |
| 2 | Bidirectional LSTM | Learns forward & backward context |
| 3 | Dense (ReLU) | Hidden layer |
| 4 | Dropout | Prevents overfitting |
| 5 | Dense (Sigmoid) | Binary output layer |

---

## ⚙️ Training Configuration

| Parameter | Value |
|------------|--------|
| Optimizer | Adam |
| Loss | Binary Crossentropy |
| Epochs | 10 |
| Batch Size | 64 |
| Accuracy | ~85–90% |

---

## 📈 Model Evaluation

✅ Achieved **85–90% accuracy** on the test set.  
✅ Can analyze new reviews and predict their sentiment in real time.

---

## 💬 Example Predictions

```python
Review: "The film was boring and too long."
Prediction: Negative 😞 (Confidence: 0.12)

Review: "Absolutely fantastic movie with great acting!"
Prediction: Positive 😀 (Confidence: 0.91)

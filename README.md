# Shopee-Sentimen-Analysis
# 📊 Sentiment Analysis of Shopee Reviews

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![HuggingFace](https://img.shields.io/badge/Transformers-🤗-yellow)
![Colab](https://img.shields.io/badge/Run%20on-Colab-orange?logo=googlecolab)

## 📌 Project Overview
This project analyzes **customer reviews from Shopee** and classifies them into **positive, neutral, and negative sentiments**.  
We use **Natural Language Processing (NLP)** with a Transformer model (**IndoBERT**) to extract insights about customer satisfaction.

---

## 🎯 Objectives
- Classify Shopee reviews into **positive**, **neutral**, and **negative**.
- Identify main drivers of satisfaction and dissatisfaction.
- Provide actionable recommendations for sellers and the platform.

---

## 📊 Dataset
- **Source:** Shopee_Sampled_Reviews.csv  
- **Size:** 2,500 reviews  
- **Columns:**  
  - `content` → review text  
  - `score` → rating (1–5)  

### Sentiment Mapping
- `1–2` → Negative  
- `3`   → Neutral  
- `4–5` → Positive  

---

## ⚙️ Tools & AI Support
- [Google Colab](https://colab.research.google.com/)  
- [Transformers (HuggingFace)](https://huggingface.co/transformers/)  
- IndoBERT (`indobenchmark/indobert-base-p1`)  
- scikit-learn for metrics  
- matplotlib & seaborn for visualization  

---

## 🔍 Analysis Process
1. Load dataset & preprocess (extract `content` & `score`)  
2. Map review scores → sentiment labels  
3. Split dataset (80% train, 20% test)  
4. Tokenize text with IndoBERT tokenizer  
5. Train IndoBERT for sentiment classification  
6. Evaluate model with classification report & confusion matrix  
7. Visualize sentiment distribution & performance  

---

## 📈 Results & Findings

### Sentiment Distribution
![Sentiment Distribution](results/sentiment_distribution.png)

### Confusion Matrix
![Confusion Matrix](results/confusion_matrix.png)

- Majority reviews are **positive**.  
- Negative reviews highlight issues like *slow delivery* and *app performance*.  
- Positive reviews mention *fast delivery*, *good packaging*, and *affordable prices*.  

---

## ✅ Conclusion & Recommendations
- Sellers should improve **delivery time & product quality**.  
- Maintain positive aspects such as **packaging & pricing**.  
- Shopee could optimize **app performance** for better experience.  

---

## 🚀 How to Run
1. Clone repo:
   ```bash
   git clone https://github.com/your-username/Shopee-Sentiment-Analysis.git
   cd Shopee-Sentiment-Analysis

# Shopee-Sentimen-Analysis
# 📊 Sentiment Analysis of Shopee Reviews

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![HuggingFace](https://img.shields.io/badge/Transformers-🤗-yellow)
![Colab](https://img.shields.io/badge/Run%20on-Colab-orange?logo=googlecolab)

---

## 📌 Project Overview
This project analyzes **customer reviews from Shopee** and classifies them into **positive, neutral, and negative sentiments**.  
We use **Natural Language Processing (NLP)** with a Transformer model (**IndoBERT**) to extract insights about customer satisfaction and provide actionable recommendations for improvement.

---

## 🎯 Objectives
- Classify Shopee reviews into **positive**, **neutral**, and **negative** categories.  
- Identify the main drivers of customer satisfaction and dissatisfaction.  
- Provide insights and recommendations for sellers and the platform.  

---

## 📊 Dataset
- **Source:** Shopee_Sampled_Reviews.csv (provided dataset)  
- **Size:** 2,500 reviews  
- **Columns Used:**  
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
- scikit-learn for metrics & evaluation  
- matplotlib & seaborn for visualization  

---

## 🔍 Analysis Process
1. Load dataset & preprocess (extract `content` & `score`).  
2. Map review scores → sentiment labels.  
3. Split dataset (80% training, 20% testing).  
4. Tokenize text with IndoBERT tokenizer.  
5. Train IndoBERT for sentiment classification.  
6. Evaluate model with classification report & confusion matrix.  
7. Visualize sentiment distribution & performance.  

---

## 📈 Results & Findings

### Confusion Matrix
The model performs well in classifying **Positive** and **Negative** reviews, but struggles with **Neutral** reviews.

![Confusion Matrix](results/confusion_matrix.png)

---

## ✅ Insights
- **Positive Reviews:** highlight *fast delivery*, *good packaging*, and *affordable prices*.  
- **Negative Reviews:** mention *slow delivery*, *app performance issues*, and *product mismatch*.  
- **Neutral Reviews:** often ambiguous and harder to classify (model misclassifies many neutral reviews).  

---

## 🎯 Conclusion & Recommendations
- Sellers should improve **delivery time** and **product quality consistency**.  
- Shopee should maintain strengths in **pricing & packaging quality**.  
- Future improvement: handle **neutral reviews** more effectively, possibly by adding more training data or using advanced sentiment techniques.  

---

## 📂 Repository Structure


## 🚀 How to Run
1. Clone repo:
   ```bash
   git clone https://github.com/your-username/Shopee-Sentiment-Analysis.git
   cd Shopee-Sentiment-Analysis

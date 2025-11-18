# 🎬 Movie Recommendation System (Hybrid Model)

## 📌 Overview
This project builds a **Hybrid Movie Recommendation System** that improves traditional rating-based recommendations by incorporating **sentiment analysis from IMDb user reviews**. It combines **TF-IDF + Naïve Bayes sentiment scoring** with **User-Based and Item-Based Collaborative Filtering**, producing more accurate and emotion-aware movie suggestions.

---

## 🔍 Key Features
- **Sentiment Analysis** using TF-IDF vectorization and Naïve Bayes classification  
- **Enhanced Ratings**: Final rating = 80% actual rating + 20% sentiment rating  
- **User-Based Collaborative Filtering** (cosine similarity)  
- **Item-Based Collaborative Filtering** for similar movie suggestions  
- **Hybrid Recommendation Score** blending user-based & item-based outputs  

---

## 🧠 Methodology
1. Clean and preprocess IMDb reviews (regex, stopwords, lemmatization)  
2. Apply TF-IDF vectorization (max 2500 features)  
3. Train Naïve Bayes model with GridSearchCV  
4. Convert sentiment probability → 1–5 rating using quantile binning  
5. Build user and item similarity matrices for collaborative filtering  
6. Combine both filtering approaches to generate final recommendations  

---

## 📊 Evaluation
- Sentiment model evaluated using **accuracy** & **confusion matrix**  
- Recommendation quality assessed using **MSE** and **MAE**  
- Hybrid approach increases personalization and accuracy  

---

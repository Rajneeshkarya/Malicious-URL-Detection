# 🚨 Malicious URL Detection using Machine Learning

This project aims to detect **malicious URLs** using a machine learning approach based on character-level feature extraction. It is designed to help prevent phishing attacks, malware distribution, and potential financial and data loss by accurately identifying harmful URLs.

## 📌 Objective

The core objective of this project is to develop a **binary classification model** capable of differentiating between legitimate and malicious URLs using a range of URL-based features. The model is intended to be lightweight, fast, and easily integrable into security systems or browser extensions.

---

## 📊 Dataset

- **Total URLs:** 11,430  
- **Malicious URLs:** 5,715  
- **Legitimate URLs:** 5,715  
- **Training Data:** 3,829 safe + 3,829 malicious  
- **Validation Data:** 1,886 safe + 1,886 malicious

---

## ⚙️ Features

The model uses several extracted features from URLs such as:

- URL Length
- Presence of IP addresses
- Top-Level Domains (TLDs)
- Special characters frequency
- Technical indicators
- WHOIS and web traffic features (if available)

---

## 🧠 Model Architecture

- **Model Used:** Random Forest Classifier  
- **Number of Trees:** 100  
- **Max Depth:** Tuned via hyperparameter optimization  
- **Criterion:** Gini impurity / Entropy

---

## 📈 Results

- **Accuracy Achieved:** **87.33%**  
- The model performs well on both training and validation datasets, indicating good generalization capability.

---

## 🛠 Methodology

### 1. Data Preprocessing
- Handled missing values
- Scaled numerical features

### 2. Feature Engineering
- Character-level analysis of URLs
- Feature selection via mutual information or recursive elimination

### 3. Model Training
- Used `RandomForestClassifier` for interpretability and performance
- Trained with balanced dataset of malicious and legitimate URLs

---

## 📌 Future Improvements

- Integrate deep learning models like CNN and RNN for sequential pattern recognition
- Add Explainable AI (XAI) components to justify decisions
- Real-time detection system integration
- Larger and more diverse dataset inclusion

---


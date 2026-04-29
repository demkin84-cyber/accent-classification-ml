# 🎙️ Accent Classification using Machine Learning

This project builds a machine learning model that predicts a speaker's accent using MFCC (Mel-frequency cepstral coefficients) audio features.

## 📊 Problem
Classify speakers into 6 accents:
- US
- UK
- Spanish
- French
- German
- Italian

## 🧠 Models Used
- Logistic Regression (baseline)
- Random Forest
- Support Vector Machine (RBF)

## ⚙️ Pipeline
1. Exploratory Data Analysis
2. Train/Test split (stratified)
3. Feature scaling
4. Model training & comparison
5. Hyperparameter tuning (GridSearchCV)
6. Feature importance analysis
7. Model saving with joblib

## 🏆 Results
Best model: **Random Forest**

Accuracy: **85%**

Key findings:
- German & Spanish accents easiest to detect
- French & Italian hardest
- US vs UK confusion due to phonetic similarity
- Dataset is class-imbalanced (US dominates)

## 💾 Saved artifacts
- `accent_model.pkl` — trained model
- `scaler.pkl` — feature scaler

## 🚀 How to run

```bash
pip install -r requirements.txt
python accent_classifier.py
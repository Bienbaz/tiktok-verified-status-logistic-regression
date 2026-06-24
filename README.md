# TikTok Verified Status Predictor

![Python](https://img.shields.io/badge/Python-3.9%2B-blue) 
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.0+-orange)
![Pandas](https://img.shields.io/badge/pandas-2.0+-blue)

**Logistic Regression model to predict whether a TikTok user is verified based on video features.**

---

## 📱 Business Context

TikTok faces a massive backlog of user reports and content moderation tasks.  
This project builds an **interpretable Logistic Regression model** to predict `verified_status` (verified vs. not verified). 

**Key Goals:**
- Achieve high Recall on the minority class (verified users)
- Help prioritize moderation for verified accounts
- Reduce manual review workload on claims vs. opinion videos

---

## 📊 Dataset

Synthetic dataset mimicking the official TikTok project dataset (~20,000 records).

**Key Features:**
- `claim_status` (claim / opinion)
- `video_transcription_text`
- `video_view_count`, `video_like_count`, `video_share_count`, etc.
- `author_ban_status`
- **Target**: `verified_status` (verified / not verified) → **94% / 6% imbalance**

---

## 🚀 Features Delivered

- Feature engineering: `text_length` from `video_transcription_text`
- Handling severe class imbalance (SMOTE / class_weight)
- Logistic Regression with hyperparameter tuning
- Confusion Matrix + Precision-Recall evaluation
- Actionable business insights for report backlog

---

## 📁 Project Structure

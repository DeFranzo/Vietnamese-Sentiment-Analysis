# 🇻🇳 Vietnamese Sentiment Classifier using PhoBERT

A production-ready sentiment analysis app for Vietnamese product reviews using [PhoBERT](https://huggingface.co/vinai/phobert-base).  
It includes a RESTful API (FastAPI) and a user-friendly web interface (Streamlit).

---

## Features

- Trained PhoBERT model for Vietnamese sentiment classification
- REST API with FastAPI (`POST /predict`)
- Web interface with Streamlit
- Evaluation script with F1, accuracy, and confusion matrix

---

## Model Overview

- **Base model**: `vinai/phobert-base`
- **Classes**: `Positive`, `Neutral`, `Negative`
- **Training time**: ~3 minutes on CPU: i5 - 10600KF /GPU: 3080TI
- **Evaluation**:  
    - Accuracy: ~87%  
    - High F1 for Positive & Negative, weaker Neutral (needs more data)

---

## Installation

cd sentiment_project/sentiment_app
pip install -r requirements.txt

## Start FastAPI

uvicorn api:app --reload

## Start Streamlit

streamlit run app.py


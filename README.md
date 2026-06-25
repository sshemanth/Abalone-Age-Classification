# 🐚 Abalone Age Classification using Computational Intelligence

An advanced Computational Intelligence (CI) framework for classifying the age of abalone. This project evaluates multiple intelligent learning paradigms—ranging from deep learning and ensemble models to interpretable neuro-fuzzy systems—using the standard Abalone dataset.

---

## 📌 Project Overview

This project implements and compares diverse machine learning and soft computing approaches to optimize classification performance while analyzing model interpretability. 

The framework evaluates:
* **Predictive Performance:** Leveraging deep neural networks and gradient boosting ensembles.
* **Fuzzy Reasoning Interpretability:** Implementing a self-constructing neuro-fuzzy pipeline to extract human-readable logic rules.

---

## 🧠 Implemented Models

The repository contains implementations for the following configurations:
1. **Baseline Feedforward Neural Network (FNN)**
2. **Advanced Deep FNN**
3. **Fixed Neuro-Fuzzy Model**
4. **XGBoost**
5. **LightGBM**
6. **CatBoost**
7. **Stacking Ensemble (Meta-Learner)**
8. **Self-Constructing Neuro-Fuzzy Inference System (SONFIN)**

---

## 🧬 Key Highlights & Features

* **SONFIN Architecture:** Automatically constructs fuzzy rules, adapts structure dynamically, and learns Gaussian membership functions from scratch during training.
* **Ensemble Learning:** High-performance stacking meta-learner that achieves a peak evaluation score of **0.808**.
* **Explainable AI (XAI):** Built-in visual plots for fuzzy membership functions, feature importances, and neural network learning curves.
* **Streamlit Web Dashboard:** Interactive real-time web application supporting manual sample evaluation and batch CSV parsing.

### Target Classification Classes
* **Class 0:** Young Abalone (Age ≤ 8)
* **Class 1:** Medium Age Abalone (Age 9–10)
* **Class 2:** Old Abalone (Age ≥ 11)

---

## 📁 Repository Structure

```text
abalone-age-classification-sonfin/
├── app.py                  # Streamlit application entry point
├── requirements.txt         # Project dependencies
├── README.md               # Project documentation
├── models/                 # Saved model weights and scalers
│   ├── xgb_model.pkl
│   ├── lgbm_model.pkl
│   ├── cat_model.pkl
│   ├── meta_model.pkl
│   ├── advanced_fnn.pth
│   └── scaler.pkl
└── notebook/               # Experimental code and training pipeline
    └── ProjectK.ipynb

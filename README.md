# 🚢 Titanic Survival Prediction Project 2025

[![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)](https://github.com/Tileli15)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

## 📌 Project Overview
This project is part of the **Applied Data Science (APDS) 2025** curriculum. It involves building a complete Machine Learning pipeline to predict passenger survival on the Titanic. The goal is to demonstrate end-to-end data processing, from raw data cleaning to model evaluation, using **Logistic Regression** and **K-Nearest Neighbors (KNN)**.

---

## 🛠️ Key Features & Workflow

### 1. 🧹 Data Cleaning & Preprocessing
- **Missing Values:** Imputed `Age` using median and `Embarked` using mode.
- **Outlier Detection:** Capped extreme outliers in `Fare` (99th percentile).
- **Data Pruning:** Removed irrelevant columns (`deck`, `embark_town`, `alive`, etc.) to reduce noise.

### 2. ⚙️ Feature Engineering
- **`FamilySize`:** Created by combining `SibSp` + `Parch` + 1.
- **`IsAlone`:** A boolean feature indicating if a passenger is travelling alone.
- **Encoding:** Applied `LabelEncoder` for binary categorical features and `One-Hot Encoding` for multi-class features.

### 3. 🤖 Machine Learning Models
- **Logistic Regression:** Used for baseline binary classification (`max_iter=500`).
- **K-Nearest Neighbors (KNN):** Implemented with `n_neighbors=5`.
- **Scaling:** Applied `StandardScaler` to ensure optimal performance for distance-based algorithms like KNN.

---

## 📊 Results & Evaluation

| Model | Accuracy | Precision (Weighted) | Recall (Weighted) | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | **81%** | 0.81 | 0.81 | 0.81 |
| **K-Nearest Neighbors** | 79% | 0.79 | 0.79 | 0.79 |

> *Note: Logistic Regression slightly outperformed KNN in this iteration, proving robust for this specific feature set.*

---

## 💻 Installation & Usage

### Prerequisites
- Python 3.11+
- Git

### 1. Clone the Repository
cd project2titanicBaloulThileli

### 2. Set Up Environment
It is recommended to use a virtual environment.

### 3. Install Dependencies
pip install -r requirements.txt

### 4. Run the Script
jupyter sulotion.ipynb

---

## 👤 Author
**Thileli Baloul**
- GitHub: [@Tileli15](https://github.com/Tileli15)

---
*Created for TP5 AP_DS 2025/2026.*

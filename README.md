# 🚀 ML Algorithm Selector (Meta-Learning Based AutoML)

This project uses **meta-learning** to automatically recommend the best machine learning algorithm for any uploaded dataset.

You simply upload a CSV file, and the system:

- extracts meta-features  
- predicts the best algorithm (RandomForest, SVM, or KNN)  
- trains the algorithm  
- returns the **accuracy score**  
- provides instant evaluation  

It is a lightweight, explainable form of **AutoML**.

---

## 📌 Features

### ✅ Meta-learning Model
A `RandomForestClassifier` trained on a synthetic meta-dataset to predict the most suitable algorithm.

### ✅ CSV Upload Interface  
Built with **Gradio** for easy dataset uploading.

### ✅ Automatic Meta-Feature Extraction  
For each uploaded dataset, the system computes:

- `n_samples` – number of rows  
- `n_features` – number of columns  
- `imbalance_ratio` – class proportion imbalance  
- `avg_corr` – average feature correlation  
- `class_sep` – class separation (placeholder for now)

### ✅ Performance Evaluation  
After recommending an algorithm, the system trains it on an **80–20 split** and reports the **accuracy**.

---

## 📁 Project Structure


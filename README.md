# 🎯 ML Assignment 2 – Data Classification

**Course:** Introduction to Machine Learning  
**University:** Alexandria National University – Faculty of Computer and Data Science  
**Due Date:** April 25, 2025  

## 📌 Objective

This assignment explores and compares various classification algorithms on the **MAGIC Gamma Telescope** dataset. The goal is to:

- Preprocess and balance an imbalanced dataset
- Train multiple classification models
- Tune hyperparameters via cross-validation
- Evaluate models using performance metrics
- Compare results and identify the best-performing classifier

---

## 🧪 Dataset

- **Source:** [UCI MAGIC Gamma Telescope Dataset](https://archive.ics.uci.edu/ml/datasets/MAGIC+Gamma+Telescope)
- **Description:** Simulated registration of high energy gamma particles using atmospheric Cherenkov imaging.
- **Classes:**
  - `g` = gamma rays (signal)
  - `h` = hadrons (background)

---

## ⚙️ Models Used

- Decision Tree Classifier
- Naive Bayes Classifier
- Random Forest Classifier (with `n_estimators` tuning)
- AdaBoost Classifier (with `n_estimators` tuning)

---

## 🔄 Preprocessing Steps

1. Load and encode the dataset
2. Balance the dataset by randomly undersampling the gamma class
3. Split into 70% training and 30% testing sets (stratified)
4. Normalize/evaluate as needed

---

## 📊 Evaluation Metrics

Each model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix (printed + heatmap)

---

## 📈 Results Summary

| Model         | Accuracy | Precision | Recall | F1-Score |
|---------------|----------|-----------|--------|----------|
| Decision Tree | ~83%     | ~0.87     | ~0.87  | ~0.87    |
| Naive Bayes   | ~73%     | ~0.73     | ~0.91  | ~0.81    |
| Random Forest | **~88%** | **0.88**  | 0.94   | **0.91** |
| AdaBoost      | ~85%     | 0.86      | **0.92** | 0.88    |

---

## 📁 Files

- `ML_Assignment2.ipynb` – Jupyter Notebook with full implementation
- `README.md` – This file
- `machine learning assignment 2_data classification report.pdf` – Summary write-up
- `ML-Assignment2.pdf` – the task 

---

## ▶️ How to Run

1. Open the notebook in Google Colab or Jupyter.
2. Run cells from top to bottom:
   - Data loading & balancing
   - Model training & tuning
   - Evaluation
3. Review printed metrics and confusion matrix heatmaps.

---

## ✅ Requirements

- Python 3.x
- Libraries:
  - `pandas`, `numpy`
  - `scikit-learn`
  - `seaborn`, `matplotlib`

Install with:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib

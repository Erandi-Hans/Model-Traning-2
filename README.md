# 🚢 Titanic Survival Prediction & Machine Learning Models Comparison

This repository contains **Day 2** of my Machine Learning journey, focusing on Supervised Learning techniques. In this project, multiple classification algorithms and a Neural Network (Multi-Layer Perceptron) were trained, evaluated, and compared on the **Titanic Dataset** to predict passenger survival.

---

## 📌 Project Overview

The primary goal of this project is to build and evaluate multiple machine learning models to solve a binary classification problem (predicting whether a passenger survived or died). Detailed preprocessing, feature engineering, and model evaluation metrics (Accuracy, Precision, Recall, and F1-Score) are included to identify the top-performing model.

---

## 🚀 Key Steps & Workflow

1. **Data Preprocessing & Cleaning:**
   - Handled missing values (imputed `age` with median, `embarked` with mode).
   - Encoded categorical features (`sex` mapped to binary, `embarked` using One-Hot Encoding).
   - Feature Scaling using `StandardScaler` for distance-based and gradient-based models (KNN, Logistic Regression, MLP).

2. **Model Training & Evaluation:**
   Trained and tested the following classification models:
   - **Logistic Regression**
   - **Decision Tree Classifier**
   - **Random Forest Classifier**
   - **K-Nearest Neighbors (KNN)** *(Tuned for optimal $K$)*
   - **Multi-Layer Perceptron (MLP) Classifier**

3. **Performance Metrics:**
   - Evaluated models using Accuracy, Precision, Recall, and F1-Score.
   - Generated Confusion Matrices and Feature Importance Visualizations.

---

## 📊 Model Performance Comparison

Below is the scorecard comparing all trained models on the test set, ordered by **F1-Score**:

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **KNN ($K=7$)** | **0.821** | **0.785** | **0.739** | **0.761** |
| **KNN ($K=14$)** | 0.827 | 0.865 | 0.652 | 0.744 |
| **Logistic Regression** | 0.804 | 0.793 | 0.667 | 0.724 |
| **Neural Network (MLP)** | 0.782 | 0.734 | 0.681 | 0.707 |
| **Random Forest** | 0.804 | 0.870 | 0.580 | 0.696 |
| **Decision Tree** | 0.777 | 0.754 | 0.623 | 0.683 |

---

## 🏆 Key Insights & Takeaways

* **Top Performing Model:** **K-Nearest Neighbors ($K=7$)** achieved the highest overall **F1-Score (0.761)** with a balanced trade-off between Precision and Recall.
* **Feature Importance:** Across tree-based models (Decision Trees & Random Forest), **Sex** and **Passenger Class (Pclass)** emerged as the most critical predictors of survival.
* **Scaling Matters:** Distance-sensitive models like KNN and Neural Networks showed significant improvements when features were scaled using `StandardScaler`.

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python 3.13
* **Libraries Used:**
  * `pandas` & `numpy` - Data Manipulation & Analysis
  * `matplotlib` & `seaborn` - Data Visualization
  * `scikit-learn` - Model Building, Preprocessing, & Evaluation

---

## 📅 Roadmap / Next Steps

- [x] **Day 1:** Data Preprocessing & Exploratory Data Analysis (EDA)
- [x] **Day 2:** Model Training & Comparative Evaluation (Classification, Regression & Neural Networks)
- [ ] **Day 3:** Hyperparameter Tuning, Introduction to NLP, and Model Deployment

---

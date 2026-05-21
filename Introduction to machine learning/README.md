# Introduction to Machine Learning — A Beginner's Course

**Based on:** *An Introduction to Statistical Learning with Applications in Python* (ISLP, 2023)
**Designed for:** Complete beginners — no prior machine learning knowledge required
**Language:** Python 3.x

---

## What This Course Is

This is a self-paced, hands-on introduction to machine learning. Each chapter contains:

- 📖 **README.md** — A simplified teaching course with plain-language explanations, everyday analogies, worked examples, and Python code
- 📝 **exercises.md** — Practice problems ranging from conceptual questions to coding challenges
- ✅ **solutions/solutions.md** — Detailed, explained answers to every exercise
- 🐍 **solutions/main.py** — Runnable Python code for all coding exercises

The materials are inspired by the structure of the ISLP textbook but written in accessible language for learners who have never encountered machine learning.

---

## Prerequisites

You do not need a mathematics or computer science background. However, you will benefit from:

- Basic Python knowledge (variables, loops, functions, importing libraries)
- Familiarity with spreadsheets or tables (data has rows and columns)
- Curiosity!

**Python libraries used** (install with `pip install`):
```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```

---

## Course Map

| Chapter | Topic | Key Concepts |
|---------|-------|-------------|
| [Chapter 1](chapter_01_what_is_ml/) | What Is Machine Learning? | Types of ML, the ML workflow, features and labels |
| [Chapter 2](chapter_02_statistical_learning/) | Statistical Learning | How models learn, bias-variance trade-off, train vs. test error |
| [Chapter 3](chapter_03_linear_regression/) | Linear Regression | Predicting numbers, R², coefficients, dummy variables |
| [Chapter 4](chapter_04_classification/) | Classification | Logistic regression, confusion matrix, precision/recall, KNN |
| [Chapter 5](chapter_05_resampling_methods/) | Resampling Methods | Cross-validation, bootstrap, honest model evaluation |
| [Chapter 6](chapter_06_model_selection_regularization/) | Model Selection & Regularization | Ridge, Lasso, feature selection, scaling |
| [Chapter 7](chapter_07_tree_based_methods/) | Tree-Based Methods | Decision trees, Random Forests, Gradient Boosting |
| [Chapter 8](chapter_08_support_vector_machines/) | Support Vector Machines | Hyperplanes, margin, kernels, grid search |
| [Chapter 9](chapter_09_deep_learning/) | Deep Learning | Neural networks, backpropagation, CNNs, RNNs |
| [Chapter 10](chapter_10_unsupervised_learning/) | Unsupervised Learning | K-Means clustering, hierarchical clustering, PCA |

---

## How to Use This Course

### Recommended Path for Complete Beginners

1. **Read the README.md** in order from Chapter 1. Do not skip — each chapter builds on the previous.
2. **Work through exercises.md** on your own before looking at solutions.
3. **Check solutions/solutions.md** and run **solutions/main.py** to verify your code.
4. **Experiment** — modify the code examples, try different parameters, break things deliberately.

### If You Have Some Experience

- Chapter 1–2 are foundational concepts — skim if you already know them.
- Chapter 3–4 introduce the first hands-on models — work through these carefully.
- Chapters 5–10 can be read in any order once you have Chapters 1–4 under your belt.

---

## Key Principles to Keep in Mind

1. **Always split your data.** Never evaluate a model on training data alone — use a test set or cross-validation.
2. **Scale your features** before distance-based methods (KNN, SVM, Ridge, Lasso, neural networks, K-Means, PCA).
3. **Start simple.** Try logistic regression or a decision tree before jumping to neural networks.
4. **Understand your metric.** Accuracy is not always the right measure — consider precision, recall, and F1.
5. **Avoid data leakage.** The test set must not influence any training decision.
6. **Model selection is iterative.** Your first model is almost never your final model.

---

## After This Course

Once you have completed all 10 chapters, you are ready to:

- Work through the **ISLP textbook** (available in the same folder as `ISLP_website.pdf`) for deeper mathematical foundations
- Explore **Kaggle** (kaggle.com) for real-world datasets and competitions
- Learn **Pandas and NumPy** more deeply for data wrangling
- Study **feature engineering** — transforming raw data into better features
- Explore advanced topics: time series, NLP, Transformers, reinforcement learning

---

## Quick Reference: Which Algorithm Should I Use?

| Your goal | Start with |
|-----------|-----------|
| Predict a number | Linear Regression |
| Predict a category (2 classes) | Logistic Regression |
| Predict a category (many classes) | Logistic Regression or Random Forest |
| Find natural groups in data | K-Means Clustering |
| Understand which features matter | Random Forest (feature importances) |
| High accuracy on tabular data | Gradient Boosting |
| Image recognition | CNN (Convolutional Neural Network) |
| Text analysis | TF-IDF + Logistic Regression, or LSTM/Transformer |
| Compress or visualise high-dimensional data | PCA |
| Evaluate any model honestly | Cross-Validation |

---

*Good luck, and enjoy the journey into machine learning!*

# Homework 1 — Linear Regression: Closed-form vs Gradient Descent

## 👤 Student Info
- **Name:** Phani Pallavi Tallavajjhala  
- **Student ID:** 700766070 

---

## 📌 Overview
This assignment covers both theory and programming tasks for Linear Regression, including function approximation, random guessing, gradient descent, and recognizing underfitting/overfitting. It also compares the **Closed-form (Normal Equation)** and **Gradient Descent** methods on synthetic data.

---

## 🗂 Repository Contents
- `Homework1_LinearRegression.ipynb` — Jupyter Notebook with dataset generation, closed-form, and GD implementation.
- `synthetic_data.csv` — synthetic dataset (200 samples, x ∈ [0,5], y = 3 + 4x + ε).
- `ML ASSIGNMENT_1.txt` — written answers for Questions 1–6 (theory tasks).
- `linear_regression_fits.png` — plot showing raw data points + both fitted lines.
- `gd_loss_curve.png` — plot showing GD loss vs iterations.

---

## ▶️ How to Run

### Option A — Jupyter Notebook
1. Open `Homework1_LinearRegression.ipynb` in Jupyter.
2. Run all cells in order to generate data, fit both models, and display plots.

### Option B — Python Script
If you have a script version (`hw1_linear_regression.py`):
```bash
python hw1_linear_regression.py
```
This will print estimated parameters and save plots.

---

## 📊 Results (Sample Run)
- **Closed-form solution:** intercept ≈ 2.69, slope ≈ 4.13  
- **Gradient Descent (η=0.05, 1000 iters):** intercept ≈ 2.69, slope ≈ 4.13  
- **Loss curve:** decreases smoothly and stabilizes by ~1000 iterations  

The fitted lines overlap visually, confirming that GD converged to the same solution as the Normal Equation.

---

## 📝 Short Explanation
The Normal Equation computes the exact least-squares solution directly. Gradient Descent starts from [0,0] and reduces error iteratively using the slope of the cost function. With η=0.05 for 1000 iterations, GD converges to nearly the same intercept and slope as the closed-form method, as shown by the overlapping lines and decreasing loss.

---

## 💡 Notes
- All code is **commented** for clarity.  
- Theory answers are included in `ML ASSIGNMENT_1.txt`.  

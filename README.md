Forward Selection in Regression Modeling using BIC
A regression modeling project using Forward Selection with Bayesian Information Criterion (BIC) to select the most significant predictor from a dataset with 6 variables and 31 observations.


# 📊 Forward Selection in Regression Modeling using BIC

This project demonstrates how to apply **Forward Selection**, a stepwise regression technique, to identify the most significant predictor in a dataset. The model selection is guided by the **Bayesian Information Criterion (BIC)**, which helps prevent overfitting, especially in small datasets.

---

## ✅ Objective

To apply forward selection on a dataset with 6 predictors and 31 observations, and identify the most impactful predictor for the target variable `y`.

---

## 🔍 About Forward Selection

Forward Selection is a greedy algorithm that begins with an empty model and adds variables one at a time based on a criterion like AIC, BIC, or p-value. In our case, **BIC** is used due to its penalty for complexity — ideal for smaller datasets.

---

## 🧮 Dataset Overview

- **Target Variable (y)**: A continuous variable representing the outcome.
- **Predictors**:
  - `x1`, `x2`, `x3`: Continuous numeric features
  - `x4`: Binary categorical variable (0 or 1)
  - `x5`, `x6`: Continuous numeric features

31 total observations were used.

---

## 🧠 Tools & Language

- **Language**: R
- **Techniques**: Linear Regression, Forward Selection
- **Model Selection**: `step()` function with `direction = "forward"` and `k = log(n)` for BIC.

---

## ⚙️ Steps Performed

1. **Create Full and Null Models**:
   - Full model includes all predictors.
   - Null model includes only the intercept.

2. **Run Forward Selection**:
   - Added predictors one by one based on improvement in BIC.
   - Stopped when no further reduction in BIC was observed.

3. **Final Model**:
   - Selected predictor: `x4`
   - Final regression equation:
     ```
     y = 11.72 - 10.77 * x4
     ```

---
👉 [![image](https://github.com/user-attachments/assets/9883fe38-31d9-49ee-b6ab-e1fd1dbeab86)

## 🧾 Interpretation

- **x4** had the most significant negative effect on `y`.
- None of the other predictors improved the BIC enough to be included.
- The model favors simplicity and generalization.

---

## 👥 Team Members

| Name              | ID           |
|-------------------|--------------|
| NATENAEL BEKELE   | DBU1501407   |
| HAFIZE HUSEN      | DBU1501241   |
| REDIET ESUBALEW   | DBU1501704   |
| BEREKET GETAW     | DBU1501044   |
| DAWIT ALEMU       | DBU1501117   |
| YIFERU MEKONEN    | DBU1501562   |
| ELBETEL ABEDI     | DBU1501145   |
| GENET MINDA       | DBU1501217   |

---

## 📌 Conclusion

Forward Selection using BIC resulted in a simple, interpretable model with strong predictive power using only one predictor. This approach avoids overfitting and highlights the strength of BIC in variable selection.

---

## 📜 License

This project is for academic and educational purposes.

> 🎓 *Debre Berhan University — Data Science Department, 2025*

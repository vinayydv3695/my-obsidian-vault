

---

# 📌 Evaluation Metrics for Regression Models

_(MSE, RMSE, R², Adjusted R² — Detailed Notes)_

## 1. Introduction

Regression models are evaluated using metrics that measure:

- Error in prediction
    
- Goodness of fit
    
- How well the model generalizes
    

The most common metrics are:

- **MSE (Mean Squared Error)**
    
- **RMSE (Root Mean Squared Error)**
    
- **MAE (Mean Absolute Error)**
    
- **R² (Coefficient of Determination)**
    
- **Adjusted R²**
    

---

# 📌 2. MSE — Mean Squared Error

## **Definition**

MSE measures the **average squared difference** between predicted and actual values.

```
MSE = (1/n) * Σ (Yi − Ŷi)²
```

## **Interpretation**

- Lower MSE = better model
    
- Penalizes **large errors heavily** due to squaring
    
- Sensitive to outliers
    

## **When to use?**

Use when:

- Large errors must be penalized
    
- Outlier effect is acceptable
    

---

# 📌 3. RMSE — Root Mean Squared Error

## **Definition**

RMSE is the **square root of MSE**.

```
RMSE = √MSE
```

## **Interpretation**

- Most commonly used regression metric
    
- Has the **same units** as the target variable
    
- Easier to interpret than MSE
    

## **When to use?**

- When original units matter (e.g., dollars, meters, temperature)
    
- When you want to penalize large errors
    

---

# 📌 4. R² — Coefficient of Determination

## **Definition**

R² measures the **proportion of variance in Y explained by X**.

```
R² = 1 − (SS_res / SS_tot)
```

Where:

- SS_res = Σ (Yi − Ŷi)² → residual sum of squares
    
- SS_tot = Σ (Yi − Ȳ)² → total variation
    

## **Interpretation**

- R² = 1 → perfect prediction
    
- R² = 0 → model predicts no better than mean
    
- R² < 0 → model worse than horizontal line
    

R² increases when more predictors are added (even useless ones).

---

# 📌 5. Adjusted R²

## **Definition**

Adjusted R² penalizes adding irrelevant predictors.

```
Adjusted R² = 1 − [(1 − R²)(n − 1) / (n − k − 1)]
```

Where:

- n = samples
    
- k = number of predictors
    

## **Interpretation**

- Increases only when added variable improves the model
    
- Better metric than R² for **multiple regression**
    

---

# 📌 6. Which Metric to Use?

|Scenario|Best Metric|
|---|---|
|Interpretability needed|RMSE|
|Large errors must be penalized|MSE / RMSE|
|Compare models with different number of predictors|Adjusted R²|
|Measure variance explained|R²|
|Presence of outliers|MAE|

---

# 📌 Regression Metrics — MCQs (20)

All MCQs include **question, options, and visible answer**.

---

## **MCQ 1**

**Question:** MSE measures:

-  Absolute error
    
-  Classification accuracy
    
-  Squared error
    
-  Linear error
    

**Answer:** Squared error

---

## **MCQ 2**

**Question:** RMSE is the:

-  Square of MSE
    
-  Square root of MSE
    
-  Log of MSE
    
-  Reciprocal of MSE
    

**Answer:** Square root of MSE

---

## **MCQ 3**

**Question:** The unit of RMSE is:

-  Squared unit
    
-  No unit
    
-  Same as target variable
    
-  Percentage
    

**Answer:** Same as target variable

---

## **MCQ 4**

**Question:** R² represents:

-  Error percentage
    
-  Fraction of variance explained
    
-  Total error
    
-  Model complexity
    

**Answer:** Fraction of variance explained

---

## **MCQ 5**

**Question:** If R² = 1, the model is:

-  Underfitting
    
-  Perfect
    
-  Poor
    
-  Random
    

**Answer:** Perfect

---

## **MCQ 6**

**Question:** R² < 0 means:

-  Overfitting
    
-  Better than the mean
    
-  Worse than predicting the mean
    
-  Error is zero
    

**Answer:** Worse than predicting the mean

---

## **MCQ 7**

**Question:** Adjusted R²:

-  Always equals R²
    
-  Can decrease when adding predictors
    
-  Always increases
    
-  Does not depend on predictors
    

**Answer:** Can decrease when adding predictors

---

## **MCQ 8**

**Question:** Which metric penalizes large errors most heavily?

-  MAE
    
-  R²
    
-  Adjusted R²
    
-  MSE
    

**Answer:** MSE

---

## **MCQ 9**

**Question:** RMSE is preferred over MSE because:

-  It inflates error
    
-  It is harder to compute
    
-  It has interpretable units
    
-  It doesn't penalize outliers
    

**Answer:** It has interpretable units

---

## **MCQ 10**

**Question:** MSE has units of:

-  Original units
    
-  Squared units
    
-  No units
    
-  Logarithmic units
    

**Answer:** Squared units

---

## **MCQ 11**

**Question:** R² improves when:

-  Irrelevant variables are added
    
-  Errors increase
    
-  Residual sum of squares increases
    
-  Predictions become worse
    

**Answer:** Irrelevant variables are added

---

## **MCQ 12**

**Question:** Best metric to compare two multiple regression models is:

-  R²
    
-  Accuracy
    
-  Entropy
    
-  Adjusted R²
    

**Answer:** Adjusted R²

---

## **MCQ 13**

**Question:** Which metric cannot decrease after adding more predictors?

-  Adjusted R²
    
-  MSE
    
-  RMSE
    
-  R²
    

**Answer:** R²

---

## **MCQ 14**

**Question:** A model with high MSE indicates:

-  Excellent prediction
    
-  Poor prediction
    
-  Perfect fit
    
-  Balanced model
    

**Answer:** Poor prediction

---

## **MCQ 15**

**Question:** RMSE penalizes:

-  Small errors
    
-  Outliers heavily
    
-  Correct predictions
    
-  Missing values
    

**Answer:** Outliers heavily

---

## **MCQ 16**

**Question:** Which metric shows how much variance is left unexplained?

-  1 − R²
    
-  RMSE
    
-  MSE
    
-  R²
    

**Answer:** 1 − R²

---

## **MCQ 17**

**Question:** A negative R² indicates:

-  The model is perfect
    
-  A normal condition
    
-  Severe model failure
    
-  Overfitting
    

**Answer:** Severe model failure

---

## **MCQ 18**

**Question:** Adjusted R² corrects R² by penalizing:

-  Large residuals
    
-  Small datasets
    
-  Adding irrelevant predictors
    
-  Non-linearity
    

**Answer:** Adding irrelevant predictors

---

## **MCQ 19**

**Question:** Which metric is best when units matter?

-  MAE
    
-  R²
    
-  Adjusted R²
    
-  RMSE
    

**Answer:** RMSE

---

## **MCQ 20**

**Question:** If the model has RMSE = 0, it means:

-  Normal prediction
    
-  Poor performance
    
-  Zero error (perfect predictions)
    
-  Overfitting always
    

**Answer:** Zero error (perfect predictions)

---

If you want next:  
✔ **Classification evaluation metrics (Accuracy, Precision, Recall, F1, ROC–AUC)**  
✔ **PCA / K-Means notes + MCQs**  
✔ Full **exam revision sheet** for Machine Learning (Obsidian-formatted)

Just tell me!
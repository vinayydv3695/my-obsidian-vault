
---

# 📌 Simple Linear Regression (SLR)

## 1. Introduction

Simple Linear Regression models the relationship between:

- One **independent variable (X)**
    
- One **dependent variable (Y)**
    

Goal:

> Fit a straight line that best predicts Y from X.

---

## 2. Equation of the Regression Line

```
Y = β₀ + β₁X + ε
```

Where:

- β₀ = intercept
    
- β₁ = slope
    
- ε = error term
    

---

## 3. Interpretation

- β₁: Change in Y for one-unit change in X
    
- β₀: Value of Y when X = 0
    

---

## 4. Cost Function — Least Squares

Regression minimizes **Sum of Squared Errors (SSE)**:

```
SSE = Σ (Yᵢ − Ŷᵢ)²
```

Ordinary Least Squares (OLS) finds β₀, β₁ that minimize SSE.

---

## 5. Assumptions

- Linearity
    
- Independence of errors
    
- Homoscedasticity (constant variance)
    
- Normality of residuals
    

---

## 6. Evaluation Metrics

- **R² (Coefficient of Determination)**
    
- **Adjusted R²** (only for multiple regression)
    
- MAE, MSE, RMSE
    

---

# 📌 Multiple Linear Regression (MLR) 

## 1. Introduction

Multiple Regression extends SLR to **two or more predictors**.

```
Y = β₀ + β₁X₁ + β₂X₂ + ... + βₙXₙ + ε
```

---

## 2. Interpretation of Coefficients

- βᵢ describes change in Y for a unit change in Xi **holding other variables constant**.
    

---

## 3. Assumptions (Same as SLR + extra concerns)

- Linearity
    
- Independence
    
- Homoscedasticity
    
- Normality
    
- **No multicollinearity**
    
- No autocorrelation (for time series)
    

---

## 4. Multicollinearity

Occurs when predictors are highly correlated.

Detected using:

- VIF (Variance Inflation Factor)
    

Effects:

- Unstable coefficients
    
- Inflated standard errors
    

---

## 5. Advantages

- More accurate predictions
    
- Ability to model complex relationships
    
- Quantifies importance of multiple factors
    

---

## 6. Disadvantages

- Sensitive to multicollinearity
    
- Requires large sample size
    
- Difficult to interpret with many predictors
    

---

# 📌 MCQs (20) — Simple & Multiple Linear Regression

Each question → options → **visible answer**.

---

## **MCQ 1**

**Question:** Simple Linear Regression models the relationship between:

-  Multiple X and multiple Y
    
-  One X and one Y
    
-  Multiple X and one Y
    
-  No variables
    

**Answer:** One X and one Y

---

## **MCQ 2**

**Question:** The SLR equation is:

-  Y = β₀ + β₁X₁ + β₂X₂
    
-  Y = mX² + c
    
-  Y = β₀ + β₁X
    
-  X = β₀ + β₁Y
    

**Answer:** Y = β₀ + β₁X

---

## **MCQ 3**

**Question:** Which metric is minimized in linear regression?

-  Cross entropy
    
-  Hinge loss
    
-  SSE (Sum of Squared Errors)
    
-  Gini impurity
    

**Answer:** SSE (Sum of Squared Errors)

---

## **MCQ 4**

**Question:** β₁ in SLR represents:

-  Intercept
    
-  Mean of Y
    
-  Error term
    
-  Slope
    

**Answer:** Slope

---

## **MCQ 5**

**Question:** R² in regression measures:

-  Non-linearity
    
-  Accuracy
    
-  Variance explained by the model
    
-  Mean error
    

**Answer:** Variance explained by the model

---

## **MCQ 6**

**Question:** Multiple Linear Regression includes:

-  One predictor
    
-  No predictors
    
-  Two or more predictors
    
-  Only categorical predictors
    

**Answer:** Two or more predictors

---

## **MCQ 7**

**Question:** An assumption **unique** to multiple regression is:

-  Linearity
    
-  Homoscedasticity
    
-  Normality
    
-  No multicollinearity
    

**Answer:** No multicollinearity

---

## **MCQ 8**

**Question:** High multicollinearity causes:

-  Lower R²
    
-  Better model
    
-  Unstable coefficients
    
-  Faster computation
    

**Answer:** Unstable coefficients

---

## **MCQ 9**

**Question:** Which metric accounts for multiple predictors?

-  R²
    
-  F1 score
    
-  AUC
    
-  Adjusted R²
    

**Answer:** Adjusted R²

---

## **MCQ 10**

**Question:** Residuals should follow which distribution?

-  Uniform
    
-  Poisson
    
-  Gaussian (Normal)
    
-  Exponential
    

**Answer:** Gaussian (Normal)

---

## **MCQ 11**

**Question:** Homoscedasticity means:

-  Errors have constant variance
    
-  Errors increase over time
    
-  Errors must be zero
    
-  X must be normally distributed
    

**Answer:** Errors have constant variance

---

## **MCQ 12**

**Question:** The purpose of the error term ε is to:

-  Remove X
    
-  Add noise intentionally
    
-  Capture unexplained variation
    
-  Increase R²
    

**Answer:** Capture unexplained variation

---

## **MCQ 13**

**Question:** Which method is used to estimate regression coefficients?

-  Bagging
    
-  Bayesian estimation
    
-  Random forests
    
-  Ordinary Least Squares
    

**Answer:** Ordinary Least Squares

---

## **MCQ 14**

**Question:** When R² = 1:

-  Model is perfect
    
-  Model has no fit
    
-  Coefficients are zero
    
-  Errors are random
    

**Answer:** Model is perfect

---

## **MCQ 15**

**Question:** Including irrelevant features in MLR leads to:

-  Better predictions
    
-  Lower variance
    
-  More stable coefficients
    
-  Overfitting
    

**Answer:** Overfitting

---

## **MCQ 16**

**Question:** Which diagnostic helps detect multicollinearity?

-  Gini score
    
-  VIF
    
-  MSE
    
-  Entropy
    

**Answer:** VIF

---

## **MCQ 17**

**Question:** Multiple regression is useful when:

-  One variable explains all variation
    
-  Data is categorical only
    
-  Many factors influence Y
    
-  No relationship exists
    

**Answer:** Many factors influence Y

---

## **MCQ 18**

**Question:** A low R² value indicates:

-  Strong linear relationship
    
-  Weak explanatory power
    
-  Perfect predictions
    
-  Overfitting
    

**Answer:** Weak explanatory power

---

## **MCQ 19**

**Question:** Regression assumes the relationship between X and Y is:

-  Non-linear
    
-  Random
    
-  Linear
    
-  Exponential
    

**Answer:** Linear

---

## **MCQ 20**

**Question:** Adding more predictors always:

-  Increases R²
    
-  Decreases R²
    
-  Keeps R² unchanged
    
-  Fixes multicollinearity
    

**Answer:** Increases R² (but may not improve the model)

---

If you want next, I can generate:  
✔ **Logistic vs Linear Regression comparison sheet**  
✔ **SVM notes + MCQs**  
✔ **K-Means clustering notes + MCQs**  
✔ A full **Unit-wise revision sheet for your exam**

Just tell me!
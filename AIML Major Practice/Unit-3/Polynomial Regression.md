
## 1. Introduction

Polynomial Regression is an extension of Linear Regression that models **non-linear relationships** between X and Y by adding **polynomial terms**.

Example:  
A linear model cannot fit curves, but polynomial regression can.

---

## 2. Polynomial Regression Model

### **General equation:**

```
Y = β₀ + β₁X + β₂X² + β₃X³ + ... + βₙXⁿ + ε
```

Where:

- β₀, β₁, … βₙ → coefficients
    
- n → degree of polynomial
    
- ε → error term
    

---

## 3. Why Polynomial Regression?

Use it when:

- Relationship between X and Y is **curved**, not linear
    
- A linear model underfits the data
    

Polynomial regression keeps the model **linear in parameters** but **non-linear in X**.

---

## 4. How It Works

1. Start with predictor X
    
2. Create polynomial features: X², X³, …, Xⁿ
    
3. Apply **Linear Regression** on these expanded features
    
4. The line bends according to polynomial degree
    

---

## 5. Degree Selection

- **Degree too low → underfitting**
    
- **Degree too high → overfitting**
    

Common approach:

- Use **Cross-Validation**
    
- Try degrees 1, 2, 3, … and choose the best
    

---

## 6. Overfitting Issue

Higher-degree polynomials can create extreme curves, leading to poor generalization.

---

## 7. Regularization

To prevent overfitting:

- Use **Ridge Regression (L2)**
    
- Use **Lasso Regression (L1)**
    

These shrink polynomial coefficients.

---

## 8. Evaluation Metrics

Same as Linear Regression:

- R²
    
- Adjusted R²
    
- MSE, RMSE
    

Adjusted R² is important because adding more polynomial terms always increases R² artificially.

---

## 9. Applications

- Growth curve modeling
    
- Trend analysis
    
- Population forecasting
    
- Non-linear scientific models
    

---

# 📌 Polynomial Regression 



---

## **MCQ 1**

**Question:** Polynomial Regression is used when the relationship between X and Y is:

-  Linear
    
-  Random
    
-  Categorical
    
-  Non-linear
    

**Answer:** Non-linear

---

## **MCQ 2**

**Question:** Polynomial Regression is:

-  Non-linear in parameters
    
-  Linear in parameters
    
-  Unsupervised
    
-  Based on clustering
    

**Answer:** Linear in parameters

---

## **MCQ 3**

**Question:** The equation of a degree-2 polynomial regression includes:

-  Only X
    
-  X and X³
    
-  X² and X³
    
-  X and X²
    

**Answer:** X and X²

---

## **MCQ 4**

**Question:** Adding higher-degree polynomial terms can lead to:

-  Underfitting
    
-  No change
    
-  Overfitting
    
-  Linear models
    

**Answer:** Overfitting

---

## **MCQ 5**

**Question:** Polynomial regression still uses which algorithm for fitting?

-  Logistic regression
    
-  KNN
    
-  Linear regression (OLS)
    
-  SVM
    

**Answer:** Linear regression (OLS)

---

## **MCQ 6**

**Question:** A polynomial of degree 1 becomes:

-  Quadratic model
    
-  Underfitted model
    
-  Logistic model
    
-  Simple Linear Regression
    

**Answer:** Simple Linear Regression

---

## **MCQ 7**

**Question:** If a model has too few polynomial terms, it will:

-  Overfit
    
-  Show perfect accuracy
    
-  Underfit
    
-  Become random
    

**Answer:** Underfit

---

## **MCQ 8**

**Question:** Which metric should be used to compare polynomial models with different numbers of predictors?

-  Accuracy
    
-  Gini index
    
-  Adjusted R²
    
-  Recall
    

**Answer:** Adjusted R²

---

## **MCQ 9**

**Question:** Polynomial regression creates:

-  New samples
    
-  New target variables
    
-  Higher-order features
    
-  Clusters
    

**Answer:** Higher-order features

---

## **MCQ 10**

**Question:** Regularization techniques used with polynomial regression include:

-  Dropout
    
-  K-means
    
-  Ridge and Lasso
    
-  Naive Bayes
    

**Answer:** Ridge and Lasso

---

## **MCQ 11**

**Question:** Polynomial regression assumes that errors follow:

-  Exponential distribution
    
-  Binomial distribution
    
-  Normal distribution
    
-  Uniform distribution
    

**Answer:** Normal distribution

---

## **MCQ 12**

**Question:** A degree-3 polynomial model is also called:

-  Linear model
    
-  Exponential model
    
-  Cubic model
    
-  Logistic model
    

**Answer:** Cubic model

---

## **MCQ 13**

**Question:** Which technique helps select the optimal polynomial degree?

-  Gradient descent
    
-  Cross-validation
    
-  Backpropagation
    
-  PCA
    

**Answer:** Cross-validation

---

## **MCQ 14**

**Question:** Polynomial regression is sensitive to extreme values because:

-  It is supervised
    
-  It uses entropy
    
-  High-degree polynomials exaggerate outliers
    
-  It uses decision trees
    

**Answer:** High-degree polynomials exaggerate outliers

---

## **MCQ 15**

**Question:** Polynomial Regression is usually applied when the data shows:

-  A straight-line pattern
    
-  No visible trend
    
-  A curved trend
    
-  Random variation
    

**Answer:** A curved trend

---

## **MCQ 16**

**Question:** Increasing polynomial degree always increases:

-  R²
    
-  Model accuracy
    
-  Interpretability
    
-  Robustness
    

**Answer:** R²

---

## **MCQ 17**

**Question:** The polynomial regression model adds complexity by adding:

-  More targets
    
-  Hidden layers
    
-  Interaction terms
    
-  Powers of X (X², X³, etc.)
    

**Answer:** Powers of X (X², X³, etc.)

---

## **MCQ 18**

**Question:** What prevents polynomial regression from overfitting?

-  Infinite degree models
    
-  Extra noise
    
-  L1/L2 regularization
    
-  Decision tree pruning
    

**Answer:** L1/L2 regularization

---

## **MCQ 19**

**Question:** Polynomial features are generated by:

-  Splitting trees
    
-  Squaring and cubing input variables
    
-  Normalizing target variables
    
-  Removing variance
    

**Answer:** Squaring and cubing input variables

---

## **MCQ 20**

**Question:** Polynomial regression belongs to which family of algorithms?

-  Clustering
    
-  Tree-based
    
-  Non-parametric
    
-  Regression
    

**Answer:** Regression

---




---

# Logistic Regression

## 1. Introduction

- Logistic Regression is a **classification algorithm**, not a regression algorithm.
    
- Used when the **target variable is categorical**, typically **binary (0/1)**.
    
- Models the **probability** that a given input belongs to class 1.
    

---

## 2. Why Logistic Regression?

- Linear Regression fails for classification because:
    
    - Predictions may be **<0 or >1**.
        
    - Not suitable for probabilistic interpretation.
        
- Logistic Regression fixes this by using the **Sigmoid function**.
    

---

## 3. Sigmoid Function

The sigmoid (logistic) function maps any real number into a probability between 0 and 1.

**Formula:**

```
σ(z) = 1 / (1 + e^(-z))
```

Where:

```
z = β₀ + β₁x₁ + β₂x₂ + ... + βₙxₙ
```

---

## 4. Hypothesis Function (Prediction)

Logistic Regression predicts probability of class 1:

```
h(x) = σ(z) = 1 / (1 + e^(- (β₀ + β₁x₁ + ... + βₙxₙ)))
```

Decision rule:

```
If h(x) ≥ 0.5 → predict 1
Else → predict 0
```

---

## 5. Odds and Log-Odds

- **Odds** of an event:
    

```
Odds = p / (1 - p)
```

- **Log-Odds (Logit Transformation):**
    

```
log(p / (1 - p)) = β₀ + β₁x₁ + ... + βₙxₙ
```

Interpretation:

- Each βᵢ shows how a unit increase in xᵢ affects the log-odds of the outcome.
    

---

## 6. Loss Function — Binary Cross Entropy

We want to minimize the **cost function**:

```
Cost(h(x), y) = - [y * log(h(x)) + (1 - y) * log(1 - h(x))]
```

For all training samples:

```
J(β) = (1/m) * Σ [ -yᵢ log(h(xᵢ)) - (1 - yᵢ) log(1 - h(xᵢ)) ]
```

---

## 7. Optimization — Gradient Descent

Gradient descent updates parameters:

```
βⱼ = βⱼ - α * ∂J/∂βⱼ
```

Where α = learning rate.

---

## 8. Evaluation Metrics

Logistic Regression is evaluated using:

- Accuracy
    
- Precision
    
- Recall
    
- F1 score
    
- ROC Curve
    
- AUC (Area Under Curve)
    
- Confusion Matrix
    

---

## 9. Regularization

Used to prevent overfitting:

### L2 Regularization (Ridge)

```
J_reg = J + λ * Σ βⱼ²
```

### L1 Regularization (Lasso)

```
J_reg = J + λ * Σ |βⱼ|
```

---

## 10. Advantages

- Simple and fast.
    
- Outputs **probabilities**.
    
- Works well for **linearly separable** data.
    
- Less prone to overfitting with regularization.
    

---

## 11. Limitations

- Assumes linear relationship between features and log-odds.
    
- Not suitable for complex, non-linear datasets.
    
- Sensitive to multicollinearity.
    

---

Here are **20 MCQs on Logistic Regression** in **perfect Obsidian format** (checkboxes + bold correct option).

---

Got it — **Obsidian does NOT show bold inside checkboxes**, so the correct answer becomes invisible.

Here is the **fixed Obsidian-friendly format**:  
✔ MCQs with **normal checkboxes**  
✔ **Correct answer shown separately below each question** (fully visible in Obsidian)

---

You’re right — I removed the actual question lines in that version. My bad. Here are **all 20 MCQs** corrected: each item includes the **question**, the **options (checkbox style)**, and the **visible answer** — ready to paste into Obsidian.

---

# Logistic Regression — MCQs (20) 

---

## **MCQ 1**

**Question:** Logistic Regression is mainly used for:

-  Regression tasks
    
-  Clustering
    
-  Dimensionality reduction
    
-  Classification tasks
    

**Answer:** Classification tasks

---

## **MCQ 2**

**Question:** Logistic Regression outputs:

-  Continuous values
    
-  Distances
    
-  Clusters
    
-  Probabilities
    

**Answer:** Probabilities

---

## **MCQ 3**

**Question:** The activation function used in Logistic Regression is:

-  ReLU
    
-  Tanh
    
-  Softmax
    
-  Sigmoid
    

**Answer:** Sigmoid

---

## **MCQ 4**

**Question:** The sigmoid function squashes input into which interval?

-  (−∞, ∞)
    
-  (−1, 1)
    
-  (0, ∞)
    
-  (0, 1)
    

**Answer:** (0, 1)

---

## **MCQ 5**

**Question:** The decision boundary of a basic logistic regression model is typically:

-  Non-linear
    
-  Quadratic
    
-  Cubic
    
-  Linear
    

**Answer:** Linear

---

## **MCQ 6**

**Question:** The hypothesis (prediction) of logistic regression is:

-  h(x) = xβ
    
-  h(x) = tanh(z)
    
-  h(x) = z²
    
-  h(x) = 1 / (1 + e^(−z))
    

**Answer:** h(x) = 1 / (1 + e^(−z))

---

## **MCQ 7**

**Question:** The log-odds (logit) is defined as:

-  log(1 − p)
    
-  log(p)
    
-  log(e^p)
    
-  log(p / (1 − p))
    

**Answer:** log(p / (1 − p))

---

## **MCQ 8**

**Question:** The loss function commonly used for binary logistic regression is:

-  MSE (Mean Squared Error)
    
-  Hinge loss
    
-  K-means loss
    
-  Binary cross entropy
    

**Answer:** Binary cross entropy

---

## **MCQ 9**

**Question:** Logistic Regression parameters are typically learned using:

-  Random guessing
    
-  Dropout
    
-  Backtracking search
    
-  Gradient descent
    

**Answer:** Gradient descent

---

## **MCQ 10**

**Question:** If the predicted probability ≥ 0.5, logistic regression commonly predicts:

-  Class 0
    
-  Both
    
-  None
    
-  Class 1
    

**Answer:** Class 1

---

## **MCQ 11**

**Question:** Regularization in logistic regression helps to:

-  Increase model size
    
-  Remove labels
    
-  Decrease data
    
-  Prevent overfitting
    

**Answer:** Prevent overfitting

---

## **MCQ 12**

**Question:** L2 regularization adds which penalty term to the loss?

-  λ Σ |βⱼ|
    
-  λ Σ √βⱼ
    
-  βⱼ / λ
    
-  λ Σ βⱼ²
    

**Answer:** λ Σ βⱼ²

---

## **MCQ 13**

**Question:** Logistic Regression is sensitive to which of the following issues in features?

-  Missing labels
    
-  Large datasets
    
-  Batch size
    
-  Multicollinearity
    

**Answer:** Multicollinearity

---

## **MCQ 14**

**Question:** Which metric is generally better for imbalanced classification problems?

-  Accuracy
    
-  Loss
    
-  MSE
    
-  F1-score
    

**Answer:** F1-score

---

## **MCQ 15**

**Question:** The ROC curve plots which two rates?

-  Accuracy vs Recall
    
-  Precision vs Loss
    
-  FPR vs Loss
    
-  TPR vs FPR
    

**Answer:** TPR vs FPR

---

## **MCQ 16**

**Question:** What does AUC stand for?

-  Average Under Calculation
    
-  Algorithm Utility Curve
    
-  Area Under Classification
    
-  Area Under Curve
    

**Answer:** Area Under Curve

---

## **MCQ 17**

**Question:** Logistic Regression will struggle when:

-  Data is numeric
    
-  Data is small
    
-  Using gradient descent
    
-  Classes are not linearly separable
    

**Answer:** Classes are not linearly separable

---

## **MCQ 18**

**Question:** Logistic regression assumes which relationship between features and outcome?

-  Non-linear decision boundary
    
-  No relationship in features
    
-  All features categorical
    
-  Linear relationship in log-odds
    

**Answer:** Linear relationship in log-odds

---

## **MCQ 19**

**Question:** The probability predicted by logistic regression lies:

-  Always 0
    
-  Always 1
    
-  Can be negative
    
-  Between 0 and 1
    

**Answer:** Between 0 and 1

---

## **MCQ 20**

**Question:** Which is a limitation of basic logistic regression?

-  Easy to implement
    
-  Fast training
    
-  Works well on linearly separable data
    
-  Cannot model complex non-linear patterns
    

**Answer:** Cannot model complex non-linear patterns

---


---



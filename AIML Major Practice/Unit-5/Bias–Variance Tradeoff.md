

## 1. Introduction

The **Bias–Variance Tradeoff** explains how model complexity affects prediction error.  
A good ML model must balance **bias** and **variance** to generalize well.

Total error can be decomposed into:

```
Total Error = Bias² + Variance + Irreducible Error
```

---

# 📌 2. Bias

## **Definition**

Bias is the error due to **simplifying assumptions** made by the model.

High bias → model is too simple → **underfitting**.

## **Characteristics of High Bias**

- Oversimplified model
    
- Misses important patterns
    
- Low flexibility
    
- Poor performance on training data
    
- Poor performance on test data
    

## **Examples of High-Bias Models**

- Linear regression on curved data
    
- Decision stump (tree with depth 1)
    
- kNN with large K
    

---

# 📌 3. Variance

## **Definition**

Variance is error due to the model being **too sensitive to training data**.

High variance → model is overly complex → **overfitting**.

## **Characteristics of High Variance**

- Model learns noise
    
- Very flexible, unstable
    
- Excellent training accuracy
    
- Poor test accuracy
    

## **Examples of High-Variance Models**

- Deep decision trees
    
- kNN with K = 1
    
- High-degree polynomial regression
    

---

# 📌 4. Tradeoff Explanation

### **Low Bias + High Variance**

- Model fits training data extremely well
    
- Performs poorly on unseen data
    

### **High Bias + Low Variance**

- Model is too simple
    
- Consistently inaccurate on both train and test
    

### **Balanced Bias–Variance**

- Good fit on train
    
- Good generalization on test
    
- Ideal performance
    

---

# 📌 5. Mathematical View

Total expected error:

```
E[(Y − Ŷ)²] = Bias² + Variance + Irreducible Error
```

Where:

- **Bias²** → error from incorrect assumptions
    
- **Variance** → sensitivity to fluctuations in training set
    
- **Irreducible error** → inherent noise in data, cannot be removed
    

---

# 📌 6. How Model Complexity Affects Bias–Variance

|Model Complexity|Bias|Variance|Under/Overfitting|
|---|---|---|---|
|Low (simple model)|High|Low|Underfitting|
|High (complex model)|Low|High|Overfitting|

Graphically:

- Increasing complexity **decreases bias**
    
- Increasing complexity **increases variance**
    

---

# 📌 7. Techniques to Control Bias & Variance

## **To Reduce High Bias (Underfitting)**

- Increase model complexity
    
- Add more features
    
- Reduce regularization
    
- Use deeper trees / larger networks
    

---

## **To Reduce High Variance (Overfitting)**

- Add regularization (L1, L2)
    
- Use dropout (for neural nets)
    
- Reduce model complexity
    
- Increase training data
    
- Early stopping
    
- Use cross-validation
    
- Ensemble methods (e.g., Random Forest reduces variance)
    

---

# 📌 8. Real-World Examples

### Example 1: kNN

- Small K → low bias, high variance (overfitting)
    
- Large K → high bias, low variance (underfitting)
    

### Example 2: Decision Trees

- Deep tree → low bias, high variance
    
- Shallow tree → high bias, low variance
    

### Example 3: Polynomial Regression

- High degree → high variance (wiggly curve)
    
- Low degree → high bias (straight line)
    

---

# 📌 9. Summary Table

|Property|High Bias|High Variance|
|---|---|---|
|Model Type|Simple|Complex|
|Error Source|Wrong assumptions|Too sensitive to training data|
|Effect|Underfitting|Overfitting|
|Train Error|High|Low|
|Test Error|High|High|
|Fix|Increase complexity|Decrease complexity|

---

# 📌 Bias–Variance Tradeoff — MCQs (20)

Each MCQ includes **question → options → visible answer**.

---

## **MCQ 1**

**Question:** Bias in ML represents:

-  Sensitivity to noise
    
-  Error due to incorrect assumptions
    
-  Over-complex models
    
-  Variability in estimates
    

**Answer:** Error due to incorrect assumptions

---

## **MCQ 2**

**Question:** High bias leads to:

-  Overfitting
    
-  Smoother decision boundaries
    
-  Underfitting
    
-  High variance
    

**Answer:** Underfitting

---

## **MCQ 3**

**Question:** Variance in ML refers to:

-  Error due to simplifying assumptions
    
-  Irreducible noise
    
-  Sensitivity to training data
    
-  Model noise
    

**Answer:** Sensitivity to training data

---

## **MCQ 4**

**Question:** High variance leads to:

-  Underfitting
    
-  Perfect generalization
    
-  No learning
    
-  Overfitting
    

**Answer:** Overfitting

---

## **MCQ 5**

**Question:** Total error is composed of:

-  Bias + variance
    
-  Accuracy + loss
    
-  Bias² + variance + irreducible error
    
-  Error + outliers
    

**Answer:** Bias² + variance + irreducible error

---

## **MCQ 6**

**Question:** A very simple model usually has:

-  Low bias, high variance
    
-  High bias, low variance
    
-  Low bias, low variance
    
-  No bias
    

**Answer:** High bias, low variance

---

## **MCQ 7**

**Question:** A very complex model usually has:

-  High bias, low variance
    
-  Low bias, high variance
    
-  High bias, high variance
    
-  Low bias, low variance
    

**Answer:** Low bias, high variance

---

## **MCQ 8**

**Question:** Which model is most likely to underfit?

-  Deep neural network
    
-  Linear regression on curved data
    
-  High-degree polynomial
    
-  Large random forest
    

**Answer:** Linear regression on curved data

---

## **MCQ 9**

**Question:** Which model is most likely to overfit?

-  Simple linear model
    
-  Logistic regression
    
-  Decision tree with depth=20
    
-  kNN with K=50
    

**Answer:** Decision tree with depth=20

---

## **MCQ 10**

**Question:** Increasing model complexity generally:

-  Decreases variance
    
-  Decreases bias
    
-  Increases bias
    
-  Removes noise
    

**Answer:** Decreases bias

---

## **MCQ 11**

**Question:** Which method reduces variance?

-  Add more training data
    
-  Increase model complexity
    
-  Reduce regularization
    
-  Increase polynomial degree
    

**Answer:** Add more training data

---

## **MCQ 12**

**Question:** Which method reduces bias?

-  Use simpler model
    
-  Reduce number of features
    
-  Increase model complexity
    
-  Add dropout
    

**Answer:** Increase model complexity

---

## **MCQ 13**

**Question:** Ensemble methods like Random Forest mainly reduce:

-  Bias
    
-  Loss
    
-  Variance
    
-  Noise
    

**Answer:** Variance

---

## **MCQ 14**

**Question:** Early stopping is used to prevent:

-  Underfitting
    
-  Data leakage
    
-  Overfitting
    
-  High bias
    

**Answer:** Overfitting

---

## **MCQ 15**

**Question:** A model with high bias and high variance would be:

-  Overfitting
    
-  Underfitting
    
-  Completely failed
    
-  Perfect
    

**Answer:** Completely failed

---

## **MCQ 16**

**Question:** In kNN, small K leads to:

-  High bias
    
-  High variance
    
-  Low variance
    
-  No learning
    

**Answer:** High variance

---

## **MCQ 17**

**Question:** In polynomial regression, high degree causes:

-  Low variance
    
-  Underfitting
    
-  High variance
    
-  No pattern
    

**Answer:** High variance

---

## **MCQ 18**

**Question:** Bias–variance tradeoff aims to minimize:

-  Only variance
    
-  Only bias
    
-  Total error
    
-  Dataset size
    

**Answer:** Total error

---

## **MCQ 19**

**Question:** Which error cannot be reduced by any model?

-  Bias
    
-  Variance
    
-  Irreducible error
    
-  Approximation error
    

**Answer:** Irreducible error

---

## **MCQ 20**

**Question:** A well-generalized model has:

-  High bias, low variance
    
-  Low bias, high variance
    
-  Low bias, low variance
    
-  High bias, high variance
    

**Answer:** Low bias, low variance

---


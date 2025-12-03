

## 1. Introduction

In machine learning, the goal is to create models that **generalize well** to unseen data.  
Two common problems affecting generalization:

- **Overfitting** → Model learns too much noise
    
- **Underfitting** → Model learns too little pattern
    

---

# 📌 2. Underfitting

## **Definition**

A model underfits when it is **too simple** to capture patterns in the training data.

## **Characteristics**

- High **bias**
    
- Low **variance**
    
- Poor performance on **training data**
    
- Poor performance on **test data**
    

## **Causes**

- Model is too simple (e.g., linear model for curved data)
    
- Too few features
    
- Too much regularization
    
- Insufficient training
    

## **Solutions**

- Use more complex models
    
- Add more features
    
- Reduce regularization
    
- Train longer / tune parameters
    

Examples:

- Fitting a straight line through curved data
    
- Using KNN with K too large
    

---

# 📌 3. Overfitting

## **Definition**

A model overfits when it **fits noise** instead of the true pattern.

## **Characteristics**

- Low **bias**
    
- High **variance**
    
- Excellent performance on **training data**
    
- Poor performance on **test data**
    

## **Causes**

- Model too complex
    
- Too many features
    
- Too little data
    
- No regularization
    
- Training too long
    

## **Solutions**

- Add regularization (L1, L2)
    
- Reduce model complexity
    
- Use dropout (NNs)
    
- Cross-validation
    
- Increase training data
    
- Early stopping
    

Examples:

- Polynomial degree too high
    
- Deep neural networks without regularization
    

---

# 📌 4. Bias–Variance Tradeoff

- **Bias** → Error due to model assumptions
    
- **Variance** → Error due to model sensitivity to training data
    

Relationship:

- High bias → underfitting
    
- High variance → overfitting
    

Goal:

> Find a model complexity that balances bias and variance.

---

# 📌 5. Detecting Overfitting vs Underfitting

|Behavior|Train Error|Test Error|
|---|---|---|
|**Underfitting**|High|High|
|**Overfitting**|Low|High|
|**Good Fit**|Low|Low|

---

# 📌 6. How to Fix Both

### **Fix Underfitting**

- Increase model complexity
    
- Add features
    
- Reduce regularization
    
- Train longer
    

### **Fix Overfitting**

- Reduce complexity
    
- Add regularization
    
- Use cross-validation
    
- Use dropout
    
- Collect more data
    

---

# 📌 MCQs (20) — Overfitting & Underfitting

Each MCQ includes **question, options, and visible answer**.

---

## **MCQ 1**

**Question:** Underfitting occurs when the model is:

-  Too complex
    
-  Random
    
-  Too simple
    
-  Perfect
    

**Answer:** Too simple

---

## **MCQ 2**

**Question:** Overfitting occurs when the model:

-  Fits only noise
    
-  Fits too little pattern
    
-  Has high bias
    
-  Ignores data
    

**Answer:** Fits only noise

---

## **MCQ 3**

**Question:** Which condition indicates overfitting?

-  High train error, high test error
    
-  Low train error, low test error
    
-  High train error, low test error
    
-  Low train error, high test error
    

**Answer:** Low train error, high test error

---

## **MCQ 4**

**Question:** Underfitting usually results from:

-  Too many layers
    
-  Too much data
    
-  Too simple a model
    
-  Too many features
    

**Answer:** Too simple a model

---

## **MCQ 5**

**Question:** Overfitting is associated with:

-  High bias
    
-  Low variance
    
-  Low bias
    
-  No variance
    

**Answer:** Low bias

---

## **MCQ 6**

**Question:** Underfitting is associated with:

-  High variance
    
-  Low bias
    
-  High bias
    
-  No bias
    

**Answer:** High bias

---

## **MCQ 7**

**Question:** A model that performs well on training data but poorly on test data is:

-  Underfitting
    
-  Generalizing well
    
-  Overfitting
    
-  Balanced
    

**Answer:** Overfitting

---

## **MCQ 8**

**Question:** Increasing model complexity generally increases:

-  Bias
    
-  Variance
    
-  Noise
    
-  Regularization
    

**Answer:** Variance

---

## **MCQ 9**

**Question:** Which technique helps reduce overfitting?

-  Increase polynomial degree
    
-  Remove regularization
    
-  Add dropout
    
-  Use simpler models
    

**Answer:** Add dropout

---

## **MCQ 10**

**Question:** Which technique helps reduce underfitting?

-  Add regularization
    
-  Increase model complexity
    
-  Reduce features
    
-  Early stopping
    

**Answer:** Increase model complexity

---

## **MCQ 11**

**Question:** The bias–variance tradeoff aims to minimize:

-  Variance alone
    
-  Bias alone
    
-  Total error
    
-  Feature count
    

**Answer:** Total error

---

## **MCQ 12**

**Question:** What does high variance typically indicate?

-  Underfitting
    
-  Balanced model
    
-  Overfitting
    
-  No learning
    

**Answer:** Overfitting

---

## **MCQ 13**

**Question:** Removing features often reduces:

-  Bias
    
-  Accuracy
    
-  Variance
    
-  Data quality
    

**Answer:** Variance

---

## **MCQ 14**

**Question:** Early stopping is used to prevent:

-  Underfitting
    
-  Dimensionality
    
-  Overfitting
    
-  Bias errors
    

**Answer:** Overfitting

---

## **MCQ 15**

**Question:** Which of the following is a sign of underfitting?

-  Very low error on training data
    
-  High error on training and test data
    
-  High variance
    
-  Too many parameters
    

**Answer:** High error on training and test data

---

## **MCQ 16**

**Question:** Adding more data usually reduces:

-  Bias
    
-  Variance
    
-  Noise
    
-  Regularization
    

**Answer:** Variance

---

## **MCQ 17**

**Question:** Dropout is a regularization method used in:

-  Decision trees
    
-  Naive Bayes
    
-  Neural networks
    
-  SVM
    

**Answer:** Neural networks

---

## **MCQ 18**

**Question:** A very large value of C in SVM leads to:

-  More bias
    
-  More margin
    
-  Overfitting
    
-  Underfitting
    

**Answer:** Overfitting

---

## **MCQ 19**

**Question:** Using a polynomial of degree 1 for curved data leads to:

-  Perfect fit
    
-  Overfitting
    
-  Underfitting
    
-  Balanced model
    

**Answer:** Underfitting

---

## **MCQ 20**

**Question:** Which situation indicates a well-generalized model?

-  Low train error, low test error
    
-  High train error, low test error
    
-  Low train error, high test error
    
-  High train error, high test error
    

**Answer:** Low train error, low test error

---


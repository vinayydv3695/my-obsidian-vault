

## 1. What is Cross-Validation?

Cross-validation (CV) is a **resampling method** used to evaluate machine learning models on **unseen data**.

Goal:

> Estimate how well a model will generalize to new data.

It reduces:

- Overfitting
    
- Bias in performance estimation
    

---

# 📌 2. Why Use Cross-Validation?

✔ Provides a more reliable estimate than a simple train-test split  
✔ Useful when dataset is small  
✔ Ensures every data point gets used for both training & testing  
✔ Helps in model selection and hyperparameter tuning

---

# 📌 3. Types of Cross-Validation

---

# **1. Hold-Out Method**

### Description:

- Split dataset into **train** and **test** sets
    
- Typical split: 70/30 or 80/20
    

### Pros:

- Fast
    
- Simple
    

### Cons:

- High variance → results depend on how the split is done
    

---

# **2. k-Fold Cross-Validation**

### Description:

1. Split dataset into **k equal folds**
    
2. Use **k−1 folds** for training, **1 fold** for testing
    
3. Repeat k times
    
4. Take average performance
    

### Typical k values: 5 or 10

### Pros:

- Low variance
    
- Effective for small datasets
    

### Cons:

- Computationally expensive
    

---

# **3. Stratified k-Fold Cross-Validation**

### Description:

- Similar to k-fold
    
- But preserves **class distribution** in each fold
    

### Used for:

- Classification with imbalanced datasets
    

---

# **4. Leave-One-Out Cross-Validation (LOOCV)**

### Description:

- Special case of k-fold where **k = n**
    
- Train on n−1 samples, test on 1
    

### Pros:

- Lowest bias
    
- Uses maximum possible data for training
    

### Cons:

- Very expensive
    
- High variance
    

---

# **5. Leave-P-Out Cross-Validation**

### Description:

- Leave **P** points out for testing
    
- Train on **n − P** samples
    
- Repeat for all combinations
    

### Cons:

- Exponentially expensive
    

---

# **6. Repeated k-Fold Cross-Validation**

### Description:

- Perform k-fold CV **multiple times** with different random splits
    

### Pros:

- Further reduces variance
    

---

# **7. Time-Series Cross-Validation (Rolling Window / Expanding Window)**

### For sequential data

Cannot use random shuffling.

### Methods:

1. **Forward Chaining / Rolling Origin**
    

```
Train: 1 → t  
Test: t+1  
```

2. **Expanding Window**
    

```
Train on increasing data size  
Test on next step  
```

### Pros:

- Respects order of time
    

### Cons:

- Computationally costly
    

---

# **8. Nested Cross-Validation**

Used for:

- Hyperparameter tuning
    
- Comparing models fairly
    

### Two loops:

- **Inner loop:** find best hyperparameters
    
- **Outer loop:** evaluate model performance
    

---

# 📌 4. Advantages of Cross-Validation

✔ More accurate model evaluation  
✔ Reduces overfitting  
✔ Works well with small datasets  
✔ Helps in comparing multiple models  
✔ Provides stable estimates

---

# 📌 5. Disadvantages of Cross-Validation

✘ Computationally expensive  
✘ Not suitable for time-series data (except special CV)  
✘ LOOCV can have high variance

---

# 📌 6. Summary Table

|CV Method|Bias|Variance|Cost|
|---|---|---|---|
|Hold-Out|High|High|Low|
|k-Fold|Moderate|Moderate|Medium|
|LOOCV|Low|High|Very High|
|Stratified k-Fold|Low|Low|Medium|
|Time-Series CV|Depends|Depends|Medium|

---

# 📌 Cross-Validation — MCQs (20)

Each MCQ includes **question → options → visible answer**.

---

## **MCQ 1**

**Question:** Cross-validation is mainly used to estimate:

-  Learning rate
    
-  Model generalization performance
    
-  Feature importance
    
-  Model memory usage
    

**Answer:** Model generalization performance

---

## **MCQ 2**

**Question:** In k-fold CV, k typically equals:

-  1
    
-  100
    
-  5 or 10
    
-  n
    

**Answer:** 5 or 10

---

## **MCQ 3**

**Question:** LOOCV is equivalent to k-fold CV when:

-  k = 2
    
-  k = 5
    
-  k = 10
    
-  k = n
    

**Answer:** k = n

---

## **MCQ 4**

**Question:** Stratified k-fold is used to:

-  Clean data
    
-  Remove outliers
    
-  Preserve class distribution
    
-  Scale features
    

**Answer:** Preserve class distribution

---

## **MCQ 5**

**Question:** The hold-out method suffers from:

-  Low bias
    
-  Low variance
    
-  High variance
    
-  No noise
    

**Answer:** High variance

---

## **MCQ 6**

**Question:** k-fold CV reduces:

-  Data
    
-  Computation
    
-  Variance in model evaluation
    
-  Overfitting always
    

**Answer:** Variance in model evaluation

---

## **MCQ 7**

**Question:** LOOCV has:

-  Low bias, low variance
    
-  High bias, low variance
    
-  Low bias, high variance
    
-  High bias, high variance
    

**Answer:** Low bias, high variance

---

## **MCQ 8**

**Question:** Which CV method is best for imbalanced classification?

-  Hold-out
    
-  Random split
    
-  Stratified k-Fold
    
-  LOOCV
    

**Answer:** Stratified k-Fold

---

## **MCQ 9**

**Question:** Time-series CV must:

-  Shuffle data randomly
    
-  Remove timestamps
    
-  Preserve order of observations
    
-  Use LOOCV
    

**Answer:** Preserve order of observations

---

## **MCQ 10**

**Question:** Nested CV is primarily used for:

-  Data cleaning
    
-  Feature selection
    
-  Hyperparameter tuning
    
-  Sampling
    

**Answer:** Hyperparameter tuning

---

## **MCQ 11**

**Question:** Repeated k-fold CV reduces:

-  Bias
    
-  Variance
    
-  Data size
    
-  Overfitting always
    

**Answer:** Variance

---

## **MCQ 12**

**Question:** Which method is most computationally expensive?

-  Hold-out
    
-  k-fold
    
-  LOOCV
    
-  Stratified split
    

**Answer:** LOOCV

---

## **MCQ 13**

**Question:** In k-fold CV, each data point is used for testing:

-  0 times
    
-  1 time
    
-  k times
    
-  n times
    

**Answer:** 1 time

---

## **MCQ 14**

**Question:** k-fold CV prevents:

-  Bias
    
-  Data leakage
    
-  High variance in evaluation
    
-  Feature scaling issues
    

**Answer:** High variance in evaluation

---

## **MCQ 15**

**Question:** Time-series CV is needed because:

-  Data is too large
    
-  Observations are dependent
    
-  Data is categorical
    
-  Classes are imbalanced
    

**Answer:** Observations are dependent

---

## **MCQ 16**

**Question:** In k-fold CV, increasing k generally:

-  Reduces computation
    
-  Reduces bias
    
-  Increases bias
    
-  Removes variance
    

**Answer:** Reduces bias

---

## **MCQ 17**

**Question:** In k-fold CV, decreasing k increases:

-  Bias
    
-  Sample size
    
-  Generalization
    
-  Regularization
    

**Answer:** Bias

---

## **MCQ 18**

**Question:** Nested CV prevents:

-  Overfitting to validation set
    
-  Data scaling
    
-  Underfitting
    
-  Feature leakage
    

**Answer:** Overfitting to validation set

---

## **MCQ 19**

**Question:** Which CV method uses nearly all data for training each iteration?

-  Hold-out
    
-  k-fold
    
-  LOOCV
    
-  Time-series CV
    

**Answer:** LOOCV

---

## **MCQ 20**

**Question:** Cross-validation helps mainly with:

-  Data cleaning
    
-  Model evaluation and selection
    
-  Noise removal
    
-  Feature scaling
    

**Answer:** Model evaluation and selection

---


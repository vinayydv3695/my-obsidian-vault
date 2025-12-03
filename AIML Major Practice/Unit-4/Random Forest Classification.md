
## 1. Introduction

Random Forest is an **ensemble learning algorithm** that builds multiple **decision trees** and combines their results.

It is used for:

- **Classification**
    
- **Regression**
    

Core idea:

> “A forest of weak decision trees becomes a strong predictive model.”

---

## 2. How Random Forest Works

Random Forest creates multiple decision trees using **two kinds of randomness**:

### **1. Bootstrap Sampling (Bagging)**

Random subsets of training data are chosen **with replacement**.

This creates many diverse datasets → many diverse trees.

---

### **2. Random Feature Selection**

At each split in the tree:

- Instead of checking **all** features,
    
- A **random subset of features** is chosen.
    

This reduces correlation between trees → increases accuracy.

---

## 3. Prediction in Random Forest

### **Classification**

Each tree votes for a class.  
Final output = **majority vote**.

### **Regression**

Final output = **average of all tree predictions**.

---

## 4. Out-of-Bag (OOB) Error

Since bootstrap sampling leaves out ~37% of samples for each tree:

- These left-out samples are called **Out-of-Bag**.
    
- They act as **test data**.
    
- OOB Error ≈ Validation error
    
- Used for model evaluation **without cross-validation**.
    

---

## 5. Feature Importance

Random Forest provides **feature importance** based on:

- How much each feature reduces impurity across all trees
    
- Or using **permutation importance**
    

This helps in:

- Feature selection
    
- Understanding model behavior
    

---

## 6. Advantages

- Handles high-dimensional data
    
- Works for both regression and classification
    
- Reduces overfitting (compared to a single tree)
    
- Good performance out-of-the-box
    
- Can handle missing data fairly well
    
- Provides feature importance
    

---

## 7. Disadvantages

- Slower than a single decision tree
    
- Harder to interpret (not explainable like a single tree)
    
- Memory-intensive
    
- Can still overfit if the number of trees is too large
    

---

## 8. Hyperparameters

Key hyperparameters:

```
n_estimators        → number of trees
max_depth           → maximum depth of each tree
min_samples_split   → minimum samples required to split
min_samples_leaf    → minimum samples at leaf
max_features        → number of features to consider at each split
bootstrap           → whether to use bootstrapping
oob_score           → compute out-of-bag error
```

---

## 9. Applications

- Fraud detection
    
- Credit scoring
    
- Medical diagnosis
    
- Stock market prediction
    
- Recommender systems
    
- Customer segmentation
    

---

# 📌 Random Forest — MCQs (20) 


---

## **MCQ 1**

**Question:** Random Forest is an example of:

-  Clustering algorithm
    
-  Dimensionality reduction
    
-  Ensemble learning
    
-  Reinforcement learning
    

**Answer:** Ensemble learning

---

## **MCQ 2**

**Question:** Random Forest is based on which individual model?

-  Logistic regression
    
-  Neural networks
    
-  Decision trees
    
-  KNN
    

**Answer:** Decision trees

---

## **MCQ 3**

**Question:** What does “bagging” stand for?

-  Bootstrap aggregation
    
-  Binary averaging
    
-  Bag-level grouping
    
-  Bias aggregation
    

**Answer:** Bootstrap aggregation

---

## **MCQ 4**

**Question:** During bootstrap sampling:

-  Data is selected without replacement
    
-  Only test data is selected
    
-  All samples are used equally
    
-  Data is selected with replacement
    

**Answer:** Data is selected with replacement

---

## **MCQ 5**

**Question:** In Random Forest classification, the final output is:

-  Average of predictions
    
-  Posterior probability
    
-  Weighted regression
    
-  Majority vote
    

**Answer:** Majority vote

---

## **MCQ 6**

**Question:** Why does Random Forest use random subsets of features?

-  To reduce training time
    
-  To improve linearity
    
-  To reduce correlation between trees
    
-  To increase tree depth
    

**Answer:** To reduce correlation between trees

---

## **MCQ 7**

**Question:** Out-of-Bag samples are used to calculate:

-  Bias
    
-  Feature scaling
    
-  OOB Error
    
-  Regularization
    

**Answer:** OOB Error

---

## **MCQ 8**

**Question:** What is the purpose of using many trees in a forest?

-  Reduce accuracy
    
-  Avoid parallel computing
    
-  Increase variance
    
-  Reduce overfitting
    

**Answer:** Reduce overfitting

---

## **MCQ 9**

**Question:** Random Forest provides which useful metric?

-  Word embeddings
    
-  Perplexity
    
-  Feature importance
    
-  Layer weights
    

**Answer:** Feature importance

---

## **MCQ 10**

**Question:** Increasing `n_estimators` usually:

-  Reduces tree depth
    
-  Reduces model performance
    
-  Reduces variance
    
-  Increases variance
    

**Answer:** Reduces variance

---

## **MCQ 11**

**Question:** Which parameter limits overfitting?

-  max_depth
    
-  learning_rate
    
-  stride
    
-  dropout
    

**Answer:** max_depth

---

## **MCQ 12**

**Question:** Random Forest works well with:

-  Categorical data
    
-  Numerical data
    
-  Missing data
    
-  All of the above
    

**Answer:** All of the above

---

## **MCQ 13**

**Question:** Random Forest tends to struggle when:

-  Data is high-dimensional
    
-  Data is mixed (numeric + categorical)
    
-  Correlation between trees is high
    
-  Data is nonlinear
    

**Answer:** Correlation between trees is high

---

## **MCQ 14**

**Question:** Which hyperparameter controls the number of decision trees?

-  max_features
    
-  bootstrap
    
-  max_depth
    
-  n_estimators
    

**Answer:** n_estimators

---

## **MCQ 15**

**Question:** Random Forest reduces overfitting by:

-  Using one deep tree
    
-  Using gradient descent
    
-  Combining many uncorrelated trees
    
-  Increasing tree depth
    

**Answer:** Combining many uncorrelated trees

---

## **MCQ 16**

**Question:** The default value of `bootstrap=True` indicates:

-  Trees are shallow
    
-  No sampling is done
    
-  Bagging is applied
    
-  All features are used at each split
    

**Answer:** Bagging is applied

---

## **MCQ 17**

**Question:** Random Forest is:

-  Easy to interpret
    
-  Highly interpretable model
    
-  Black-box model
    
-  Transparent and simple
    

**Answer:** Black-box model

---

## **MCQ 18**

**Question:** Random Forest reduces:

-  Bias only
    
-  Variance only
    
-  Neither bias nor variance
    
-  Both bias and variance
    

**Answer:** Variance only

---

## **MCQ 19**

**Question:** Random Forest can handle missing values by:

-  Deleting rows
    
-  Using mean imputation
    
-  Using internal surrogate splits
    
-  Refusing to train
    

**Answer:** Using internal surrogate splits

---

## **MCQ 20**

**Question:** Random Forest regression output is computed by:

-  Maximum likelihood
    
-  Majority vote
    
-  Median
    
-  Averaging predictions
    

**Answer:** Averaging predictions

---

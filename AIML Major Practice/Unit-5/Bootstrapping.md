

## 1. Introduction

**Bootstrapping** is a **resampling technique** used in statistics and machine learning to estimate:

- Accuracy of a model
    
- Variance of an estimator
    
- Confidence intervals
    
- Sampling distribution of a statistic
    

It works by drawing **multiple samples with replacement** from the original dataset.

---

# 📌 2. What Is Bootstrapping?

Given a dataset of size **n**, bootstrapping creates **B new datasets** (bootstrap samples), each also size **n**, by sampling **with replacement**.

This means:

- Some points will appear multiple times
    
- Some points may not appear at all
    

---

## 3. Purpose of Bootstrapping

Bootstrapping helps us:

- Estimate **uncertainty** of predictions
    
- Approximate **sampling distribution** without complex formulas
    
- Compute **confidence intervals**, **bias**, and **variance**
    
- Train models when data is limited
    

Bootstrapping is especially useful when:

- Theoretical distribution is unknown
    
- Sample size is small
    
- Analytical solutions are hard
    

---

# 📌 4. Bootstrap Sample

### Example:

Original dataset: {1, 2, 3, 4}

A bootstrap sample (size 4) may look like:  
{2, 4, 2, 3}

Each element is chosen **with replacement**.

---

# 📌 5. Out-of-Bag (OOB) Samples

Since each bootstrap sample draws **n samples with replacement**, on average:

- Only **63.2%** of unique observations appear
    
- Remaining **36.8%** do NOT appear → Out-of-Bag samples
    

OOB samples are used in:

- **Random Forest** for OOB error estimation
    
- Model validation without cross-validation
    

---

# 📌 6. Types of Bootstrapping

## **1. Non-parametric Bootstrapping**

- Most common
    
- Resample data directly
    

## **2. Parametric Bootstrapping**

- Assume data comes from a known distribution
    
- Sample using estimated parameters
    

## **3. Bayesian Bootstrapping**

- Uses weights drawn from a Dirichlet distribution
    

---

# 📌 7. Bootstrapping vs Traditional Sampling

|Method|Resample Size|Replacement|Purpose|
|---|---|---|---|
|Normal sampling|< n|No|Train-test split|
|Bootstrapping|n|Yes|Estimate uncertainty|

---

# 📌 8. When Bootstrapping Is Useful

✔ Small datasets  
✔ Unknown population distribution  
✔ Estimating confidence intervals  
✔ Estimating standard errors  
✔ Bagging/Random Forest models  
✔ Model stability analysis

---

# 📌 9. When Bootstrapping Fails

✘ When dataset is too small (n < 10)  
✘ When data is highly dependent (e.g., time series without modification)  
✘ When noise is extremely high

---

# 📌 10. Relationship to Bagging (Bootstrap Aggregating)

Bagging uses:

- Bootstrapping to generate training subsets
    
- Aggregation to reduce variance
    

Random Forest = Bagging + Random Feature Selection.

---

# 📌 Bootstrapping — MCQs (20)

Each MCQ includes **question → options → visible answer**.

---

## **MCQ 1**

**Question:** Bootstrapping samples data:

-  Without replacement
    
-  Only once
    
-  With replacement
    
-  By shuffling only
    

**Answer:** With replacement

---

## **MCQ 2**

**Question:** The size of each bootstrap sample is typically:

-  n/2
    
-  2n
    
-  n
    
-  n²
    

**Answer:** n

---

## **MCQ 3**

**Question:** Bootstrapping is mainly used to estimate:

-  Learning rate
    
-  Sampling distribution
    
-  Optimization loss
    
-  Clustering centroids
    

**Answer:** Sampling distribution

---

## **MCQ 4**

**Question:** Which of the following appears on average in a bootstrap sample?

-  100% of observations
    
-  50% of observations
    
-  63.2% of observations
    
-  10% of observations
    

**Answer:** 63.2% of observations

---

## **MCQ 5**

**Question:** Out-of-Bag samples are used to:

-  Increase variance
    
-  Test the model
    
-  Train the model
    
-  Remove noise
    

**Answer:** Test the model

---

## **MCQ 6**

**Question:** Bootstrapping is essential for which ML method?

-  K-Means
    
-  Gradient Descent
    
-  Random Forest
    
-  SVM
    

**Answer:** Random Forest

---

## **MCQ 7**

**Question:** Bootstrapping is helpful when:

-  The sample size is small
    
-  Data is extremely large
    
-  Distribution is known
    
-  Noise is high
    

**Answer:** The sample size is small

---

## **MCQ 8**

**Question:** Which type of bootstrapping assumes a known distribution?

-  Random
    
-  Bayesian
    
-  Non-parametric
    
-  Parametric
    

**Answer:** Parametric

---

## **MCQ 9**

**Question:** In non-parametric bootstrapping, we sample from:

-  Estimated distribution
    
-  Uniform distribution
    
-  Original dataset
    
-  Gaussian distribution
    

**Answer:** Original dataset

---

## **MCQ 10**

**Question:** The number of bootstrap samples (B) is typically:

-  1
    
-  Very large (e.g., 1000)
    
-  n²
    
-  Always equal to n
    

**Answer:** Very large (e.g., 1000)

---

## **MCQ 11**

**Question:** Bootstrapping helps estimate:

-  Standard error
    
-  Hyperparameters
    
-  Missing features
    
-  Feature scaling
    

**Answer:** Standard error

---

## **MCQ 12**

**Question:** Bootstrapping is NOT suitable for:

-  Time-series data without modifications
    
-  Small but iid datasets
    
-  Confidence interval estimation
    
-  Variance estimation
    

**Answer:** Time-series data without modifications

---

## **MCQ 13**

**Question:** Bagging stands for:

-  Bootstrap Aggregation
    
-  Binary Aggregation
    
-  Batch Generation
    
-  Bayesian Averaging
    

**Answer:** Bootstrap Aggregation

---

## **MCQ 14**

**Question:** Bootstrapping reduces:

-  Bias
    
-  Variance
    
-  Noise
    
-  Regularization
    

**Answer:** Variance

---

## **MCQ 15**

**Question:** A bootstrap sample will contain some observations:

-  Exactly once
    
-  At most twice
    
-  Multiple times
    
-  Never
    

**Answer:** Multiple times

---

## **MCQ 16**

**Question:** OOB error is commonly used in:

-  SVM
    
-  Decision trees
    
-  Naive Bayes
    
-  Random Forest
    

**Answer:** Random Forest

---

## **MCQ 17**

**Question:** Bootstrapping is a type of:

-  Ensemble method
    
-  Resampling method
    
-  Optimization method
    
-  Clustering method
    

**Answer:** Resampling method

---

## **MCQ 18**

**Question:** Bootstrapping approximates:

-  Learning rate
    
-  Loss function
    
-  Sampling distribution
    
-  Data preprocessing
    

**Answer:** Sampling distribution

---

## **MCQ 19**

**Question:** A dataset with n observations will have how many unique observations in a bootstrap sample on average?

-  n
    
-  n/2
    
-  63.2% of n
    
-  √n
    

**Answer:** 63.2% of n

---

## **MCQ 20**

**Question:** Bootstrapping helps overcome limitations due to:

-  Too many features
    
-  Too much training time
    
-  Small dataset size
    
-  High dimensionality
    

**Answer:** Small dataset size

---

If you want next, I can give you:  
✔ **Bagging (Bootstrap Aggregating) notes + MCQs**  
✔ **AdaBoost / Gradient Boosting notes + MCQs**  
✔ **Cross-Validation detailed notes + MCQs**  
✔ A consolidated **Unit-wise ML exam notes file for Obsidian**

Just tell me!
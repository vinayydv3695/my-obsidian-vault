

## 1. Introduction

Support Vector Machine (SVM) is a **supervised learning algorithm** used for:

- **Classification (main use)**
    
- **Regression (SVR)**
    

Goal:

> Find the optimal hyperplane that **maximally separates** classes.

---

# 📌 2. Key Concepts in SVM

## **2.1 Hyperplane**

A decision boundary used to separate classes.

- In 2D → line
    
- In 3D → plane
    
- In higher dimensions → hyperplane
    

---

## **2.2 Margin**

Distance between the hyperplane and the **nearest data points** from each class.

SVM tries to **maximize the margin** → best generalization.

---

## **2.3 Support Vectors**

The data points **closest to the hyperplane**.

- They determine the margin
    
- Removing them changes the boundary
    

SVM depends **only** on support vectors, not all data points.

---

# 📌 3. Hard Margin vs Soft Margin

## **3.1 Hard Margin SVM**

Assumes:

- Data is **perfectly linearly separable**
    
- No misclassification allowed
    

Rarely used because real-world data has noise.

---

## **3.2 Soft Margin SVM**

Allows classification errors using **slack variables (ξ)**.

Controlled by **C parameter**:

- Large C → fewer errors, less margin → **overfitting risk**
    
- Small C → more errors allowed → **smoother boundary**
    

---

# 📌 4. SVM Optimization Objective

### Goal:

```
Minimize:  (1/2)*||w||²  +  C * Σ ξᵢ
```

This balances:

- **Margin maximization**
    
- **Misclassification penalty**
    

---

# 📌 5. Kernel Trick (Kernel SVM)

SVM can only draw linear boundaries in original space.  
**Kernel Trick** allows SVM to classify **non-linear data** by mapping it into a high-dimensional space.

### Common Kernels:

## **5.1 Linear Kernel**

Best for linearly separable data.

```
K(x, x') = x · x'
```

---

## **5.2 Polynomial Kernel**

Useful for curved boundaries.

```
K(x, x') = (x · x' + c)ᵈ
```

Parameters: degree d, constant c.

---

## **5.3 RBF (Gaussian) Kernel** _(Most used)_

```
K(x, x') = exp(−γ ||x − x'||²)
```

- γ (gamma) controls the spread:
    
    - High γ → tighter curves → overfitting
        
    - Low γ → smoother shape → underfitting
        

---

## **5.4 Sigmoid Kernel**

Used in neural networks.

```
K(x, x') = tanh(α x·x' + c)
```

---

# 📌 6. Advantages of SVM

- Works well with high-dimensional data
    
- Effective in non-linear problems (with kernels)
    
- Robust to overfitting
    
- Strong theoretical foundation
    

---

# 📌 7. Disadvantages of SVM

- Slow on large datasets
    
- Hard to tune (C and gamma)
    
- No probabilistic output by default
    
- Not ideal for noisy datasets
    

---

# 📌 8. Hyperparameters in SVM

```
C        → regularization strength
kernel   → linear, poly, rbf, sigmoid
degree   → polynomial degree
gamma    → RBF kernel smoothness
coef0    → used in poly/sigmoid kernels
```

---

# 📌 9. Applications of SVM

- Face recognition
    
- Text classification
    
- Bioinformatics
    
- Handwriting recognition
    
- Spam filtering
    

---

# 📌 SVM & Kernel SVM — MCQs (20)

Each MCQ includes **question → options → answer**.

---

## **MCQ 1**

**Question:** SVM is mainly used for:

-  Clustering
    
-  Regression only
    
-  Classification
    
-  Dimensionality reduction
    

**Answer:** Classification

---

## **MCQ 2**

**Question:** The main goal of SVM is to:

-  Minimize entropy
    
-  Grow decision trees
    
-  Maximize margin
    
-  Increase cluster centers
    

**Answer:** Maximize margin

---

## **MCQ 3**

**Question:** Support vectors are:

-  Random data points
    
-  Furthest points from hyperplane
    
-  Points closest to hyperplane
    
-  All data points
    

**Answer:** Points closest to hyperplane

---

## **MCQ 4**

**Question:** Which parameter controls misclassification penalty?

-  gamma
    
-  kernel
    
-  degree
    
-  C
    

**Answer:** C

---

## **MCQ 5**

**Question:** Hard-margin SVM requires:

-  Categorical data
    
-  Perfectly separable data
    
-  Non-linear data
    
-  Missing values
    

**Answer:** Perfectly separable data

---

## **MCQ 6**

**Question:** The soft margin SVM uses slack variables to:

-  Increase number of kernels
    
-  Allow misclassification
    
-  Remove noise
    
-  Reduce margin
    

**Answer:** Allow misclassification

---

## **MCQ 7**

**Question:** Kernel trick is used to:

-  Reduce dimensionality
    
-  Remove noise
    
-  Transform data to a higher-dimensional space
    
-  Speed up training
    

**Answer:** Transform data to a higher-dimensional space

---

## **MCQ 8**

**Question:** The most commonly used kernel in SVM is:

-  Linear
    
-  Polynomial
    
-  Sigmoid
    
-  RBF (Gaussian)
    

**Answer:** RBF (Gaussian)

---

## **MCQ 9**

**Question:** In RBF kernel, gamma controls:

-  Number of support vectors
    
-  Margin width
    
-  Smoothness of decision boundary
    
-  Learning rate
    

**Answer:** Smoothness of decision boundary

---

## **MCQ 10**

**Question:** Large gamma in RBF kernel leads to:

-  Underfitting
    
-  Smoother boundaries
    
-  Overfitting
    
-  No impact
    

**Answer:** Overfitting

---

## **MCQ 11**

**Question:** Linear kernel is best suited for:

-  Curved data
    
-  Data with high noise
    
-  Nested classes
    
-  Linearly separable data
    

**Answer:** Linearly separable data

---

## **MCQ 12**

**Question:** Polynomial kernel uses which parameter?

-  epsilon
    
-  learning rate
    
-  degree
    
-  dropout
    

**Answer:** degree

---

## **MCQ 13**

**Question:** SVM is:

-  Non-parametric
    
-  Parametric
    
-  Probabilistic
    
-  Tree-based
    

**Answer:** Non-parametric

---

## **MCQ 14**

**Question:** Which of the following increases the margin width?

-  Increasing C
    
-  Decreasing C
    
-  Increasing gamma
    
-  Increasing degree
    

**Answer:** Decreasing C

---

## **MCQ 15**

**Question:** SVM struggles on:

-  Small datasets
    
-  High-dimensional data
    
-  Linearly separable data
    
-  Large datasets
    

**Answer:** Large datasets

---

## **MCQ 16**

**Question:** Which kernel function is similar to neural networks?

-  Polynomial
    
-  Linear
    
-  Sigmoid
    
-  RBF
    

**Answer:** Sigmoid

---

## **MCQ 17**

**Question:** SVM decision boundary is determined by:

-  Error terms
    
-  All points
    
-  Points far from margin
    
-  Support vectors
    

**Answer:** Support vectors

---

## **MCQ 18**

**Question:** Kernel SVM helps solve:

-  Overfitting
    
-  Non-linear classification problems
    
-  Missing data issues
    
-  Feature scaling
    

**Answer:** Non-linear classification problems

---

## **MCQ 19**

**Question:** Which SVM hyperparameter must be tuned carefully for RBF kernel?

-  dropout
    
-  hidden layers
    
-  gamma
    
-  stride
    

**Answer:** gamma

---

## **MCQ 20**

**Question:** SVM models are often considered:

-  Highly interpretable
    
-  Easy to visualize
    
-  Black-box models
    
-  Transparent
    

**Answer:** Black-box models

---


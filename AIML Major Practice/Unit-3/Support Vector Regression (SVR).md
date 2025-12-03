

## 1. Introduction

Support Vector Regression (SVR) is the **regression version of SVM**.  
It tries to fit a function that deviates from the actual target **by at most ε** (epsilon margin).

Goal:

> Find a regression line (or curve) that fits the data with the smallest error and maximum generalization.

---

## 2. Core Concepts

### **1. ε-Insensitive Tube**

SVR tries to fit a function such that:

- Errors **within** ε are ignored
    
- Errors **outside** ε are penalized
    

This creates a _margin of tolerance_.

---

### **2. Support Vectors**

Only the points **outside the ε-tube** influence the model.  
These points are the _support vectors_.

---

### **3. Flatness Objective**

SVR aims to make the function as flat as possible:

```
Minimize:  (1/2) * ||w||²
```

subject to constraints involving ε.

Flatness improves generalization.

---

## 3. Kernel Trick

SVR can use kernels to learn **non-linear** relationships:

Common kernels:

- Linear
    
- Polynomial
    
- RBF (Gaussian)
    
- Sigmoid
    

Kernel function maps input X → high-dimensional space where a linear regression boundary can be fit.

---

## 4. SVR Optimization Formulation

### **Primary objective:**

```
Minimize:   (1/2)||w||² + C * Σ (ξᵢ + ξᵢ*)
```

Where:

- C = penalty term (tradeoff between flatness & errors)
    
- ξᵢ, ξᵢ* = slack variables
    

Large C → low bias, high variance  
Small C → high bias, low variance

---

## 5. Hyperparameters

```
C          → regularization strength
ε          → epsilon-tube width
kernel     → linear, poly, RBF
gamma      → RBF kernel smoothness
degree     → polynomial degree
```

---

## 6. Advantages

- Works well with **non-linear** data
    
- Robust to outliers (because of ε-insensitive loss)
    
- Uses only support vectors → efficient model representation
    

---

## 7. Disadvantages

- Slow for large datasets
    
- Many hyperparameters to tune
    
- Hard to interpret
    
- Sensitive to feature scaling (must standardize data)
    

---

## 8. Applications

- Stock price prediction
    
- Time-series regression
    
- Weather forecasting
    
- Real-estate price prediction
    
- Load forecasting
    

---

# 📌 SVR — MCQs (20) 

Each MCQ includes **question, options, and visible answer**.

---

## **MCQ 1**

**Question:** SVR is based on which algorithm?

-  Decision trees
    
-  KNN
    
-  Logistic regression
    
-  Support Vector Machine
    

**Answer:** Support Vector Machine

---

## **MCQ 2**

**Question:** SVR uses which concept to ignore small errors?

-  Max-margin loss
    
-  Entropy
    
-  ε-insensitive loss
    
-  Gini impurity
    

**Answer:** ε-insensitive loss

---

## **MCQ 3**

**Question:** In SVR, points that influence the model are called:

-  Centroids
    
-  Leaves
    
-  Hidden units
    
-  Support vectors
    

**Answer:** Support vectors

---

## **MCQ 4**

**Question:** Which parameter controls the width of the ε-tube?

-  C
    
-  gamma
    
-  degree
    
-  ε
    

**Answer:** ε

---

## **MCQ 5**

**Question:** The main objective in SVR is to:

-  Minimize entropy
    
-  Maximize classification accuracy
    
-  Make the function flat
    
-  Reduce number of features
    

**Answer:** Make the function flat

---

## **MCQ 6**

**Question:** The regularization parameter C controls:

-  Kernel type
    
-  Number of clusters
    
-  Tradeoff between flatness and error
    
-  Number of support vectors
    

**Answer:** Tradeoff between flatness and error

---

## **MCQ 7**

**Question:** Which kernel is most commonly used for non-linear SVR?

-  Linear
    
-  Gaussian RBF
    
-  Hamming
    
-  Binary
    

**Answer:** Gaussian RBF

---

## **MCQ 8**

**Question:** SVR is sensitive to:

-  One-hot encoding
    
-  Missing labels
    
-  Feature scaling
    
-  Bagging
    

**Answer:** Feature scaling

---

## **MCQ 9**

**Question:** A smaller value of C leads to:

-  More complex model
    
-  Lower bias
    
-  Stronger penalties
    
-  Smoother model with higher bias
    

**Answer:** Smoother model with higher bias

---

## **MCQ 10**

**Question:** SVR can capture non-linear relationships using:

-  Gradient descent
    
-  PCA
    
-  Kernel trick
    
-  Entropy reduction
    

**Answer:** Kernel trick

---

## **MCQ 11**

**Question:** Which parameter controls the curvature of the RBF kernel?

-  C
    
-  ε
    
-  degree
    
-  gamma
    

**Answer:** gamma

---

## **MCQ 12**

**Question:** SVR is considered a:

-  Parametric model
    
-  Non-parametric model
    
-  Clustering model
    
-  Rule-based model
    

**Answer:** Non-parametric model

---

## **MCQ 13**

**Question:** In SVR, slack variables represent:

-  Kernel complexity
    
-  Amount of error beyond ε
    
-  Feature scaling
    
-  Regularization strength
    

**Answer:** Amount of error beyond ε

---

## **MCQ 14**

**Question:** SVR is most computationally expensive when the dataset is:

-  Numeric
    
-  Small
    
-  Categorical
    
-  Large
    

**Answer:** Large

---

## **MCQ 15**

**Question:** SVR performs regression by:

-  Averaging neighbors
    
-  Minimizing squared error
    
-  Fitting a function inside an ε-tube
    
-  Splitting data recursively
    

**Answer:** Fitting a function inside an ε-tube

---

## **MCQ 16**

**Question:** The loss function used in SVR is:

-  Cross-entropy loss
    
-  Hinge loss
    
-  ε-insensitive loss
    
-  MSE
    

**Answer:** ε-insensitive loss

---

## **MCQ 17**

**Question:** SVR tries to minimize:

-  ||w||²
    
-  dataset size
    
-  residual variance
    
-  number of features
    

**Answer:** ||w||²

---

## **MCQ 18**

**Question:** Which term is added when errors exceed ε?

-  kernel decay
    
-  entropy
    
-  slack variables
    
-  pruning metric
    

**Answer:** slack variables

---

## **MCQ 19**

**Question:** SVR aims to create a model that has:

-  High variance
    
-  Perfect fit to training data
    
-  Sparse support vectors
    
-  Complete dependence on all points
    

**Answer:** Sparse support vectors

---

## **MCQ 20**

**Question:** SVR prediction is based on:

-  Only X-values
    
-  All training points
    
-  Only support vectors
    
-  Centroid distances
    

**Answer:** Only support vectors

---

If you want next:  
✔ **SVM (Classification) notes + MCQs**  
✔ **K-Means Clustering notes + MCQs**  
✔ **PCA notes + MCQs**  
✔ A full **Unit 2 Machine Learning Revision Sheet** (Obsidian-ready)

Just tell me!
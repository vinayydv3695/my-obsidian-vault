

---

# 📌 K-Nearest Neighbors (KNN) 

## 1. Introduction

- KNN is a **supervised learning algorithm** used for:
    
    - **Classification**
        
    - **Regression**
        
- It is a **lazy learner** (no training phase).
    
- Decisions are made based on the **closest K neighbors** in the feature space.
    

---

## 2. How KNN Works

1. Choose **K** (number of neighbors).
    
2. Compute **distance** between the test point and all training points.
    
3. Select the **K nearest neighbors**.
    
4. For classification → take **majority vote**.  
    For regression → take **average**.
    
5. Output prediction.
    

---

## 3. Distance Metrics

Most common:

```
Euclidean:       d = √Σ(xᵢ − yᵢ)²
Manhattan:       d = Σ|xᵢ − yᵢ|
Minkowski:       d = (Σ|xᵢ − yᵢ|ᵖ)^(1/p)
```

---

## 4. Choosing K

- **Small K** → high variance, overfitting.
    
- **Large K** → smoother decision boundary, may underfit.
    
- Odd K is preferred for binary classification.
    

---

## 5. Pros of KNN

- Simple and intuitive.
    
- No training time.
    
- Works well with small datasets.
    
- Non-parametric → no assumptions about data distribution.
    

---

## 6. Cons of KNN

- Slow prediction on large datasets.
    
- Sensitive to **irrelevant features**.
    
- Sensitive to **feature scale**.
    
- Requires storing all training data.
    

---

## 7. Feature Scaling

KNN requires scaling:

```
Standardization: (x − μ) / σ
Normalization: (x − min) / (max − min)
```

---

## 8. Applications

- Recommendation systems
    
- Image classification
    
- Pattern recognition
    
- Anomaly detection
    

---

# 📌 KNN — MCQs (20 Obsidian-ready)

Each includes question → options → visible answer.

---

## **MCQ 1**

**Question:** KNN belongs to which type of learning?

-  Unsupervised
    
-  Reinforcement
    
-  Self-supervised
    
-  Supervised
    

**Answer:** Supervised

---

## **MCQ 2**

**Question:** KNN is considered a:

-  Eager learner
    
-  Deep learning model
    
-  Rule-based system
    
-  Lazy learner
    

**Answer:** Lazy learner

---

## **MCQ 3**

**Question:** KNN makes predictions based on:

-  Gradient descent
    
-  Activation functions
    
-  Nearest neighbors
    
-  Weight updates
    

**Answer:** Nearest neighbors

---

## **MCQ 4**

**Question:** KNN mainly uses which distance metric by default?

-  Manhattan
    
-  Hamming
    
-  Cosine
    
-  Euclidean
    

**Answer:** Euclidean

---

## **MCQ 5**

**Question:** Small values of K typically lead to:

-  Underfitting
    
-  Perfect accuracy
    
-  No effect
    
-  Overfitting
    

**Answer:** Overfitting

---

## **MCQ 6**

**Question:** Large values of K usually cause KNN to:

-  Memorize noise
    
-  Become more sensitive
    
-  Overfit
    
-  Underfit
    

**Answer:** Underfit

---

## **MCQ 7**

**Question:** Which step is required before applying KNN?

-  PCA
    
-  Normalization / Standardization
    
-  Removing labels
    
-  Building a neural network
    

**Answer:** Normalization / Standardization

---

## **MCQ 8**

**Question:** In KNN classification, the label is predicted using:

-  Mean of neighbors
    
-  Argmax of class counts
    
-  Weighted matrix multiplication
    
-  Logistic function
    

**Answer:** Argmax of class counts

---

## **MCQ 9**

**Question:** In KNN regression, the output is:

-  Mode of neighbors
    
-  Median of neighbors
    
-  Majority vote
    
-  Average of neighbors
    

**Answer:** Average of neighbors

---

## **MCQ 10**

**Question:** KNN complexity during prediction is:

-  O(1)
    
-  O(log n)
    
-  O(n)
    
-  O(n log n)
    

**Answer:** O(n)

---

## **MCQ 11**

**Question:** KNN is best suited for which type of dataset?

-  Very large datasets
    
-  High-dimensional data
    
-  Small datasets
    
-  Noisy data
    

**Answer:** Small datasets

---

## **MCQ 12**

**Question:** The Minkowski distance with p=1 becomes:

-  Euclidean
    
-  Mahalanobis
    
-  Cosine
    
-  Manhattan
    

**Answer:** Manhattan

---

## **MCQ 13**

**Question:** Which issue affects KNN the most?

-  Learning rate
    
-  Vanishing gradients
    
-  Multicollinearity
    
-  Curse of dimensionality
    

**Answer:** Curse of dimensionality

---

## **MCQ 14**

**Question:** KNN stores:

-  Only weights
    
-  Only model parameters
    
-  Summary of data
    
-  The entire dataset
    

**Answer:** The entire dataset

---

## **MCQ 15**

**Question:** For categorical variables, which distance metric is preferred?

-  Euclidean
    
-  Manhattan
    
-  Minkowski
    
-  Hamming
    

**Answer:** Hamming

---

## **MCQ 16**

**Question:** KNN decision boundaries are generally:

-  Always linear
    
-  Always non-linear
    
-  Quadratic
    
-  Cubic
    

**Answer:** Always non-linear

---

## **MCQ 17**

**Question:** KNN performs poorly when:

-  Data is low-dimensional
    
-  Classes are separable
    
-  Dataset is small
    
-  Dataset is high-dimensional
    

**Answer:** Dataset is high-dimensional

---

## **MCQ 18**

**Question:** What happens if K = 1?

-  Underfitting
    
-  No prediction
    
-  Perfect smoothing
    
-  Very high variance
    

**Answer:** Very high variance

---

## **MCQ 19**

**Question:** How is tie-breaking typically handled in KNN classification?

-  Random selection
    
-  Weighted loss
    
-  Linear regression
    
-  Increasing K
    

**Answer:** Random selection

---

## **MCQ 20**

**Question:** Which factor strongly affects KNN performance?

-  Number of epochs
    
-  Activation function
    
-  Feature scaling
    
-  Hidden layers
    

**Answer:** Feature scaling

---

If you want next:  
✔ **Naive Bayes notes + MCQs**  
✔ **SVM notes + MCQs**  
✔ A combined **chapter summary** for ML algorithms  
✔ A consolidated **Obsidian vault file** for the whole unit

Just tell me.
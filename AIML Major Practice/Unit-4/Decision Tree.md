

## 1. Introduction

A **Decision Tree** is a supervised learning algorithm used for:

- **Classification**
    
- **Regression** (Decision Tree Regressor)
    

It predicts the target by **learning simple decision rules** inferred from the data.

A decision tree consists of:

- **Root Node** → first split
    
- **Internal Nodes** → decisions
    
- **Leaf Nodes** → final class labels
    

---

## 2. How Decision Trees Work

The tree is built using a **top-down, greedy** approach:

1. Choose the **best feature** to split the data.
    
2. Apply the split to create child nodes.
    
3. Repeat recursively until stopping criteria are met.
    

This approach is called **"Recursive Binary Splitting".**

---

## 3. Impurity Measures (Splitting Criteria)

### **1. Gini Impurity**

Used in CART.

Formula:

```
Gini = 1 − Σ (pᵢ)²
```

Where pᵢ = probability of class i.

Properties:

- Lower Gini = purer node
    
- Fast to compute
    

---

### **2. Entropy (Information Gain)**

Used in ID3, C4.5.

```
Entropy = − Σ pᵢ * log₂(pᵢ)
```

**Information Gain (IG):**

```
IG = Entropy(parent) − Weighted entropy(children)
```

Higher IG = better split.

---

### **3. Classification Error**

Not commonly used for splitting.

```
Error = 1 − max(pᵢ)
```

---

## 4. Stopping Criteria

Tree stops growing when:

- All samples belong to the **same class**
    
- No feature remains to split
    
- Maximum depth reached
    
- Minimum samples per node reached
    
- Gain from splitting becomes negligible
    

---

## 5. Overfitting in Decision Trees

Decision trees can easily **overfit** because they keep splitting to reduce impurity.

### Ways to prevent overfitting:

#### **Pre-Pruning (Early Stopping)**

- Limit depth
    
- Min samples per split
    
- Min samples per leaf
    
- Max number of nodes
    

#### **Post-Pruning**

- Grow full tree
    
- Remove weak splits (cost-complexity pruning)
    

Formula for cost complexity pruning:

```
Rα(T) = R(T) + α|T|
```

---

## 6. Advantages

- Easy to understand and visualize
    
- Works with both numerical + categorical data
    
- No scaling required
    
- Can capture non-linear patterns
    
- Fast inference
    

---

## 7. Disadvantages

- Highly prone to **overfitting**
    
- Small changes in data → different tree
    
- Greedy splitting doesn't guarantee global optimum
    
- Biased toward features with more levels
    

---

## 8. Applications

- Medical diagnosis
    
- Fraud detection
    
- Loan approval
    
- Customer segmentation
    
- Credit scoring
    

---

# 📌 Decision Tree — MCQs (20) 

Each MCQ includes the **question**, **options**, and **visible answer**.

---

## **MCQ 1**

**Question:** Decision Trees are primarily used for:

-  Clustering
    
-  Dimensionality reduction
    
-  Reinforcement learning
    
-  Classification and regression
    

**Answer:** Classification and regression

---

## **MCQ 2**

**Question:** Which algorithm uses Gini Impurity?

-  ID3
    
-  Naive Bayes
    
-  C4.5
    
-  CART
    

**Answer:** CART

---

## **MCQ 3**

**Question:** Entropy is used to compute:

-  Mean squared error
    
-  Weight decay
    
-  Activation
    
-  Information Gain
    

**Answer:** Information Gain

---

## **MCQ 4**

**Question:** Which of the following leads to a pure node?

-  Gini = 0.45
    
-  Entropy = 0.5
    
-  Gini = 0
    
-  Entropy = 1
    

**Answer:** Gini = 0

---

## **MCQ 5**

**Question:** A greedy algorithm in decision trees means:

-  Looks ahead for all splits
    
-  Finds the global optimum
    
-  Uses dynamic programming
    
-  Chooses the best split at each step
    

**Answer:** Chooses the best split at each step

---

## **MCQ 6**

**Question:** Splitting stops when:

-  All nodes are pure
    
-  Features are exhausted
    
-  Max depth reached
    
-  All of the above
    

**Answer:** All of the above

---

## **MCQ 7**

**Question:** Decision Trees often suffer from:

-  Underfitting
    
-  High bias
    
-  High variance
    
-  Dimensionality reduction
    

**Answer:** High variance

---

## **MCQ 8**

**Question:** Which pruning method removes weak splits after building the full tree?

-  Early stopping
    
-  Regularization
    
-  Feature scaling
    
-  Post-pruning
    

**Answer:** Post-pruning

---

## **MCQ 9**

**Question:** Cost complexity pruning uses which parameter?

-  Dropout rate
    
-  Learning rate
    
-  Regularization constant α
    
-  Number of features
    

**Answer:** Regularization constant α

---

## **MCQ 10**

**Question:** Which impurity measure is the fastest to compute?

-  Entropy
    
-  Information gain
    
-  Chi-square
    
-  Gini impurity
    

**Answer:** Gini impurity

---

## **MCQ 11**

**Question:** In a decision tree, leaf nodes represent:

-  Best feature
    
-  Impure nodes
    
-  Decision boundaries
    
-  Final class labels
    

**Answer:** Final class labels

---

## **MCQ 12**

**Question:** Decision trees do NOT require:

-  One-hot encoding
    
-  Feature scaling
    
-  Normalization
    
-  Both normalization and scaling
    

**Answer:** Both normalization and scaling

---

## **MCQ 13**

**Question:** Which algorithm is known as the predecessor of decision tree techniques?

-  kNN
    
-  ID3
    
-  Logistic regression
    
-  Random Forest
    

**Answer:** ID3

---

## **MCQ 14**

**Question:** A tree becomes too deep and complex when it:

-  Underfits
    
-  Overfits
    
-  Has fewer nodes
    
-  Uses small datasets
    

**Answer:** Overfits

---

## **MCQ 15**

**Question:** Which of the following is a disadvantage of decision trees?

-  Easy to visualize
    
-  Fast inference
    
-  Handles non-linearity
    
-  Unstable with small changes in data
    

**Answer:** Unstable with small changes in data

---

## **MCQ 16**

**Question:** A split that reduces impurity the most is considered:

-  Invalid
    
-  Weak
    
-  Best
    
-  Noisy
    

**Answer:** Best

---

## **MCQ 17**

**Question:** Decision trees are biased toward features with:

-  Low variance
    
-  Strong correlations
    
-  More categories
    
-  Missing values
    

**Answer:** More categories

---

## **MCQ 18**

**Question:** Which dataset type is ideal for decision trees?

-  Linear data
    
-  Highly dimensional data
    
-  Non-linear relationships
    
-  Only numerical data
    

**Answer:** Non-linear relationships

---

## **MCQ 19**

**Question:** Which algorithm combines multiple decision trees?

-  Logistic regression
    
-  SVM
    
-  Naive Bayes
    
-  Random Forest
    

**Answer:** Random Forest

---

## **MCQ 20**

**Question:** Decision Tree regression uses which metric for splitting?

-  Cross entropy
    
-  MSE (Mean Squared Error)
    
-  Hinge loss
    
-  Accuracy
    

**Answer:** MSE (Mean Squared Error)

---

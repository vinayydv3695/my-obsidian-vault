Machine Learning models perform better when redundant, irrelevant, and noisy features are removed.  
This topic covers:

- **Feature Selection** → selecting the best subset of existing features
    
- **Feature Extraction** → transforming features into new ones (e.g., PCA)
    

---

# ============================

# **1. What is Feature Selection?**

# ============================

Feature Selection = choosing the most important features from the dataset.

### Why Feature Selection?

✔ Reduces overfitting  
✔ Improves accuracy  
✔ Reduces training time  
✔ Removes irrelevant/noisy features  
✔ Simplifies the model

---

# ============================

# **2. Types of Feature Selection Methods**

# ============================

There are **three main categories**:

---

# 📌 **A) Filter Methods**

Use statistical tests to score features.

### Common Filter Methods:

1. **Correlation Coefficient (Pearson)**
    
    - High correlation → remove one of the features
        
2. **Chi-Square Test**
    
    - For categorical variables
        
3. **ANOVA F-test**
    
    - For numerical → categorical target
        
4. **Mutual Information**
    
    - Measures shared information between features
        

### Pros:

✔ Fast  
✔ Model-independent

### Cons:

✘ Ignores interactions between features

---

# 📌 **B) Wrapper Methods**

Use ML models to evaluate feature subsets.

### Common Wrapper Techniques:

### **1. Forward Selection**

Start with **0 features** → keep adding best feature.

### **2. Backward Elimination**

Start with **all features** → remove worst one.

### **3. Recursive Feature Elimination (RFE)**

Uses model training to remove least important features iteratively.

### Pros:

✔ Very accurate  
✔ Considers interactions

### Cons:

✘ Slow  
✘ Computationally expensive

---

# 📌 **C) Embedded Methods**

Feature selection happens **during model training**.

### Common Embedded Techniques:

- **Lasso Regression (L1 Regularization)** → Shrinks some coefficients to 0
    
- **Ridge Regression (L2)** → Shrinks values, but not to zero
    
- **Tree-based Models (Random Forest, XGBoost)**  
    → Provide feature importance scores
    

### Pros:

✔ Balanced  
✔ Efficient  
✔ Used in real-world ML pipelines

---

# ============================

# **3. Feature Extraction Techniques**

# ============================

Feature Extraction = transform high-dimensional data into lower dimensions.

---

# 📌 **A) PCA (Principal Component Analysis)**

Already covered in Topic 5.  
Turns correlated variables → uncorrelated components.

---

# 📌 **B) LDA (Linear Discriminant Analysis)**

- Supervised technique
    
- Maximizes **class separation**
    
- Used in classification problems
    

---

# 📌 **C) t-SNE (t-Distributed Stochastic Neighbor Embedding)**

- Highly non-linear
    
- Produces 2D/3D visualization  
    ✘ Not for training ML models  
    ✔ Great for understanding data clusters
    

---

# 📌 **D) Autoencoders (Neural Networks)**

- Learn compressed representation of data
    
- Used for feature extraction in DL
    

---

# ============================

# **4. Feature Selection vs Feature Extraction**

# ============================

|Feature Selection|Feature Extraction|
|---|---|
|Removes irrelevant features|Creates new transformed features|
|Keeps original meaning|Hard to interpret|
|Simple|Complex|
|Faster|Slower|
|Examples: RFE, Lasso|PCA, LDA, Autoencoders|

---

# ============================

# **5. When to Use What?**

# ============================

### ✔ Use **Feature Selection** when:

- Dataset has irrelevant features
    
- Model interpretability matters
    
- You want simpler models
    

### ✔ Use **Feature Extraction** when:

- Many correlated features exist
    
- Need dimensionality reduction (e.g., images)
    
- PCA visualization is needed
    

---

# ============================

# **MCQs — Feature Selection & Extraction (20)**

# ============================

### **MCQ 1**

Feature selection chooses:

-  New transformed features
    
-  Best subset of existing features
    
-  Random features
    
-  Target variables  
    **Answer:** Best subset of existing features
    

---

### **MCQ 2**

Which method removes least important features iteratively?

-  PCA
    
-  RFE
    
-  Chi-square
    
-  t-SNE  
    **Answer:** RFE
    

---

### **MCQ 3**

Lasso regression performs:

-  L2 regularization
    
-  L1 regularization
    
-  No regularization
    
-  Encoding  
    **Answer:** L1 regularization
    

---

### **MCQ 4**

Which feature selection method is model-independent?

-  Wrapper
    
-  Embedded
    
-  Filter
    
-  Neural networks  
    **Answer:** Filter
    

---

### **MCQ 5**

Chi-square test is used for:

-  Numerical-numerical
    
-  Categorical-numerical
    
-  Categorical-categorical
    
-  Image data  
    **Answer:** Categorical-categorical
    

---

### **MCQ 6**

Which method is computationally expensive?

-  Filter
    
-  Wrapper
    
-  Standardization
    
-  RFE  
    **Answer:** Wrapper
    

---

### **MCQ 7**

Which technique creates new features?

-  RFE
    
-  PCA
    
-  Lasso
    
-  ANOVA  
    **Answer:** PCA
    

---

### **MCQ 8**

Tree-based models provide:

-  Encoders
    
-  Feature importance
    
-  Missing values
    
-  Scaling  
    **Answer:** Feature importance
    

---

### **MCQ 9**

Backward elimination starts with:

-  Zero features
    
-  All features
    
-  Random features
    
-  PCA components  
    **Answer:** All features
    

---

### **MCQ 10**

Forward selection starts with:

-  All features
    
-  Zero features
    
-  Lasso regression
    
-  Only categorical features  
    **Answer:** Zero features
    

---

### **MCQ 11**

PCA components are:

-  Correlated
    
-  Orthogonal
    
-  Random
    
-  Categorical  
    **Answer:** Orthogonal
    

---

### **MCQ 12**

t-SNE is mainly used for:

-  Classification
    
-  Visualization
    
-  Regularization
    
-  Encoding  
    **Answer:** Visualization
    

---

### **MCQ 13**

Mutual information measures:

-  Covariance
    
-  Shared information
    
-  Missingness
    
-  Distances  
    **Answer:** Shared information
    

---

### **MCQ 14**

LDA is a:

-  Supervised technique
    
-  Unsupervised technique
    
-  Reinforcement technique
    
-  Dimensionality reduction for PCA  
    **Answer:** Supervised technique
    

---

### **MCQ 15**

Which technique is ideal for image compression?

-  Decision trees
    
-  Autoencoders
    
-  Forward selection
    
-  ANOVA  
    **Answer:** Autoencoders
    

---

### **MCQ 16**

Feature extraction reduces:

-  Training accuracy
    
-  Dimensionality
    
-  Hyperparameters
    
-  Missing values  
    **Answer:** Dimensionality
    

---

### **MCQ 17**

Wrapper methods use:

-  Neural networks
    
-  ML models to evaluate features
    
-  Statistics only
    
-  PCA  
    **Answer:** ML models to evaluate features
    

---

### **MCQ 18**

Filter methods rely on:

-  Model training
    
-  Statistical scores
    
-  Backpropagation
    
-  Tree importance  
    **Answer:** Statistical scores
    

---

### **MCQ 19**

Feature reduction helps reduce:

-  Overfitting
    
-  Labels
    
-  Clustering
    
-  Missing values  
    **Answer:** Overfitting
    

---

### **MCQ 20**

Feature selection should NOT be used when:

-  Interpretability is required
    
-  Features are correlated
    
-  Dataset is small
    
-  New complex features are needed  
    **Answer:** New complex features are needed
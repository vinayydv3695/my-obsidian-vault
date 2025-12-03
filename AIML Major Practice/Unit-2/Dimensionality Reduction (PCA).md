
# 📌 **1. What is Dimensionality Reduction?**

Dimensionality reduction reduces the number of input features while preserving the important information.

### Why needed?

- High-dimensional data → computationally expensive
    
- Reduces overfitting
    
- Removes noise
    
- Improves visualization
    
- Faster ML training
    

---

# ============================

# **2. Principal Component Analysis (PCA)**

# ============================

PCA is the most widely used dimensionality reduction technique.

PCA transforms original features into a new set of **orthogonal components** called **principal components (PCs)**.

---

# 📌 **3. Goals of PCA**

- Reduce dimensionality
    
- Retain maximum variance
    
- Remove feature correlation
    
- Compress data
    

---

# 📌 **4. How PCA Works (Step-by-Step)**

### **Step 1: Standardize the Data**

Because PCA is sensitive to scale.

### **Step 2: Compute Covariance Matrix**

Shows relationships between features.

### **Step 3: Compute Eigenvalues & Eigenvectors**

- Eigenvalues → amount of variance
    
- Eigenvectors → direction of components
    

### **Step 4: Choose Top k Components**

Select components with the highest variance.

### **Step 5: Transform the Data**

Project onto the new subspace.

---

# 📌 **5. Important Concepts**

### **A) Principal Component**

A new feature that captures maximum variance.

### **B) Eigenvalue**

Represents variance explained by its principal component.

### **C) Scree Plot**

Graph showing eigenvalues → used to select number of components.

### **D) Explained Variance Ratio**

Percentage of variance each principal component explains.

---

# 📌 **6. Pros of PCA**

✔ Reduces dimensionality  
✔ Removes multicollinearity  
✔ Improves algorithm speed  
✔ Useful for visualization (2D/3D)

---

# 📌 **7. Cons of PCA**

✘ Components are not interpretable  
✘ Loses original meaning of features  
✘ Only captures linear relationships  
✘ Scaling required

---

# 📌 **8. When to Use PCA?**

- Many correlated features
    
- Need faster training
    
- Need visualization in 2D or 3D
    
- Remove noise
    
- Avoid overfitting
    

---

# 📌 **9. When NOT to Use PCA?**

- When interpretability is important
    
- Data is categorical
    
- Data is not scaled
    
- Non-linear relationships → use t-SNE or UMAP
    

---

# ============================

# **MCQs — Dimensionality Reduction (PCA) (20)**

# ============================

### **MCQ 1**

PCA reduces dimensionality by:

-  Removing rows
    
-  Creating new uncorrelated features
    
-  Filling missing values
    
-  Adding noise  
    **Answer:** Creating new uncorrelated features
    

---

### **MCQ 2**

PCA components are:

-  Categorical
    
-  Orthogonal
    
-  Correlated
    
-  Identical  
    **Answer:** Orthogonal
    

---

### **MCQ 3**

PCA maximizes:

-  Covariance
    
-  Variance
    
-  Error
    
-  Noise  
    **Answer:** Variance
    

---

### **MCQ 4**

Which plot is used to select number of components?

-  Histogram
    
-  Scree plot
    
-  Box plot
    
-  Heatmap  
    **Answer:** Scree plot
    

---

### **MCQ 5**

Eigenvalues represent:

-  Skewness
    
-  Variance explained
    
-  Mean shift
    
-  Range  
    **Answer:** Variance explained
    

---

### **MCQ 6**

Before applying PCA, we must:

-  Normalize or standardize data
    
-  Remove all outliers
    
-  Apply one-hot encoding
    
-  Fill missing values only  
    **Answer:** Normalize or standardize data
    

---

### **MCQ 7**

PCA fails when data:

-  Has linear correlation
    
-  Has non-linear relationships
    
-  Is numeric
    
-  Is balanced  
    **Answer:** Has non-linear relationships
    

---

### **MCQ 8**

Components in PCA are also called:

-  Scores
    
-  Loadings
    
-  Principal Components
    
-  Factors  
    **Answer:** Principal Components
    

---

### **MCQ 9**

PCA removes:

-  Outliers
    
-  Multicollinearity
    
-  Categories
    
-  Missing values  
    **Answer:** Multicollinearity
    

---

### **MCQ 10**

The first principal component captures:

-  Least variance
    
-  Maximum variance
    
-  Random information
    
-  Noise  
    **Answer:** Maximum variance
    

---

### **MCQ 11**

PCA transforms data using:

-  Eigenvectors
    
-  Means
    
-  Boxplots
    
-  Mode  
    **Answer:** Eigenvectors
    

---

### **MCQ 12**

PCA is NOT suitable for:

-  Numerical data
    
-  Categorical data
    
-  High-dimensional data
    
-  Correlated data  
    **Answer:** Categorical data
    

---

### **MCQ 13**

Dimensionality reduction helps prevent:

-  Underfitting
    
-  Overfitting
    
-  Data leakage
    
-  Missing values  
    **Answer:** Overfitting
    

---

### **MCQ 14**

If PCA reduces features from 50 to 5, it means:

-  5 features explain most variance
    
-  Data is deleted
    
-  Total loss of information
    
-  Scaling failed  
    **Answer:** 5 features explain most variance
    

---

### **MCQ 15**

Explained variance ratio tells:

-  Distribution
    
-  Percentage of variance captured
    
-  Standard deviation
    
-  Noise ratio  
    **Answer:** Percentage of variance captured
    

---

### **MCQ 16**

PCA is a:

-  Supervised method
    
-  Unsupervised method
    
-  Regression method
    
-  Classification method  
    **Answer:** Unsupervised method
    

---

### **MCQ 17**

PCA requires features to be:

-  Correlated
    
-  Missing
    
-  Noisy
    
-  Categorical  
    **Answer:** Correlated
    

---

### **MCQ 18**

Which ML model benefits most from PCA?

-  KNN
    
-  Decision trees
    
-  Random forest
    
-  Naive Bayes  
    **Answer:** KNN
    

---

### **MCQ 19**

PCA components are ranked by:

-  Mean
    
-  Variance explained
    
-  Skew
    
-  Frequency  
    **Answer:** Variance explained
    

---

### **MCQ 20**

The main disadvantage of PCA:

-  Too fast
    
-  Hard to interpret components
    
-  Requires labels
    
-  Works only for text  
    **Answer:** Hard to interpret components
    

---
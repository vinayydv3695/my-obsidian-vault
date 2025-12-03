
# **1. Standardization (Z-Score Scaling)**

Standardization transforms data so that it has:

- **Mean = 0**
    
- **Standard deviation = 1**
    

### Formula:

`z = (x − μ) / σ`

### When to Use:

- When data contains **outliers**
    
- When feature scales differ
    
- For ML algorithms that assume normality:
    
    - Logistic Regression
        
    - Linear Regression
        
    - SVM
        
    - KNN
        
    - Neural Networks
        

### Characteristics:

- Does **not** squash data to a fixed range
    
- Robust for many ML algorithms
    

---

# 📌 **2. Normalization (Min–Max Scaling)**

Normalization rescales values to a fixed range:  
**[0, 1]**

### Formula:

`x' = (x − min) / (max − min)`

### When to Use:

- Neural networks (sigmoid, tanh, ReLU)
    
- Distance-based models:
    
    - KNN
        
    - K-Means
        
    - SVM (RBF kernel)
        

### Characteristics:

- Sensitive to outliers
    
- Preserves data distribution shape
    

---

# 📌 **3. Data Smoothing**

Data smoothing reduces **noise** in data.

### Common Smoothing Techniques:

### **a) Moving Average**

`New value = average of last k values`

Used in time-series.

### **b) Binning (Equal-width / Equal-frequency)**

- Group values into bins
    
- Replace values with bin mean, median, or boundary
    

### **c) LOESS / LOWESS**

Locally weighted regression curves.

### **d) Exponential Smoothing**

Weights recent values more:

`S_t = αX_t + (1 − α)S_(t−1)`

### Why Smoothing?

✔ Removes random fluctuations  
✔ Makes trends clearer  
✔ Helps models generalize better

---

# 📌 **4. Standardization vs Normalization — Quick Comparison**

|Property|Standardization|Normalization|
|---|---|---|
|Output Range|Unbounded|0 to 1|
|Affected by Outliers?|Less|Highly|
|Best for|Linear models, SVM, KNN|Neural networks|
|Distribution Assumption|Normal|None|

---

# 📌 **5. Why Scaling Is Important?**

✔ Improves gradient descent convergence  
✔ Prevents one feature from dominating  
✔ Improves accuracy of distance-based methods  
✔ Stabilizes training

---

# ============================

# **MCQs — Standardization, Normalization & Smoothing (20)**

# ============================

### **MCQ 1**

Standardization transforms data to have:

-  Mean = 1
    
-  Mean = 0
    
-  Std = 5
    
-  Max = 1  
    **Answer:** Mean = 0
    

---

### **MCQ 2**

Which scaling technique produces values in [0, 1]?

-  Z-score
    
-  Min–max
    
-  Log transform
    
-  Binning  
    **Answer:** Min–max
    

---

### **MCQ 3**

Standardization is also known as:

-  Min-max scaling
    
-  Z-score scaling
    
-  Log scaling
    
-  Encoding  
    **Answer:** Z-score scaling
    

---

### **MCQ 4**

Normalization is sensitive to:

-  Missing values
    
-  Duplicates
    
-  Outliers
    
-  Timestamps  
    **Answer:** Outliers
    

---

### **MCQ 5**

Which algorithm requires normalization the most?

-  Decision trees
    
-  Random forest
    
-  KNN
    
-  Naive Bayes  
    **Answer:** KNN
    

---

### **MCQ 6**

Which algorithm benefits from standardization?

-  Logistic Regression
    
-  Decision Trees
    
-  Random Forest
    
-  Naive Bayes  
    **Answer:** Logistic Regression
    

---

### **MCQ 7**

Data smoothing is used to remove:

-  Missing values
    
-  Duplicates
    
-  Noise
    
-  Labels  
    **Answer:** Noise
    

---

### **MCQ 8**

Binning is a technique used in:

-  Scaling
    
-  Encoding
    
-  Smoothing
    
-  Feature extraction  
    **Answer:** Smoothing
    

---

### **MCQ 9**

Moving average is used for:

-  Clustering
    
-  Spectral analysis
    
-  Time-series smoothing
    
-  Regression  
    **Answer:** Time-series smoothing
    

---

### **MCQ 10**

Min-max scaling formula is:

-  (x - μ) / σ
    
-  (x - min) / (max - min)
    
-  log(x)
    
-  x²  
    **Answer:** (x - min) / (max - min)
    

---

### **MCQ 11**

Z-score scaling requires computing:

-  Only min
    
-  Only max
    
-  Mean and standard deviation
    
-  Range  
    **Answer:** Mean and standard deviation
    

---

### **MCQ 12**

Which method reduces skewness?

-  Binning
    
-  Log transform
    
-  Standardization
    
-  Min-max  
    **Answer:** Log transform
    

---

### **MCQ 13**

Which technique is NOT a smoothing method?

-  Moving average
    
-  Exponential smoothing
    
-  LOESS
    
-  One-hot encoding  
    **Answer:** One-hot encoding
    

---

### **MCQ 14**

Normalization rescales values to:

-  Mean zero
    
-  Unit variance
    
-  Fixed range
    
-  Infinite range  
    **Answer:** Fixed range
    

---

### **MCQ 15**

Standardization is preferred over normalization when:

-  Outliers exist
    
-  Data has no outliers
    
-  Data is categorical
    
-  Data is very small  
    **Answer:** Outliers exist
    

---

### **MCQ 16**

Smoothing improves:

-  Data noise
    
-  Encoding
    
-  Scaling
    
-  Feature count  
    **Answer:** Data noise
    

---

### **MCQ 17**

Exponential smoothing assigns more weight to:

-  Older values
    
-  All values equally
    
-  Recent values
    
-  Categorical values  
    **Answer:** Recent values
    

---

### **MCQ 18**

Which scaling method is often used with Neural Networks?

-  Standardization
    
-  Normalization
    
-  Binning
    
-  PCA  
    **Answer:** Normalization
    

---

### **MCQ 19**

LOESS is primarily used for:

-  Local smoothing
    
-  Encoding
    
-  Classification
    
-  Feature extraction  
    **Answer:** Local smoothing
    

---

### **MCQ 20**

Which scaling technique keeps outliers but reduces their influence?

-  Min-max
    
-  Standardization
    
-  One-hot
    
-  Binning  
    **Answer:** Standardization
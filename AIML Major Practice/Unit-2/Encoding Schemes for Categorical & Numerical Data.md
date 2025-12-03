
# **1. Why Encoding is Needed?**

Most ML models cannot work directly with text labels or categories.  
Encoding converts categorical/numerical formats into **machine-readable numeric values**.

Used in:

- Classification
    
- Regression
    
- NLP
    
- Recommendation engines
    

---

# ============================

# **2. Types of Categorical Encoding**

# ============================

# 📌 **A) Label Encoding**

Each category → unique integer.

Example:

`Red → 0   Blue → 1   Green → 2`

### Pros:

✔ Simple  
✔ No extra columns

### Cons:

✘ Implies **ordinal relationship** even if none exists  
✘ Not suitable for nominal categories with no order

Used in:

- Decision trees
    
- XGBoost
    
- LightGBM
    

---

# 📌 **B) One-Hot Encoding**

Converts each category into a **binary (0/1) column**.

Example:

`Color_Red   Color_Blue   Color_Green     1            0            0`

### Pros:

✔ No ordinal assumptions  
✔ Works well for linear models & NN

### Cons:

✘ Increases dimensionality  
✘ Not ideal for high-cardinality columns

---

# 📌 **C) Ordinal Encoding**

Used when categories have natural order.

Example:

`Small=1, Medium=2, Large=3`

### Pros:

✔ Preserves order  
✔ Compact

### Cons:

✘ Not valid for nominal data

---

# 📌 **D) Target Encoding**

Replace category with **mean of target variable** for that category.

Example:  
For category "A":

`Target Mean of A = 0.78`

### Pros:

✔ Works well for high-cardinality data  
✔ Used in Kaggle competitions

### Cons:

✘ Risk of overfitting  
✘ Needs smoothing & cross-validation

---

# 📌 **E) Frequency / Count Encoding**

Replace category with its frequency (count).

### Pros:

✔ Low dimensionality  
✔ Captures importance

### Cons:

✘ Might not work for purely nominal categories

---

# 📌 **F) Binary Encoding**

Category → integer → binary form.

Example:

`5 → 101`

More compact than one-hot.

---

# 📌 **G) Hash Encoding**

Used for VERY high-cardinality data (e.g., text features).

✔ Fast  
✔ Fixed output dimensions

✘ Hash collisions may occur

---

# ============================

# **3. Numerical Encoding (Binning)**

# ============================

# 📌 **A) Equal-Width Binning**

Divide numeric range into equal intervals.

Example:

`0-10, 10-20, 20-30`

# 📌 **B) Equal-Frequency Binning**

Each bin has equal number of samples.

Better for skewed data.

# 📌 **C) Custom Binning**

Domain expert decides boundaries (e.g., age groups).

---

# ============================

# **4. Scaling vs Encoding**

Encoding = for categorical data  
Scaling = for numerical data

They serve different purposes.

---

# ============================

# **5. Which Encoding to Use When?**

|Situation|Best Encoding|
|---|---|
|Nominal data|One-hot, Binary|
|Ordinal data|Ordinal encoding|
|High-cardinality|Target, Hash, Count encoding|
|Tree-based models|Label encoding|
|Linear models|One-hot encoding|

---

# ============================

# **MCQs — Encoding Schemes (20)**

# ============================

### **MCQ 1**

Label encoding is mainly used for:

-  Ordinal data
    
-  Nominal data
    
-  Image data
    
-  Time-series  
    **Answer:** Ordinal data
    

---

### **MCQ 2**

One-hot encoding increases:

-  Missing values
    
-  Dimensionality
    
-  Outliers
    
-  Noise  
    **Answer:** Dimensionality
    

---

### **MCQ 3**

One-hot encoding is best for:

-  Ordered categories
    
-  Unordered categories
    
-  Numerical columns
    
-  Missing values  
    **Answer:** Unordered categories
    

---

### **MCQ 4**

Ordinal encoding preserves:

-  Distance
    
-  Order
    
-  Noise
    
-  Missingness  
    **Answer:** Order
    

---

### **MCQ 5**

Target encoding replaces categories with:

-  Binary values
    
-  Mean of target
    
-  Random numbers
    
-  Z-scores  
    **Answer:** Mean of target
    

---

### **MCQ 6**

A major disadvantage of target encoding:

-  Slow
    
-  High dimensionality
    
-  Overfitting
    
-  Cannot be used in ML  
    **Answer:** Overfitting
    

---

### **MCQ 7**

Binary encoding is more compact than:

-  One-hot encoding
    
-  Ordinal encoding
    
-  Z-score
    
-  Min-max scaling  
    **Answer:** One-hot encoding
    

---

### **MCQ 8**

Hash encoding can cause:

-  Missing values
    
-  Noise
    
-  Hash collisions
    
-  Extra labels  
    **Answer:** Hash collisions
    

---

### **MCQ 9**

Count encoding replaces categories by:

-  Average
    
-  Median
    
-  Frequency
    
-  Maximum  
    **Answer:** Frequency
    

---

### **MCQ 10**

Tree-based models (XGBoost, Random Forest) prefer:

-  One-hot encoding
    
-  Label encoding
    
-  Binary encoding
    
-  None  
    **Answer:** Label encoding
    

---

### **MCQ 11**

One-hot encoding leads to what issue?

-  Data leakage
    
-  Curse of dimensionality
    
-  Overfitting
    
-  Undersampling  
    **Answer:** Curse of dimensionality
    

---

### **MCQ 12**

Ordinal encoding should NOT be used for:

-  Education levels
    
-  Days of week
    
-  Colors
    
-  Rating scales  
    **Answer:** Colors
    

---

### **MCQ 13**

Normalization is applied to:

-  Categorical features
    
-  Numerical features
    
-  Missing features
    
-  Encoded text  
    **Answer:** Numerical features
    

---

### **MCQ 14**

High-cardinality categorical features should use:

-  One-hot
    
-  Hash or Target encoding
    
-  Ordinal encoding
    
-  Linear regression  
    **Answer:** Hash or Target encoding
    

---

### **MCQ 15**

Binning converts numeric data into:

-  Text
    
-  Categorical bins
    
-  Images
    
-  Missing values  
    **Answer:** Categorical bins
    

---

### **MCQ 16**

Equal-frequency binning:

-  Maintains equal ranges
    
-  Ensures equal sample count per bin
    
-  Removes duplicates
    
-  Encodes labels  
    **Answer:** Ensures equal sample count per bin
    

---

### **MCQ 17**

Label encoding can mislead models because:

-  It removes classes
    
-  It introduces artificial order
    
-  It increases noise
    
-  It reduces variance  
    **Answer:** It introduces artificial order
    

---

### **MCQ 18**

One-hot encoding is ideal for:

-  Linear regression and logistic regression
    
-  Decision trees
    
-  Isolation forests
    
-  PCA  
    **Answer:** Linear regression and logistic regression
    

---

### **MCQ 19**

Binary encoding reduces dimensions by:

-  Splitting columns
    
-  Using binary representation
    
-  Removing noise
    
-  Smoothing out categories  
    **Answer:** Using binary representation
    

---

### **MCQ 20**

Which encoding should NOT be used for neural networks?

-  One-hot encoding
    
-  Ordinal encoding
    
-  Target encoding
    
-  Label encoding  
    **Answer:** Ordinal encoding
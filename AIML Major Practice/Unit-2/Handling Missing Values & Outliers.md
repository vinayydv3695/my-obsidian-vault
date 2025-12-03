# **1. Why Missing Values Occur?**

Missing values appear due to:

- Human entry errors
    
- Sensor failure
    
- Data corruption
    
- Incomplete surveys
    
- System crashes
    

Missing values cause:  
✘ Biased models  
✘ Incorrect predictions  
✘ Failure of ML algorithms

---

# 📌 **2. Types of Missing Data**

### **1. MCAR — Missing Completely at Random**

Missingness is unrelated to any feature or target.

Example: Sensor failed randomly.

### **2. MAR — Missing at Random**

Missingness depends on **other features**, not the missing feature.

Example: Older people skip income field more often.

### **3. MNAR — Missing Not at Random**

Missingness depends on the **missing value itself**.

Example: People with high income do not disclose salary.

MNAR is the hardest to handle.

---

# 📌 **3. Handling Missing Values**

## **A) Deletion Methods**

### **1. Listwise Deletion (Drop Rows)**

Remove rows with missing values.

✔ Simple  
✔ Good when % missing is low

✘ Loses data  
✘ Not suitable for small datasets

### **2. Column Deletion**

Remove features with too many missing values (> 60–70%).

✔ Removes useless features  
✘ Risk of losing important signal

---

## **B) Imputation Methods**

### **1. Mean Imputation**

Fill missing values with the **mean**.

Works for:

- Numerical data
    
- Normally distributed features
    

### **2. Median Imputation**

Useful when:

- Data has outliers
    
- Skewed data
    

### **3. Mode Imputation**

For categorical features.

---

## **C) Advanced Imputation**

### **1. KNN Imputation**

Fills missing value based on nearest neighbors.

✔ Accurate  
✘ Slow for large datasets

### **2. Regression Imputation**

Predict missing values using regression models.

### **3. MICE (Multiple Imputation by Chained Equations)**

Multiple models build multiple imputations.

✔ Best for complex datasets

---

# 📌 **4. Handling Outliers**

Outliers = extreme values far from the rest of the data.

Outliers cause:

- Skewed distributions
    
- Wrong model coefficients
    
- Incorrect scaling
    

---

## **A) Detection Methods**

### **1. Z-Score Method**

`Z = (x − μ) / σ Outlier if |Z| > 3`

### **2. IQR Method**

`IQR = Q3 − Q1 Lower Bound = Q1 − 1.5 * IQR Upper Bound = Q3 + 1.5 * IQR`

### **3. Box Plot**

Visual detection.

### **4. Isolation Forest**

ML-based outlier detection.

---

## **B) Handling Outliers**

### **1. Removal**

Delete outlier rows.

### **2. Capping (Winsorization)**

Replace outliers with boundary values:

- 5th percentile
    
- 95th percentile
    

### **3. Transformation**

Log, sqrt, or box-cox transforms reduce extreme values.

### **4. Binning**

Group extreme values into bins.

---

# 📌 **5. When NOT to Remove Outliers**

- Outliers are meaningful (fraud, disease indicators)
    
- Data represents heavy-tailed distribution
    
- Outliers carry important signals
    

---

# ============================

# **MCQs — Handling Missing Values & Outliers (20)**

# ============================

### **MCQ 1**

Mean imputation is suitable for:

-  Categorical data
    
-  Normally distributed numeric data
    
-  Text data
    
-  Images  
    **Answer:** Normally distributed numeric data
    

---

### **MCQ 2**

Median imputation is preferred when:

-  Data is symmetric
    
-  Data has outliers
    
-  Data is categorical
    
-  No missing values  
    **Answer:** Data has outliers
    

---

### **MCQ 3**

MCAR means missingness is:

-  Based on missing value
    
-  Random
    
-  Based on another feature
    
-  None  
    **Answer:** Random
    

---

### **MCQ 4**

MAR means missingness depends on:

-  The missing value
    
-  Other variables
    
-  Noise
    
-  Outliers  
    **Answer:** Other variables
    

---

### **MCQ 5**

MNAR refers to missingness depending on:

-  Target variable
    
-  The value itself
    
-  Columns
    
-  Noise  
    **Answer:** The value itself
    

---

### **MCQ 6**

Dropping rows with missing values is useful when:

-  Missing % is very high
    
-  Missing % is very low
    
-  Dataset is small
    
-  Column is categorical  
    **Answer:** Missing % is very low
    

---

### **MCQ 7**

Mode imputation is used for:

-  Numerical values
    
-  Categorical values
    
-  Time-series
    
-  Images  
    **Answer:** Categorical values
    

---

### **MCQ 8**

KNN imputation works by:

-  Random guessing
    
-  Using nearest neighbors
    
-  Using regression
    
-  Using PCA  
    **Answer:** Using nearest neighbors
    

---

### **MCQ 9**

IQR method labels an outlier if:

-  |Z| > 2
    
-  It is outside (Q1 − 1.5×IQR, Q3 + 1.5×IQR)
    
-  Value is 0
    
-  Data is missing  
    **Answer:** It is outside the IQR boundary
    

---

### **MCQ 10**

Z-score > 3 indicates:

-  Normal value
    
-  Missing value
    
-  Possible outlier
    
-  Categorical value  
    **Answer:** Possible outlier
    

---

### **MCQ 11**

Capping outliers is also called:

-  Encoding
    
-  Scaling
    
-  Winsorization
    
-  Binning  
    **Answer:** Winsorization
    

---

### **MCQ 12**

Which technique reduces outlier impact?

-  Log transformation
    
-  Standardization
    
-  One-hot encoding
    
-  PCA  
    **Answer:** Log transformation
    

---

### **MCQ 13**

Should outliers in fraud datasets be removed?

-  Yes
    
-  No
    
-  Sometimes
    
-  Only if small  
    **Answer:** No
    

---

### **MCQ 14**

Which method predicts missing values?

-  Deletion
    
-  Regression imputation
    
-  Noise addition
    
-  Capping  
    **Answer:** Regression imputation
    

---

### **MCQ 15**

MICE stands for:

-  Multi-layer Imputation for Clean Environment
    
-  Multiple Imputation by Chained Equations
    
-  Machine Imputation Confidence Estimation
    
-  Multi Input Correction Engine  
    **Answer:** Multiple Imputation by Chained Equations
    

---

### **MCQ 16**

Outlier removal should be avoided when:

-  Outliers indicate fraud
    
-  Outliers are noise
    
-  Outliers create bias
    
-  Data is symmetric  
    **Answer:** Outliers indicate fraud
    

---

### **MCQ 17**

Which algorithm is good for outlier detection?

-  Logistic Regression
    
-  Isolation Forest
    
-  Naive Bayes
    
-  PCA  
    **Answer:** Isolation Forest
    

---

### **MCQ 18**

A column with 80% missing values should be:

-  Standardized
    
-  Deleted
    
-  Encoded
    
-  Smoothed  
    **Answer:** Deleted
    

---

### **MCQ 19**

Missing values in time-series can be handled using:

-  Interpolation
    
-  One-hot encoding
    
-  PCA
    
-  Scaling  
    **Answer:** Interpolation
    

---

### **MCQ 20**

Smoothing helps by:

-  Adding noise
    
-  Reducing noise
    
-  Increasing dimensionality
    
-  Removing categories  
    **Answer:** Reducing noise
    

---
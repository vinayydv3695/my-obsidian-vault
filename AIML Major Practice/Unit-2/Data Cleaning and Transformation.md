
## 1. What is Data Cleaning?

Data cleaning refers to identifying and correcting errors, inconsistencies, and incomplete data before applying ML models.

### Goals of Data Cleaning:

- Improve data quality
    
- Remove noise
    
- Fix inconsistencies
    
- Prepare data for modeling
    

---

## 2. Common Data Cleaning Tasks

### **a) Handling Missing Data**

- Drop missing values
    
- Fill using mean/median/mode
    
- Predict missing values
    
- Use interpolation (time-series)
    

---

### **b) Handling Duplicates**

- Detect using `.duplicate()`
    
- Remove duplicates if unnecessary
    

---

### **c) Fixing Inconsistencies**

- Standardizing units (kg vs pounds)
    
- Converting formats (DD/MM vs MM/DD)
    
- Correcting typos
    

---

### **d) Handling Noise**

Noise = random errors in data.

Noise reduction techniques:

- Smoothing
    
- Binning
    
- Aggregation
    
- Outlier removal
    

---

## 3. Data Transformation

Transformation modifies the data format or structure to improve performance.

### **a) Scaling**

Changes range of data (Standardization, Normalization).

### **b) Encoding**

Convert categories into numbers.

### **c) Aggregation**

Summarizing data values:

- Mean
    
- Sum
    
- Min/Max
    

### **d) Discretization**

Convert continuous → categorical (e.g., age groups)

### **e) Log Transform**

Reduces skew in highly skewed data.

---

## 4. Why Data Cleaning & Transformation are Important?

✔ Improves model accuracy  
✔ Reduces training time  
✔ Prevents incorrect predictions  
✔ Avoids model bias  
✔ Necessary for ML algorithms to work correctly

---

# 📌 **MCQs — Data Cleaning & Transformation (20)**

### **MCQ 1**

Data cleaning is performed to:

-  Increase missing values
    
-  Improve data quality
    
-  Remove model accuracy
    
-  Add noise  
    **Answer:** Improve data quality
    

---

### **MCQ 2**

Removing duplicated rows is part of:

-  Feature scaling
    
-  Data cleaning
    
-  Model training
    
-  Regularization  
    **Answer:** Data cleaning
    

---

### **MCQ 3**

Fixing inconsistent units belongs to:

-  Data visualization
    
-  Data cleaning
    
-  Dimensionality reduction
    
-  Feature extraction  
    **Answer:** Data cleaning
    

---

### **MCQ 4**

Scaling (Standardization/Normalization) is a type of:

-  Data cleaning
    
-  Data transformation
    
-  Model tuning
    
-  Encoding  
    **Answer:** Data transformation
    

---

### **MCQ 5**

Binning is used for:

-  Feature splitting
    
-  Noise reduction
    
-  Dimensionality reduction
    
-  Outlier creation  
    **Answer:** Noise reduction
    

---

### **MCQ 6**

Replacing missing values with mean is known as:

-  Encoding
    
-  Imputation
    
-  Smoothing
    
-  Normalization  
    **Answer:** Imputation
    

---

### **MCQ 7**

Log transformation is useful when data is:

-  Normally distributed
    
-  Categorical
    
-  Highly skewed
    
-  Missing  
    **Answer:** Highly skewed
    

---

### **MCQ 8**

Outliers can be handled by:

-  PCA
    
-  Capping or flooring
    
-  One-hot encoding
    
-  Logistic regression  
    **Answer:** Capping or flooring
    

---

### **MCQ 9**

Changing date formats (DD/MM → MM/DD) is:

-  Encoding
    
-  Cleaning
    
-  Scaling
    
-  Feature extraction  
    **Answer:** Cleaning
    

---

### **MCQ 10**

Noise refers to:

-  Missing values
    
-  Random errors in data
    
-  Duplicate rows
    
-  Encoded categories  
    **Answer:** Random errors in data
    

---

### **MCQ 11**

The process of converting continuous data into categories is:

-  Discretization
    
-  Normalization
    
-  PCA
    
-  Aggregation  
    **Answer:** Discretization
    

---

### **MCQ 12**

Aggregation is used to:

-  Increase noise
    
-  Summarize data
    
-  Encode categories
    
-  Add missing features  
    **Answer:** Summarize data
    

---

### **MCQ 13**

Which method removes skewness?

-  One-hot encoding
    
-  Normalization
    
-  Log transformation
    
-  PCA  
    **Answer:** Log transformation
    

---

### **MCQ 14**

Data cleaning must be done:

-  After model training
    
-  Before model training
    
-  After prediction
    
-  Never  
    **Answer:** Before model training
    

---

### **MCQ 15**

Imputation helps in handling:

-  Duplicates
    
-  Missing values
    
-  Encoding
    
-  Outliers  
    **Answer:** Missing values
    

---

### **MCQ 16**

Removing noise improves:

-  Overfitting
    
-  Model interpretability
    
-  Data quality
    
-  GPU utilization  
    **Answer:** Data quality
    

---

### **MCQ 17**

Which is NOT a transformation method?

-  Normalization
    
-  Standardization
    
-  Discretization
    
-  Model tuning  
    **Answer:** Model tuning
    

---

### **MCQ 18**

Which is an example of data inconsistency?

-  Missing values
    
-  "kg" vs "Kilogram"
    
-  Duplicate rows
    
-  Log transform  
    **Answer:** "kg" vs "Kilogram"
    

---

### **MCQ 19**

Data smoothing removes:

-  Missing values
    
-  Noise
    
-  Labels
    
-  Target values  
    **Answer:** Noise
    

---

### **MCQ 20**

Cleaning and transformation together improve:

-  Only accuracy
    
-  Both accuracy and reliability
    
-  Only training speed
    
-  Only outliers  
    **Answer:** Both accuracy and reliability
    

---
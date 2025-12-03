
Evaluation metrics measure how well a machine-learning model performs.  
They depend on whether the task is:

- **Regression** (predicting numbers)
    
- **Classification** (predicting classes)
    

---

# ===========================

# 📌 PART 1 — REGRESSION METRICS

# ===========================

# **1. Mean Squared Error (MSE)**

Measures the average squared difference between predicted and actual values.

```
MSE = (1/n) Σ (Yi − Ŷi)²
```

### Key Points:

- Penalizes large errors heavily
    
- Sensitive to outliers
    
- Lower MSE = better
    

---

# **2. Root Mean Squared Error (RMSE)**

Square root of MSE.

```
RMSE = √MSE
```

### Key Points:

- Same units as target variable
    
- Easier to interpret
    
- Often used in real-world regression
    

---

# **3. Mean Absolute Error (MAE)**

Measures average absolute error.

```
MAE = (1/n) Σ |Yi − Ŷi|
```

### Key Points:

- Less sensitive to outliers
    
- More robust metric
    
- Linear penalty
    

---

# **4. R² Score (Coefficient of Determination)**

Measures how much variance is explained by the model.

```
R² = 1 − (SS_res / SS_tot)
```

### Key Points:

- 1 = perfect
    
- 0 = no better than mean
    
- < 0 = worse than mean model
    

---

# **5. Adjusted R²**

Corrects R² for multiple predictors.

```
Adjusted R² = 1 − [(1 − R²)(n − 1) / (n − k − 1)]
```

Where **k = number of predictors**.

### Key Points:

- Increases only when new feature improves the model
    
- Preferred for Multiple Linear Regression
    

---

# ===========================

# 📌 PART 2 — CLASSIFICATION METRICS

# ===========================

A confusion matrix is the base for all classification metrics.

```
               Predicted
              Pos   Neg
Actual Pos    TP    FN
       Neg    FP    TN
```

---

# **1. Accuracy**

```
Accuracy = (TP + TN) / Total
```

### Key Points:

- Overall correctness
    
- Misleading for imbalance
    

---

# **2. Precision**

```
Precision = TP / (TP + FP)
```

### Key Points:

- Out of predicted positives, how many are correct?
    
- High precision → few false positives (FP)
    

---

# **3. Recall (Sensitivity / True Positive Rate)**

```
Recall = TP / (TP + FN)
```

### Key Points:

- Out of actual positives, how many did we catch?
    
- High recall → few false negatives (FN)
    

---

# **4. F1 Score**

```
F1 = 2 * (Precision * Recall) / (Precision + Recall)
```

### Key Points:

- Harmonic mean
    
- Best when classes are imbalanced
    

---

# **5. Specificity (True Negative Rate)**

```
Specificity = TN / (TN + FP)
```

### Key Points:

- Measures how well negatives are identified
    

---

# **6. False Positive Rate (FPR)**

```
FPR = FP / (FP + TN)
```

---

# **7. False Negative Rate (FNR)**

```
FNR = FN / (TP + FN)
```

---

# **8. ROC Curve (Receiver Operating Characteristic)**

Plots **TPR vs FPR** for different thresholds.

### Key Points:

- Threshold-independent
    
- Helps compare classifiers
    

---

# **9. AUC (Area Under Curve)**

Measures separability of classes.

- 1 → perfect
    
- 0.5 → random
    
- < 0.5 → worse than random
    

---

# ===========================

# 📌 PART 3 — METRIC SELECTION

# ===========================

### **Use MAE when:**

- Outliers present
    
- Need robustness
    

### **Use RMSE when:**

- Large errors must be penalized
    

### **Use R² when:**

- Want to measure explanatory power
    

### **Use Accuracy when:**

- Data is balanced
    

### **Use Precision when:**

- False positives are costly (e.g., fraud detection)
    

### **Use Recall when:**

- False negatives are costly (e.g., cancer detection)
    

### **Use F1 Score when:**

- Data is imbalanced
    
- Need a balance between Precision and Recall
    

### **Use AUC when:**

- Need threshold-independent evaluation
    

---

# 📌 Evaluation Metrics — MCQs (25)

All MCQs contain **question → options → visible answer**.

---

## **MCQ 1**

**Question:** Which metric is most affected by outliers?

-  MAE
    
-  RMSE
    
-  Accuracy
    
-  F1 Score
    

**Answer:** RMSE

---

## **MCQ 2**

**Question:** MSE is defined as:

-  √Σ|errors|
    
-  Average classification error
    
-  Mean squared difference between predicted and actual
    
-  Sum of absolute residuals
    

**Answer:** Mean squared difference between predicted and actual

---

## **MCQ 3**

**Question:** Which metric has the same units as the target variable?

-  MSE
    
-  RMSE
    
-  R²
    
-  MAE
    

**Answer:** RMSE

---

## **MCQ 4**

**Question:** R² < 0 indicates:

-  Perfect fit
    
-  Model worse than predicting mean
    
-  High variance
    
-  Low bias
    

**Answer:** Model worse than predicting mean

---

## **MCQ 5**

**Question:** Precision formula is:

-  TP / (TP + FN)
    
-  TP / (TP + FP)
    
-  TN / (TN + FP)
    
-  TP / (TN + FP)
    

**Answer:** TP / (TP + FP)

---

## **MCQ 6**

**Question:** Recall is also known as:

-  Specificity
    
-  Accuracy
    
-  Sensitivity
    
-  Precision
    

**Answer:** Sensitivity

---

## **MCQ 7**

**Question:** F1 score is high when:

-  Only precision is high
    
-  Only recall is high
    
-  Both precision and recall are high
    
-  Accuracy is high
    

**Answer:** Both precision and recall are high

---

## **MCQ 8**

**Question:** Specificity measures:

-  True positives
    
-  False negatives
    
-  True negatives correctly identified
    
-  Correct predictions
    

**Answer:** True negatives correctly identified

---

## **MCQ 9**

**Question:** Accuracy can be misleading when:

-  Dataset is small
    
-  Dataset is imbalanced
    
-  Confusion matrix is large
    
-  Regression problem exists
    

**Answer:** Dataset is imbalanced

---

## **MCQ 10**

**Question:** FPR (False Positive Rate) is:

-  FP / (FP + TN)
    
-  TN / total
    
-  TP / (TP + FN)
    
-  FN / (TP + FN)
    

**Answer:** FP / (FP + TN)

---

## **MCQ 11**

**Question:** AUC close to 1 indicates:

-  Poor model
    
-  Random model
    
-  Excellent discrimination
    
-  Overfitting
    

**Answer:** Excellent discrimination

---

## **MCQ 12**

**Question:** Which metric does NOT apply to regression?

-  RMSE
    
-  MAE
    
-  R²
    
-  Recall
    

**Answer:** Recall

---

## **MCQ 13**

**Question:** MAE is preferred over MSE when:

-  You want to penalize large errors more
    
-  Outliers are present
    
-  Data is perfectly linear
    
-  Noise is Gaussian
    

**Answer:** Outliers are present

---

## **MCQ 14**

**Question:** Which metric increases even when adding useless predictors?

-  Adjusted R²
    
-  RMSE
    
-  MAE
    
-  R²
    

**Answer:** R²

---

## **MCQ 15**

**Question:** F1 score is a:

-  Weighted average
    
-  Harmonic mean
    
-  Geometric mean
    
-  Arithmetic mean
    

**Answer:** Harmonic mean

---

## **MCQ 16**

**Question:** Which metric is best for imbalanced classification?

-  Accuracy
    
-  Precision/Recall
    
-  MAE
    
-  RMSE
    

**Answer:** Precision/Recall

---

## **MCQ 17**

**Question:** AUC represents:

-  Error rate
    
-  Probability model ranks positive higher than negative
    
-  Difference between precision and recall
    
-  Loss
    

**Answer:** Probability model ranks positive higher than negative

---

## **MCQ 18**

**Question:** False Negative (FN) affects which metric most?

-  Precision
    
-  Recall
    
-  Specificity
    
-  AUC
    

**Answer:** Recall

---

## **MCQ 19**

**Question:** If FP increases, which metric decreases?

-  Recall
    
-  Precision
    
-  RMSE
    
-  R²
    

**Answer:** Precision

---

## **MCQ 20**

**Question:** Which regression metric penalizes large errors most?

-  MAE
    
-  RMSE
    
-  Accuracy
    
-  F1
    

**Answer:** RMSE

---

## **MCQ 21**

**Question:** Specificity is:

-  TN / (TN + FP)
    
-  TP / (TP + FN)
    
-  FP / (TP + FP)
    
-  FN / total
    

**Answer:** TN / (TN + FP)

---

## **MCQ 22**

**Question:** Which metric is threshold-independent?

-  Accuracy
    
-  Precision
    
-  ROC–AUC
    
-  Recall
    

**Answer:** ROC–AUC

---

## **MCQ 23**

**Question:** Which metric is used to evaluate ranking ability?

-  Accuracy
    
-  R²
    
-  AUC
    
-  RMSE
    

**Answer:** AUC

---

## **MCQ 24**

**Question:** Adjusted R² is best used in:

-  Simple regression
    
-  Polynomial regression
    
-  Multiple regression
    
-  Classification
    

**Answer:** Multiple regression

---

## **MCQ 25**

**Question:** A good model has:

-  High bias and high variance
    
-  Low RMSE and high R²
    
-  High MAE and low precision
    
-  Low recall and high accuracy
    

**Answer:** Low RMSE and high R²

---


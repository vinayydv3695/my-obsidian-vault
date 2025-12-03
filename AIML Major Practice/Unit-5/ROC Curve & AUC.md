

## 1. Introduction

The **ROC Curve** (Receiver Operating Characteristic Curve) is a popular tool for evaluating **binary classification models**, especially when dealing with **imbalanced datasets**.

The **AUC** (Area Under the Curve) quantifies the model’s ability to distinguish between classes.

---

# 📌 2. What is the ROC Curve?

ROC curve plots the performance of a classifier by varying the **classification threshold**.

### The two metrics plotted are:

- **True Positive Rate (TPR)**
    

```
TPR = TP / (TP + FN)
```

Also called **Sensitivity** or **Recall**.

- **False Positive Rate (FPR)**
    

```
FPR = FP / (FP + TN)
```

### ROC Curve axes:

- **X-axis:** False Positive Rate (FPR)
    
- **Y-axis:** True Positive Rate (TPR)
    

Each point on the ROC curve corresponds to a specific **threshold**.

---

# 📌 3. Why ROC Curve?

✔ Evaluates classifier performance across all thresholds  
✔ Helps compare multiple classification models  
✔ Good for imbalanced data  
✔ Measures ranking ability, not just accuracy

---

# 📌 4. Ideal ROC Curve Shape

### A perfect classifier:

- TPR = 1
    
- FPR = 0
    
- ROC curve passes through **top-left corner (0,1)**
    

### A random classifier:

- ROC curve is a diagonal line from (0,0) to (1,1)
    

---

# 📌 5. Area Under the Curve (AUC)

AUC is the **area under the ROC curve**.

Interpretation:

|AUC Value|Meaning|
|---|---|
|**1.0**|Perfect classifier|
|**0.9 – 1.0**|Excellent|
|**0.8 – 0.9**|Good|
|**0.7 – 0.8**|Fair|
|**0.5 – 0.7**|Poor|
|**0.5**|No better than random|
|**< 0.5**|Worse than random|

---

# 📌 6. AUC Meaning (Important)

AUC represents the probability that the classifier will rank a **random positive** instance higher than a **random negative** instance.

Example:  
AUC = 0.9 means → The model has a **90% probability** of ranking a positive sample higher than a negative sample.

---

# 📌 7. ROC vs Precision–Recall Curve

|Metric|Best When|
|---|---|
|ROC|balanced or imbalanced datasets|
|PR Curve|heavily imbalanced datasets where positive class is rare|

---

# 📌 8. When Not to Use ROC Curve

✘ When the positive class is extremely rare  
✘ When calibration (actual probabilities) matters more

In such cases, Precision–Recall curve is more meaningful.

---

# 📌 9. Threshold Effect

Changing threshold affects:

- TPR
    
- FPR
    
- Precision
    
- Recall
    

ROC curve shows performance **independent of threshold**.

---

# 📌 10. Summary Table

|Concept|Formula|Meaning|
|---|---|---|
|TPR|TP / (TP + FN)|Recall|
|FPR|FP / (FP + TN)|False alarm rate|
|ROC Curve|TPR vs FPR|Tradeoff curve|
|AUC|Area under ROC|Overall discrimination ability|

---

# 📌 ROC Curve & AUC — MCQs (20)

(All answers are visible and Obsidian-compatible.)

---

## **MCQ 1**

**Question:** ROC curve plots:

-  Precision vs Recall
    
-  TPR vs FPR
    
-  Accuracy vs Recall
    
-  Loss vs Epoch
    

**Answer:** TPR vs FPR

---

## **MCQ 2**

**Question:** TPR is also known as:

-  Specificity
    
-  Precision
    
-  Recall
    
-  F1 score
    

**Answer:** Recall

---

## **MCQ 3**

**Question:** FPR formula is:

-  FP / (TP + FP)
    
-  FP / (FP + TN)
    
-  FN / (TP + FN)
    
-  TN / (TN + FP)
    

**Answer:** FP / (FP + TN)

---

## **MCQ 4**

**Question:** A perfect classifier has ROC curve that passes through:

-  (1,0)
    
-  (0,1)
    
-  (0,0)
    
-  (1,1)
    

**Answer:** (0,1)

---

## **MCQ 5**

**Question:** A random classifier has an AUC of:

-  1.0
    
-  0.8
    
-  0.5
    
-  0
    

**Answer:** 0.5

---

## **MCQ 6**

**Question:** AUC measures:

-  Classification accuracy
    
-  Model training speed
    
-  Probability that model ranks positive higher than negative
    
-  Loss
    

**Answer:** Probability that model ranks positive higher than negative

---

## **MCQ 7**

**Question:** Higher AUC means:

-  Worse classifier
    
-  Random prediction
    
-  Better class separability
    
-  Higher error
    

**Answer:** Better class separability

---

## **MCQ 8**

**Question:** ROC curve is useful when:

-  Dataset is balanced only
    
-  Dataset is imbalanced
    
-  Regression problem
    
-  Clustering problem
    

**Answer:** Dataset is imbalanced

---

## **MCQ 9**

**Question:** ROC curve is threshold:

-  Dependent
    
-  Meaningless
    
-  Independent
    
-  Unpredictable
    

**Answer:** Independent

---

## **MCQ 10**

**Question:** AUC < 0.5 means:

-  Better than random
    
-  Worse than random
    
-  Perfect classifier
    
-  No model exists
    

**Answer:** Worse than random

---

## **MCQ 11**

**Question:** TPR increases when:

-  FP decreases
    
-  FN decreases
    
-  TN increases
    
-  Threshold increases
    

**Answer:** FN decreases

---

## **MCQ 12**

**Question:** FPR increases when:

-  TP increases
    
-  FN decreases
    
-  FP increases
    
-  TN increases
    

**Answer:** FP increases

---

## **MCQ 13**

**Question:** Best AUC value for a classifier is:

-  0.1
    
-  0.5
    
-  0.75
    
-  1.0
    

**Answer:** 1.0

---

## **MCQ 14**

**Question:** ROC curve diagonal line represents:

-  Perfect classification
    
-  Random guessing
    
-  Best threshold
    
-  Underfitting
    

**Answer:** Random guessing

---

## **MCQ 15**

**Question:** PR curve is preferred over ROC when:

-  Balanced classes
    
-  Many positive samples
    
-  Extremely imbalanced dataset
    
-  Continuous target
    

**Answer:** Extremely imbalanced dataset

---

## **MCQ 16**

**Question:** AUC remains unaffected by:

-  Threshold changes
    
-  Threshold selection
    
-  Scaling features
    
-  Class label ordering
    

**Answer:** Threshold changes

---

## **MCQ 17**

**Question:** ROC curve shows tradeoff between:

-  Precision and Recall
    
-  Sensitivity and Specificity
    
-  TPR and FPR
    
-  Accuracy and Recall
    

**Answer:** TPR and FPR

---

## **MCQ 18**

**Question:** A model with TPR = 1 and FPR = 1 is:

-  Perfect
    
-  Useless
    
-  Random
    
-  Ideal
    

**Answer:** Useless

---

## **MCQ 19**

**Question:** ROC curve helps identify:

-  Best learning rate
    
-  Best threshold
    
-  Dataset imbalance
    
-  Feature scaling issues
    

**Answer:** Best threshold

---

## **MCQ 20**

**Question:** AUC close to 0.8 indicates:

-  Excellent model
    
-  Poor model
    
-  No discriminative power
    
-  Fairly good model
    

**Answer:** Fairly good model

---


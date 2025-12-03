
## 1. What is a Confusion Matrix?

A **Confusion Matrix** is a table used to evaluate the performance of a **classification model** by comparing predicted labels with actual labels.

It provides a complete picture of:

- Correct predictions
    
- Incorrect predictions
    
- Types of errors
    

---

# 📌 2. Structure of Confusion Matrix (Binary Classification)

```
               Predicted
              |  Positive  |  Negative
Actual  --------------------------------
Positive      |    TP      |     FN
Negative      |    FP      |     TN
```

Where:

- **TP (True Positive)** → Model predicted Positive, actual is Positive
    
- **TN (True Negative)** → Model predicted Negative, actual is Negative
    
- **FP (False Positive)** → Model predicted Positive, actual is Negative (Type I Error)
    
- **FN (False Negative)** → Model predicted Negative, actual is Positive (Type II Error)
    

---

# 📌 3. Key Metrics Derived from Confusion Matrix

## **1. Accuracy**

```
Accuracy = (TP + TN) / (TP + TN + FP + FN)
```

Measures overall correctness.

---

## **2. Precision**

```
Precision = TP / (TP + FP)
```

Out of predicted positives, how many are correct?  
High precision = low false positives.

---

## **3. Recall (Sensitivity / True Positive Rate)**

```
Recall = TP / (TP + FN)
```

Out of actual positives, how many did we correctly identify?  
High recall = few false negatives.

---

## **4. F1 Score**

```
F1 = 2 * (Precision * Recall) / (Precision + Recall)
```

Harmonic mean of precision and recall.  
Useful when classes are imbalanced.

---

## **5. Specificity (True Negative Rate)**

```
Specificity = TN / (TN + FP)
```

Correctly identifying negatives.

---

## **6. False Positive Rate (FPR)**

```
FPR = FP / (FP + TN)
```

---

## **7. False Negative Rate (FNR)**

```
FNR = FN / (TP + FN)
```

---

# 📌 4. Why Confusion Matrix is Important

- Gives **complete error breakdown**
    
- Helps understand **type of mistakes**
    
- Useful for **imbalanced datasets** where accuracy is misleading
    
- Provides metrics like **Precision, Recall, F1**
    

Accuracy alone can be wrong:  
Example → 95% negatives, model predicts everything as negative → 95% accuracy but useless!

---

# 📌 5. Example Confusion Matrix Interpretation

Example:

```
TP = 80  
FP = 20  
FN = 10  
TN = 90
```

- Accuracy = (80 + 90) / 200 = 85%
    
- Precision = 80 / (80 + 20) = 0.80
    
- Recall = 80 / (80 + 10) = 0.89
    

Shows good recall but slightly lower precision.

---

# 📌 6. Confusion Matrix for Multiclass Classification

For classes A, B, C, a confusion matrix becomes:

```
        Predicted
        A   B   C
Actual A  40  3   2
       B   5  50  1
       C   6   2  60
```

Each row → actual class  
Each column → predicted class

---

# 📌 7. When Confusion Matrix is Useful

✔ Imbalanced data  
✔ Medical diagnosis  
✔ Fraud detection  
✔ Spam detection  
✔ Credit risk modeling

---

# 📌 Confusion Matrix — MCQs (20)

Each includes **question → options → visible answer**.

---

## **MCQ 1**

**Question:** A confusion matrix is used for evaluating:

-  Regression models
    
-  Clustering models
    
-  Classification models
    
-  Dimensionality reduction
    

**Answer:** Classification models

---

## **MCQ 2**

**Question:** True Positive (TP) means:

-  Model predicted negative but actual positive
    
-  Model predicted positive and actual positive
    
-  Both predicted and actual negative
    
-  Prediction was random
    

**Answer:** Model predicted positive and actual positive

---

## **MCQ 3**

**Question:** False Positive (FP) is also known as:

-  Type III error
    
-  Type II error
    
-  Type I error
    
-  Zero error
    

**Answer:** Type I error

---

## **MCQ 4**

**Question:** Which metric is calculated as TP / (TP + FP)?

-  Accuracy
    
-  Recall
    
-  Precision
    
-  F1 score
    

**Answer:** Precision

---

## **MCQ 5**

**Question:** Which metric is TP / (TP + FN)?

-  Specificity
    
-  Precision
    
-  Recall
    
-  F1
    

**Answer:** Recall

---

## **MCQ 6**

**Question:** Accuracy can be misleading when:

-  Data is balanced
    
-  All classes have equal distribution
    
-  Classes are imbalanced
    
-  Model is linear
    

**Answer:** Classes are imbalanced

---

## **MCQ 7**

**Question:** F1 score is the harmonic mean of:

-  Accuracy and Recall
    
-  Precision and Recall
    
-  TN and FP
    
-  TP and FN
    

**Answer:** Precision and Recall

---

## **MCQ 8**

**Question:** Specificity measures:

-  True negatives correctly predicted
    
-  False negatives incorrectly predicted
    
-  Only positive class
    
-  All errors
    

**Answer:** True negatives correctly predicted

---

## **MCQ 9**

**Question:** FN (False Negative) means:

-  Model predicted negative, actual positive
    
-  Model predicted positive, actual negative
    
-  Both predicted and actual positive
    
-  Both predicted and actual negative
    

**Answer:** Model predicted negative, actual positive

---

## **MCQ 10**

**Question:** In spam detection, False Positive means:

-  Spam marked as important
    
-  Important email marked as spam
    
-  Email deleted
    
-  Email unread
    

**Answer:** Important email marked as spam

---

## **MCQ 11**

**Question:** Which metric is useful for imbalanced datasets?

-  Accuracy
    
-  Recall and Precision
    
-  Standard deviation
    
-  Clustering score
    

**Answer:** Recall and Precision

---

## **MCQ 12**

**Question:** What does a confusion matrix NOT show?

-  Correct predictions
    
-  Types of errors
    
-  Overall distribution
    
-  Correlation coefficients
    

**Answer:** Correlation coefficients

---

## **MCQ 13**

**Question:** If FP increases, which metric decreases most?

-  Recall
    
-  Precision
    
-  Accuracy
    
-  F1
    

**Answer:** Precision

---

## **MCQ 14**

**Question:** Which of the following increases when FN decreases?

-  Precision
    
-  Recall
    
-  Accuracy
    
-  Specificity
    

**Answer:** Recall

---

## **MCQ 15**

**Question:** FPR (False Positive Rate) formula is:

-  FP / (FP + TN)
    
-  FP / (TP + FP)
    
-  FN / (TP + FN)
    
-  TN / (TN + FP)
    

**Answer:** FP / (FP + TN)

---

## **MCQ 16**

**Question:** Which metric focuses on the positive class detection ability?

-  Specificity
    
-  Accuracy
    
-  Recall
    
-  FNR
    

**Answer:** Recall

---

## **MCQ 17**

**Question:** Type II error corresponds to:

-  FP
    
-  FN
    
-  TN
    
-  TP
    

**Answer:** FN

---

## **MCQ 18**

**Question:** When both precision and recall are low, the model is:

-  Excellent
    
-  Confused
    
-  Overfitting
    
-  Underperforming
    

**Answer:** Underperforming

---

## **MCQ 19**

**Question:** In a perfect classifier:

-  TP = TN = 0
    
-  FP = FN = 0
    
-  Only FP exists
    
-  Only FN exists
    

**Answer:** FP = FN = 0

---

## **MCQ 20**

**Question:** Confusion matrix is most useful for which type of ML problem?

-  Regression
    
-  Clustering
    
-  Classification
    
-  Dimensionality reduction
    

**Answer:** Classification

---


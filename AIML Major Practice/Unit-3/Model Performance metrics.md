

---

## **1. Classification Accuracy**

- Measures the **ratio of correct predictions** to total samples.
    
- Works well **only when classes are balanced**.
    
- Can be misleading when one class dominates (class imbalance problem).
    

### **Formula**

```
Accuracy = (Number of Correct Predictions) / (Total Samples)
```

---

## **2. Logarithmic Loss (Log Loss)**

- Penalizes **incorrect and overconfident predictions**.
    
- Suitable for **multi-class** classification.
    
- Lower Log Loss → better model.
    

### **Formula**

```
LogLoss = -(1/N) * Σ Σ (y_ij * log(p_ij))
```

Where:

- `y_ij` = 1 if sample _i_ belongs to class _j_, else 0
    
- `p_ij` = predicted probability that sample _i_ belongs to class _j_
    
- Range:
    

```
[0, ∞)
```

---

## **3. Confusion Matrix**

For binary classification:

||Predicted YES|Predicted NO|
|---|---|---|
|Actual YES|TP|FN|
|Actual NO|FP|TN|

### **Accuracy from confusion matrix**

```
Accuracy = (TP + TN) / (TP + TN + FP + FN)
```

---

## **4. Area Under Curve (AUC)**

- Used for **binary classification**.
    
- AUC = probability that classifier ranks a positive sample **higher** than a negative one.
    
- Higher AUC → better performance.
    

### **True Positive Rate (TPR)**

```
TPR = TP / (TP + FN)
```

### **False Positive Rate (FPR)**

```
FPR = FP / (FP + TN)
```

- AUC = Area under **TPR vs FPR curve**.
    
- Range:
    

```
0 to 1
```

---

## **5. F1 Score**

- Harmonic mean of **Precision** and **Recall**.
    
- Good for **imbalanced datasets**.
    
- High F1 = high precision **and** high recall.
    

### **Precision**

```
Precision = TP / (TP + FP)
```

### **Recall**

```
Recall = TP / (TP + FN)
```

### **F1 Score Formula**

```
F1 = 2 * (Precision * Recall) / (Precision + Recall)
```

---

# **📚 MCQs (20 Questions)**

_Easy → Medium → Hard_

---

## **🟢 EASY (1–7)**

### **1. Classification accuracy is best suited when:**

A. Classes are heavily imbalanced  
B. Classes are equally distributed  
C. Only one class exists  
D. None

**Answer: B**

---

### **2. Log Loss is minimized when:**

A. Predictions are wrong but confident  
B. Predictions are close to true probabilities  
C. Classes are balanced  
D. Accuracy is lowest

**Answer: B**

---

### **3. In a confusion matrix, FN means:**

A. Predicted YES but actual NO  
B. Predicted NO but actual YES  
C. Both predicted NO  
D. None

**Answer: B**

---

### **4. AUC is used for:**

A. Regression  
B. Multi-class only  
C. Binary classification  
D. Clustering

**Answer: C**

---

### **5. F1 score is:**

A. Arithmetic mean of precision & recall  
B. Harmonic mean of precision & recall  
C. Geometric mean  
D. None

**Answer: B**

---

### **6. TPR is calculated as:**

A. TP / (TP + FP)  
B. TP / (TP + FN)  
C. TN / (TN + FP)  
D. (TP + TN) / Total

**Answer: B**

---

### **7. High recall but low precision means:**

A. Many false positives  
B. Many false negatives  
C. Both FP and FN high  
D. Model is perfectly balanced

**Answer: A**

---

## **🟡 MEDIUM (8–15)**

### **8. Log Loss is defined for:**

A. 0 or 1 predictions only  
B. Probability predictions  
C. Continuous outputs  
D. Clustering metrics

**Answer: B**

---

### **9. Which metric is most sensitive to class imbalance?**

A. AUC  
B. F1  
C. Accuracy  
D. Recall

**Answer: C**

---

### **10. AUC of 0.5 indicates:**

A. Excellent model  
B. Worse than random  
C. Random classifier  
D. Perfect classifier

**Answer: C**

---

### **11. If FPR increases while TPR stays same, AUC:**

A. Increases  
B. Decreases  
C. Stays same  
D. Becomes 1

**Answer: B**

---

### **12. Precision focuses on reducing:**

A. FN  
B. FP  
C. TN  
D. TPR

**Answer: B**

---

### **13. Recall focuses on reducing:**

A. FP  
B. TN  
C. FN  
D. All errors

**Answer: C**

---

### **14. F1 score becomes low when:**

A. Precision high, recall high  
B. Precision low, recall high  
C. Precision and recall differ widely  
D. Both zero

**Answer: C**

---

### **15. AUC is derived from:**

A. Recall vs Precision  
B. TPR vs FPR  
C. Accuracy vs Error Rate  
D. TP vs TN

**Answer: B**

---

## **🔵 HARD (16–20)**

### **16. A classifier outputs 99% probability for class A, but actual class is B. Log Loss will be:**

A. Very small  
B. Very large  
C. Zero  
D. Equal to 0.5

**Answer: B**

---

### **17. When accuracy is high but F1 score is low, the model likely suffers from:**

A. High variance  
B. Overfitting  
C. Class imbalance  
D. Perfect calibration

**Answer: C**

---

### **18. AUC = 1 means:**

A. Model cannot classify  
B. Model misclassifies every sample  
C. Perfect separation between classes  
D. Random guessing

**Answer: C**

---

### **19. Which metric is _threshold-independent_?**

A. Precision  
B. Recall  
C. AUC  
D. F1 Score

**Answer: C**

---

### **20. If TP = 0, FP = 10, FN = 0, TN = 90, then Precision is:**

A. 0  
B. Undefined  
C. 1  
D. 0.9

**Answer: A**  
(Precision = TP / (TP + FP) = 0 / 10 = 0)

---


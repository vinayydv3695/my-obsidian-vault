


---

## **1. Confusion Matrix Terms**

- **TP** → Actual YES, Predicted YES
    
- **TN** → Actual NO, Predicted NO
    
- **FP** → Actual NO, Predicted YES
    
- **FN** → Actual YES, Predicted NO
    

---

## **2. Evaluation Metrics**

### **Accuracy**

```
Accuracy = (TP + TN) / (TP + TN + FP + FN)
```

### **Error Rate**

```
Error Rate = 1 − Accuracy
```

### **Re-substitution Error**

- Calculated using **training data** instead of test data.
    

### **Sensitivity (Recall / True Positive Rate)**

```
Sensitivity = TP / (TP + FN)
```

### **Specificity (True Negative Rate)**

```
Specificity = TN / (TN + FP)
```

### **Precision**

```
Precision = TP / (TP + FP)
```

### **Recall**

```
Recall = TP / (TP + FN)
```

### **F1 Score**

```
F1 Score = 2 * (Precision * Recall) / (Precision + Recall)
```

---

## **3. Accuracy Estimation Techniques**

### **Holdout Method**

- Train on ~⅔ of data
    
- Test on ~⅓ of data
    

### **Random Subsampling**

- Repeat the holdout process multiple times
    
- Average the accuracies
    

### **K-Fold Cross Validation**

- Split data into **K folds**
    
- Train on K−1 folds, test on remaining fold
    
- Repeat K times; average accuracy
    

### **Leave-One-Out (LOO)**

- Special case of K-fold
    

```
K = number of samples
```

### **Stratified K-Fold**

- Maintains original class distribution in all folds
    
- **Stratified 10-fold CV** is recommended
    

---


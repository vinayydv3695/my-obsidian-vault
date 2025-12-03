

---

## **1. Supervised vs Unsupervised Learning**

### **Supervised Learning**

- Training data includes **class labels**.
    
- Goal: Learn a function to map **input → class**.
    
- Example: Email spam classification.
    

### **Unsupervised Learning**

- No class labels in training data.
    
- Goal: Discover **clusters or structure** in the data.
    
- Example: Customer segmentation.
    

---

## **2. Basic Terminologies**

### **Classifier**

- Algorithm that maps input data to category labels.
    

### **Classification Model**

- Learns from labeled data to predict labels for new samples.
    

### **Feature**

- A measurable property (attribute) of an observation.
    

### **Binary Classification**

- Only two classes (e.g., Male/Female).
    

### **Multi-Class Classification**

- More than two classes; each sample has **one** label.
    

### **Multi-Label Classification**

- A sample can have **multiple labels** simultaneously.
    

---

## **3. Classification vs Prediction**

### **Classification**

- Output: **Categorical label**.
    
- Example: “Approve loan?” → Yes/No.
    

### **Prediction**

- Output: **Continuous value**.
    
- Example: Predicting house price.
    

---

## **4. What Is Classification?**

- Training set consists of tuples: **(x, y)**
    
    - x → attributes
        
    - y → class label
        
- Task: Learn a model mapping x → y.
    

---

## **5. Classification: The Two-Step Process**

### **Step 1: Model Construction**

- Build model using training set.
    
- Models may be: decision trees, rules, formulas, etc.
    

### **Step 2: Model Usage**

- Classify new/unknown data.
    
- Measure **accuracy** using test set.
    

---

## **6. Approaches for Classification**

- Rule-Based Classification
    
- Decision Tree Induction
    
- Bayesian Classification
    
- Artificial Neural Networks
    
- K-Nearest Neighbour (KNN)
    

---

## **7. Rule-Based Classification**

- Model consists of IF-THEN rules.  
    Example:  
    `IF rank = professor OR years > 6 THEN tenured = yes`
    

---

## **8. Decision Tree Induction**

- Produces a **tree** with decision nodes and leaf nodes.
    
- Can overfit if too many branches are created.
    
- Splits based on **categorical/continuous** attributes.
    

---

## **9. Naïve Bayes Classification**

- Based on **Bayes Theorem**.
    
- Assumes **attribute independence**.
    
- Fast and scalable.
    
- Suffers from **zero probability problem** → solved using **Laplace Estimation**.
    

---

## **10. Artificial Neural Networks (ANN)**

- Consists of connected neurons with weights.
    
- Learns by adjusting weights during training.
    
- Can have multiple hidden layers → deep learning.
    

---

## **11. K-Nearest Neighbour (KNN)**

- Lazy learner → no model building; stores all training points.
    
- Classifies based on **k nearest points**.
    
- Distance-weighted KNN gives more weight to closer neighbours.
    

---

## **12. Issues in Classification & Prediction**

### **Data Preparation**

- Data cleaning: handle noise, missing values.
    
- Feature selection: remove irrelevant attributes.
    
- Data transformation: normalization, generalization.
    

### **Evaluation Concerns**

- Predictive accuracy
    
- Speed & scalability
    
- Robustness
    
- Interpretability
    
- Compactness of rules / tree size
    

---

## **13. Confusion Matrix Concepts**

### **TP / TN / FP / FN**

- **TP**: Actual YES, Predicted YES
    
- **TN**: Actual NO, Predicted NO
    
- **FP**: Actual NO, Predicted YES
    
- **FN**: Actual YES, Predicted NO
    

### **Metrics**

- **Accuracy = (TP + TN) / Total**
    
- **Error Rate = 1 − Accuracy**
    
- **Sensitivity (Recall for positive class) = TP / (TP + FN)**
    
- **Specificity = TN / (TN + FP)**
    
- **Precision = TP / (TP + FP)**
    
- **F1 Score = 2 × (Precision × Recall) / (Precision + Recall)**
    

---

## **14. Accuracy Estimation Methods**

### **Holdout Method**

- Split into **training** (⅔) and **test** (⅓).
    

### **Random Subsampling**

- Repeat holdout multiple times → average accuracy.
    

### **K-Fold Cross-Validation**

- Data split into K folds.
    
- Train K times, each time leaving one fold out.
    

### **Leave-One-Out**

- Special case where K = number of samples.
    

### **Stratified K-Fold**

- Preserves class distribution in each fold.
    
- Recommended: **Stratified 10-Fold Cross Validation**.
    

---

# **📚 MCQs (Based on PPT) + Answers**

---

### **1. Supervised learning uses:**

A. Unlabeled data  
B. Labeled data  
C. Clustering  
D. None

**Answer: B**

---

### **2. Multi-label classification means:**

A. Only one label per sample  
B. No label per sample  
C. More than one label per sample  
D. Exactly two labels per sample

**Answer: C**

---

### **3. Classification outputs:**

A. Continuous values  
B. Categorical values  
C. Missing values  
D. Random values

**Answer: B**

---

### **4. Naïve Bayes assumes:**

A. All attributes are dependent  
B. Attributes are conditionally independent  
C. Output is continuous  
D. No probabilities used

**Answer: B**

---

### **5. KNN is:**

A. Eager learner  
B. Lazy learner  
C. Probabilistic learner  
D. None

**Answer: B**

---

### **6. Overfitting commonly occurs in:**

A. KNN  
B. Neural networks only  
C. Decision trees  
D. Naïve Bayes

**Answer: C**

---

### **7. Confusion matrix FP means:**

A. Actual YES, predicted YES  
B. Actual NO, predicted YES  
C. Actual YES, predicted NO  
D. Actual NO, predicted NO

**Answer: B**

---

### **8. Sensitivity measures:**

A. TN rate  
B. TP rate  
C. FP rate  
D. Error rate

**Answer: B**

---

### **9. Best method to preserve class distribution in folds:**

A. Holdout  
B. Random Subsampling  
C. Stratified Cross Validation  
D. Leave-One-Out

**Answer: C**

---

### **10. Accuracy formula is:**

A. TP / Total  
B. (TP + TN) / Total  
C. (FP + FN) / Total  
D. TN / Total

**Answer: B**

---

If you want, I can also generate:

✔ **Chapter-wise MCQs (50–100)**  
✔ **Short answers / long answers**  
✔ **Exam-focused condensed notes**

Just tell me what format you want.
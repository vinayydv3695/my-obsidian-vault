## **Unit 1 – Introduction to AI and Machine Learning**

### **Introduction & History of AI**

- AI focuses on building machines that can think and act intelligently.
    
- Key milestones: Turing Test → Expert Systems → Machine Learning → Deep Learning → Generative AI.
    

### **Overview of Machine Learning & Deep Learning**

- **Machine Learning (ML):** Algorithms learn patterns from data.
    
- **Deep Learning (DL):** Subset of ML using neural networks with multiple layers.
    

### **Applications of AI & ML**

- Healthcare (diagnosis, drug discovery)
    
- Finance (fraud detection, trading)
    
- Robotics
    
- Recommendation systems
    
- Natural language processing
    
- Computer vision
    

### **Differences: AI vs ML vs DL**

- **AI:** Umbrella concept—machines that mimic human intelligence.
    
- **ML:** Approach to achieve AI using data-driven learning.
    
- **DL:** Specialized ML using deep neural networks.
    

### **Types of Data in ML Systems**

- Structured
    
- Unstructured
    
- Semi-structured
    
- Time-series
    
- Image/audio/text data
    

---

## **Unit 2 – Data Preprocessing and Feature Engineering**

### **Data Cleaning & Transformation**

- Removing inconsistencies
    
- Correcting errors
    
- Converting data types
    

### **Standardization, Normalization & Smoothing**

- **Standardization:** Mean = 0, Std = 1
    
- **Normalization:** Scale to [0, 1]
    
- **Smoothing:** Techniques to reduce noise (e.g., moving average)
    

### **Handling Missing Values & Outliers**

- Missing values: deletion, mean/median/mode imputation, model-based imputation
    
- Outliers: clipping, transformation, removal
    

### **Encoding Schemes**

- **Categorical → Numerical**
    
    - One-Hot Encoding
        
    - Label Encoding
        
    - Ordinal Encoding
        
- **Numerical → Categorical**
    
    - Binning / Discretization
        

### **Dimensionality Reduction (PCA)**

- Reduces data dimensions while preserving variance
    
- Converts correlated variables to uncorrelated principal components
    

### **Feature Selection & Extraction**

- Filter, wrapper, and embedded methods
    
- Extraction: PCA, LDA, Autoencoders
    

### **Exploratory Data Analysis (EDA) & Visualization**

- Summary statistics
    
- Histograms, boxplots, scatter plots
    
- Correlation analysis
    

---

## **Unit 3 – Regression Techniques**

### **Types of Regression**

- **Simple Linear Regression**
    
- **Multiple Regression**
    
- **Polynomial Regression**
    
- **Support Vector Regression (SVR)**
    
- **Decision Tree Regression**
    
- **Logistic Regression** (for classification despite its name)
    

### **Evaluation Metrics**

- **MSE (Mean Squared Error)**
    
- **RMSE (Root Mean Squared Error)**
    
- **R² (Coefficient of Determination)**
    

---

## **Unit 4 – Classification Algorithms**

### **Classification Methods**

- **K-Nearest Neighbors (KNN)**
    
- **Support Vector Machines (SVM)**
    
    - Kernel SVM (RBF, Polynomial, Sigmoid kernels)
        
- **Naïve Bayes Classifier**
    
- **Decision Tree Classification**
    
- **Random Forest Classification**
    

---

## **Unit 5 – Analysis of Various Algorithms (Part 1)**

### **Overfitting & Underfitting**

- **Overfitting:** Model learns noise, performs poorly on test data
    
- **Underfitting:** Model too simple, poor performance on both train & test
    

### **Bias–Variance Tradeoff**

- High bias → underfitting
    
- High variance → overfitting
    
- Goal: Balance both
    

### **Bootstrapping & Cross-Validation**

- **Bootstrapping:** Sampling with replacement
    
- **Cross-Validation:** Splitting data into folds to evaluate model consistency
    

---

## **Unit 5 – Analysis of Various Algorithms (Part 2)**

### **Confusion Matrix**

- Shows TP, FP, TN, FN
    
- Basis for many metrics (precision, recall)
    

### **ROC Curve & AUC**

- ROC: Plot of TPR vs FPR
    
- AUC: Area under ROC → higher value = better classifier
    

### **Evaluation Metrics**

- Accuracy
    
- Precision
    
- Recall
    
- F1-Score
    
- Specificity
    
- Sensitivity
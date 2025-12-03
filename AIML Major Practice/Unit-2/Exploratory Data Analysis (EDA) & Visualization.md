
# 📌 **1. What is EDA?**

Exploratory Data Analysis (EDA) is the **process of analyzing datasets** to understand:

- Distribution
    
- Patterns
    
- Relationships
    
- Outliers
    
- Missing values
    
- Anomalies
    

EDA is performed **before** building any ML model.

### Goals of EDA:

✔ Understand data structure  
✔ Detect errors/noise/duplicates  
✔ Reveal hidden patterns  
✔ Form hypotheses  
✔ Guide feature engineering

---

# ============================

# **2. Types of EDA**

# ============================

EDA is broadly divided into three types:

---

## 📌 **A) Univariate Analysis**

Analyzes **one variable** at a time.

### Tools:

- Histogram
    
- Box plot
    
- Bar chart
    
- Pie chart
    
- Frequency tables
    

Used for:

- Detecting skewness
    
- Identifying outliers
    
- Understanding distribution
    

---

## 📌 **B) Bivariate Analysis**

Analyzes relationship between **two variables**.

### Tools:

- Scatter plot
    
- Correlation heatmap
    
- Box plot (categorical vs numeric)
    
- Line plots
    
- Grouped bar charts
    

Used for:

- Detecting correlation
    
- Understanding impact of features on target
    
- Identifying linear/non-linear relations
    

---

## 📌 **C) Multivariate Analysis**

Analyzes **more than two variables**.

### Tools:

- Pairplot
    
- Heatmap
    
- Parallel coordinate plots
    
- 3D scatter plots
    

Useful for:

- Feature selection
    
- Multicollinearity detection
    
- Understanding high-dimensional data
    

---

# ============================

# **3. Key EDA Techniques**

# ============================

---

## 📌 1. Summary Statistics

Measures central tendency and spread:

- Mean, median, mode
    
- Range
    
- Variance, standard deviation
    
- Quartiles
    
- Skewness & kurtosis
    

---

## 📌 2. Correlation Analysis

Correlation matrix identifies relationships between numerical variables.

- Pearson correlation
    
- Spearman correlation
    

High correlation → multicollinearity → affects linear models.

---

## 📌 3. Outlier Detection

Using:

- Box plots
    
- Z-score
    
- IQR method
    

---

## 📌 4. Distribution Analysis

Using:

- Histograms
    
- KDE (Kernel Density Estimation)
    
- Dist plots
    

Shows skewness, modality (uni/bi/multi-modal).

---

## 📌 5. Missing Value Analysis

Check missing patterns:

- Heatmaps
    
- Percentage missing
    
- MCAR/MAR/MNAR insights
    

---

## 📌 6. Feature Relationships

Used to:

- Identify important features
    
- Detect redundant features
    
- Understand target behavior
    

Tools:

- Scatter plots
    
- Grouped boxplots
    
- Violin plots
    

---

# ============================

# **4. Visualization Techniques**

# ============================

### 📌 For Numeric Data:

- Histogram
    
- Boxplot
    
- Violin plot
    
- Line chart
    
- Scatterplot
    

### 📌 For Categorical Data:

- Barplot
    
- Count plot
    
- Pie chart
    
- Stacked bar chart
    

### 📌 For Multivariate Data:

- Heatmap
    
- Pairplot
    
- 3D plots
    
- Parallel coordinates
    

---

# ============================

# **5. EDA Tools & Libraries**

# ============================

### In Python:

- Pandas
    
- NumPy
    
- Matplotlib
    
- Seaborn
    
- Plotly
    
- Sweetviz
    
- Pandas-Profiling
    

### In R:

- ggplot2
    
- dplyr
    
- tidyr
    

---

# ============================

# **6. Why EDA is Essential Before Modeling?**

✔ Identifies noisy or irrelevant features  
✔ Helps choose correct ML algorithms  
✔ Prevents overfitting  
✔ Helps in feature engineering  
✔ Improves data quality  
✔ Reduces dimensionality efforts

---

# ============================

# **MCQs — EDA & Visualization (20)**

# ============================

### **MCQ 1**

EDA is mainly used to:

-  Train models
    
-  Understand data patterns
    
-  Deploy models
    
-  Replace missing values  
    **Answer:** Understand data patterns
    

---

### **MCQ 2**

Which plot shows distribution of a numeric variable?

-  Scatterplot
    
-  Histogram
    
-  Bar chart
    
-  Heatmap  
    **Answer:** Histogram
    

---

### **MCQ 3**

Box plots are mainly used to identify:

-  Missing values
    
-  Outliers
    
-  Correlations
    
-  Categorical encodings  
    **Answer:** Outliers
    

---

### **MCQ 4**

Correlation matrix is used for:

-  Categorical target
    
-  Numeric features
    
-  Missing value filling
    
-  Scaling  
    **Answer:** Numeric features
    

---

### **MCQ 5**

A scatter plot is used for:

-  Two numeric variables
    
-  One numeric variable
    
-  Categorical variable
    
-  Time-series only  
    **Answer:** Two numeric variables
    

---

### **MCQ 6**

Which EDA type deals with one variable?

-  Multivariate
    
-  Bivariate
    
-  Univariate
    
-  Quantitative  
    **Answer:** Univariate
    

---

### **MCQ 7**

Pairplot is used for exploring:

-  One variable
    
-  Two variables
    
-  Multiple variables
    
-  Only categorical variables  
    **Answer:** Multiple variables
    

---

### **MCQ 8**

Heatmaps are used to visualize:

-  Feature importance
    
-  Correlation
    
-  Missing values only
    
-  PCA components  
    **Answer:** Correlation
    

---

### **MCQ 9**

Violin plots show:

-  Distribution + density
    
-  Only median
    
-  Only outliers
    
-  Only standard deviation  
    **Answer:** Distribution + density
    

---

### **MCQ 10**

Which chart is best for categorical data?

-  Histogram
    
-  Bar chart
    
-  Violin plot
    
-  Scatterplot  
    **Answer:** Bar chart
    

---

### **MCQ 11**

Missing value heatmaps are generated using:

-  Matplotlib
    
-  Seaborn
    
-  Pandas
    
-  All of these  
    **Answer:** All of these
    

---

### **MCQ 12**

Skewness represents:

-  Correlation
    
-  Symmetry of distribution
    
-  Mean shift
    
-  Standard deviation  
    **Answer:** Symmetry of distribution
    

---

### **MCQ 13**

KDE stands for:

-  Kernel Data Extraction
    
-  Kernel Density Estimation
    
-  Key Data Encoder
    
-  Knowledge Data Engine  
    **Answer:** Kernel Density Estimation
    

---

### **MCQ 14**

Which of the following detects multicollinearity?

-  Scatterplot
    
-  Boxplot
    
-  Correlation matrix
    
-  Histogram  
    **Answer:** Correlation matrix
    

---

### **MCQ 15**

Scree plots are used in:

-  PCA
    
-  EDA only
    
-  Regression
    
-  Classification  
    **Answer:** PCA
    

---

### **MCQ 16**

Large number of outliers in EDA indicates:

-  Data quality issues
    
-  Perfect dataset
    
-  Balanced dataset
    
-  No preprocessing needed  
    **Answer:** Data quality issues
    

---

### **MCQ 17**

A line plot is ideal for:

-  Time-series data
    
-  Categorical data
    
-  Random data
    
-  Binary classification  
    **Answer:** Time-series data
    

---

### **MCQ 18**

A pairplot shows:

-  Only correlations
    
-  Pairwise relationships
    
-  Only missing values
    
-  PCA projections  
    **Answer:** Pairwise relationships
    

---

### **MCQ 19**

A pie chart is used for:

-  Distribution of numeric features
    
-  Proportion of categories
    
-  Detecting outliers
    
-  Time-series  
    **Answer:** Proportion of categories
    

---

### **MCQ 20**

The first step in EDA is usually:

-  Plotting histograms
    
-  Understanding the dataset structure
    
-  Running PCA
    
-  Training ML models  
    **Answer:** Understanding the dataset structure
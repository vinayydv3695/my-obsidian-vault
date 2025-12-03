

## 1. Introduction

- Naive Bayes is a **probabilistic classifier** based on **Bayes’ Theorem**.
    
- It assumes **feature independence** (“naive” assumption).
    
- Works extremely well for **text classification**, especially **spam detection**, **sentiment analysis**, etc.
    

---

## 2. Bayes’ Theorem

Bayes’ rule:

```
P(Y|X) = [P(X|Y) * P(Y)] / P(X)
```

Where:

- P(Y|X): Posterior probability
    
- P(Y): Prior probability
    
- P(X|Y): Likelihood
    
- P(X): Evidence (normalizing term)
    

---

## 3. Naive Independence Assumption

For features x₁, x₂, …, xₙ:

```
P(X|Y) = P(x₁|Y) * P(x₂|Y) * ... * P(xₙ|Y)
```

This simplifies computation massively.

---

## 4. Types of Naive Bayes Classifiers

### **1. Gaussian Naive Bayes**

Used when features are **continuous** and follow normal distribution.

```
P(x|y) = (1 / √(2πσ²)) * exp( -(x − μ)² / (2σ²) )
```

---

### **2. Multinomial Naive Bayes**

Used for **text data**, where features represent **word counts** or **frequencies**.

---

### **3. Bernoulli Naive Bayes**

Used when features are **binary** (word present/absent).

---

## 5. Zero-Frequency Problem

If a word never appears in a class, probability becomes zero.

**Solution: Laplace Smoothing:**

```
P(word|class) = (count + 1) / (N + V)
```

Where:

- N = total word count in the class
    
- V = vocabulary size
    

---

## 6. Advantages

- Fast training + prediction
    
- Handles high-dimensional data
    
- Works well with text
    
- Robust to irrelevant features
    
- Requires little training data
    

---

## 7. Limitations

- Assumes **independence**, which is rarely true
    
- Poor performance when features are correlated
    
- Zero-frequency issue without smoothing
    

---

## 8. Applications

- Spam filtering
    
- Sentiment analysis
    
- Document classification
    
- Recommendation systems
    

---

# 📌 Naive Bayes — MCQs (20) 

Each question → options → visible answer.

---

## **MCQ 1**

**Question:** Naive Bayes is based on which theorem?

-  Pythagoras
    
-  Bayes' Rule
    
-  Central Limit Theorem
    
-  Markov Chain
    

**Answer:** Bayes' Rule

---

## **MCQ 2**

**Question:** The term “Naive” refers to which assumption?

-  Class labels are dependent
    
-  Features are dependent
    
-  Only continuous features exist
    
-  Features are independent
    

**Answer:** Features are independent

---

## **MCQ 3**

**Question:** Naive Bayes is mainly used for:

-  Clustering
    
-  Regression
    
-  Reinforcement learning
    
-  Classification
    

**Answer:** Classification

---

## **MCQ 4**

**Question:** Which Naive Bayes type is used for continuous data?

-  Bernoulli NB
    
-  Multinomial NB
    
-  Polynomial NB
    
-  Gaussian NB
    

**Answer:** Gaussian NB

---

## **MCQ 5**

**Question:** Multinomial Naive Bayes works best for:

-  Images
    
-  Binary features
    
-  Word counts
    
-  Regression tasks
    

**Answer:** Word counts

---

## **MCQ 6**

**Question:** Bernoulli Naive Bayes is used when features are:

-  Continuous
    
-  Binary
    
-  Multi-class
    
-  Gaussian
    

**Answer:** Binary

---

## **MCQ 7**

**Question:** What problem does Laplace smoothing solve?

-  High variance
    
-  Low bias
    
-  Zero probability issue
    
-  Overfitting
    

**Answer:** Zero probability issue

---

## **MCQ 8**

**Question:** Which probability is P(Y) in Naive Bayes?

-  Likelihood
    
-  Evidence
    
-  Posterior
    
-  Prior
    

**Answer:** Prior

---

## **MCQ 9**

**Question:** Which probability is P(Y|X)?

-  Likelihood
    
-  Posterior
    
-  Marginal
    
-  Prior
    

**Answer:** Posterior

---

## **MCQ 10**

**Question:** Naive Bayes works best when features are:

-  Highly correlated
    
-  All categorical
    
-  Independent
    
-  Missing
    

**Answer:** Independent

---

## **MCQ 11**

**Question:** Naive Bayes handles which type of data very well?

-  Spatial data
    
-  Audio signals
    
-  Text data
    
-  Image pixel data
    

**Answer:** Text data

---

## **MCQ 12**

**Question:** Which Naive Bayes model is commonly used for spam filtering?

-  Gaussian
    
-  HMM
    
-  Deep learning
    
-  Multinomial / Bernoulli
    

**Answer:** Multinomial / Bernoulli

---

## **MCQ 13**

**Question:** What is the computational complexity of predicting using Naive Bayes?

-  Very high
    
-  O(n³)
    
-  O(log n)
    
-  Very fast
    

**Answer:** Very fast

---

## **MCQ 14**

**Question:** Naive Bayes requires:

-  Large training data
    
-  Weight initialization
    
-  Backpropagation
    
-  Very little training data
    

**Answer:** Very little training data

---

## **MCQ 15**

**Question:** Which statement is TRUE for Naive Bayes?

-  Needs gradient descent
    
-  Is a parametric algorithm
    
-  Requires feature scaling
    
-  Assumes conditional independence
    

**Answer:** Assumes conditional independence

---

## **MCQ 16**

**Question:** Gaussian Naive Bayes assumes features follow:

-  Uniform distribution
    
-  Poisson distribution
    
-  Normal distribution
    
-  Exponential distribution
    

**Answer:** Normal distribution

---

## **MCQ 17**

**Question:** P(X) in Bayes' theorem is called:

-  Likelihood
    
-  Prior
    
-  Evidence
    
-  Posterior
    

**Answer:** Evidence

---

## **MCQ 18**

**Question:** Naive Bayes struggles when:

-  Data is high-dimensional
    
-  Features are strongly correlated
    
-  Dataset is small
    
-  Vocabulary size is large
    

**Answer:** Features are strongly correlated

---

## **MCQ 19**

**Question:** Naive Bayes is:

-  Slow to train
    
-  A lazy learner
    
-  A parametric model
    
-  Memory inefficient
    

**Answer:** A parametric model

---

## **MCQ 20**

**Question:** In text classification, Naive Bayes typically represents documents as:

-  Images
    
-  Bag-of-words
    
-  Matrices of pixels
    
-  Audio waveforms
    

**Answer:** Bag-of-words

---


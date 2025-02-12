# Business_Analytics_Bootcamp_4


# Matching


## Overview  
This repository contains materials and analysis related to **Matching** as part of the Business Analytics Bootcamp. **Matching** is a statistical technique used for causal inference when a naturally comparable control group is not available. It helps estimate treatment effects by reducing selection bias in observational studies.

## Topics Covered  
### 📌 Matching Game Plan  
- When a naturally similar control group is missing, we can **create one** by selecting individuals/entities with similar characteristics.  
- This method allows for **causal inference** by reducing bias in observational studies.  

### 📌 What is Matching?  
- A statistical technique used to estimate causal effects by **pairing treated and control units** based on observed covariates.  

### 📌 Unconfoundedness  
- Assumes that **treatment assignment is independent** of potential outcomes given observed covariates.  

### 📌 The Curse of Dimensionality  
- As the number of covariates increases, it becomes **harder to find exact matches**, making matching less effective in high-dimensional data.  

### 📌 Common Support Region  
- The region where **treatment and control groups have overlapping covariates** to ensure a fair comparison.  

### 📌 Matching Robustness  
- Checking the **sensitivity of results** by varying matching criteria and removing certain confounders.  

---

## 📊 Findings & Insights  

### **Data Summary & Challenges**  
The dataset consists of student demographic information, parental background, socioeconomic status, and standardized test scores. A key challenge was the significant differences in characteristics between students in Catholic and public schools, making a direct comparison **inappropriate** without adjustments.

### **Initial Analysis Before Matching**  
- There were statistically significant differences in parental education, income, and age between Catholic and public school students.  
- Students in Catholic schools tended to come from families with **higher income and parental education levels**.  
- These pre-existing differences suggested that **any observed effect on test scores could be due to these factors rather than the type of school**.  

### **Matching Results & Treatment Effect Estimates**  
- After applying matching techniques, we found **no significant advantage** in standardized test scores for students attending Catholic schools.  
- The results suggested that once we account for background characteristics, the differences in performance between Catholic and public school students become **statistically insignificant**.  
- This means that **students’ performance is likely influenced more by family background and socioeconomic factors rather than the type of school itself**.  

### **Robustness Check**  
- A robustness check confirmed that the results remained consistent even when slight variations in the matching criteria were applied.  
- The treatment effect estimates remained **negative or close to zero**, further reinforcing the conclusion that Catholic schooling does not provide a measurable academic advantage.  

---

## 🚀 Key Takeaways  
- **Matching is crucial for causal inference**, especially when dealing with observational data.  
- **Before matching, students in Catholic schools appeared to perform better**, but this was largely due to socioeconomic advantages rather than school quality.  
- **After matching, the apparent advantage disappeared**, indicating that Catholic schooling does not significantly improve standardized test scores.  
- **Robustness checks supported the findings**, making the conclusion more reliable.  

---

## 📂 Repository Structure  
- **`/school.csv/`** → Contains dataset files.  
- **`/Matching.ipynb/`** → Contains Jupyter Notebooks with analysis.  
- **`README.md`** → This file.  

---

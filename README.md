# 🎯 Phishing Website Detection Using Machine Learning

**Cyber Security – Assignment 2 (CBIT 2025-26)**  
Based on *H V Kishan Kumar, Praveen K S, IJRASET54850 2023-07-19*

---

## 📌 Project Overview

Phishing websites imitate legitimate websites to steal sensitive information such as usernames, passwords, and banking details. Detecting phishing websites is crucial for cybersecurity.  

In this assignment, I implemented **machine learning models** to automatically detect phishing websites. The workflow involved **data collection, preprocessing, model training, feature selection, evaluation, and visualization**. The proposed method uses **Recursive Feature Elimination (RFE) with Random Forest** to improve prediction accuracy.

---

## 🗂 Dataset

- **Dataset Name:** UCI Phishing Websites Dataset  
- **File Name:** `phishing.csv`  
- **Instances:** 11,055  
- **Features:** 30+ website attributes (e.g., URL length, presence of IP, domain registration length)  
- **Target Column:** `Result` (0 = Legitimate, 1 = Phishing)  
- **Source:** [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/Phishing+Websites)

---

## ⚙️ Tech Stack

- **Programming Language:** Python 3  
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn  
- **IDE / Platform:** Jupyter Notebook, VS Code, Google Colab  

---

## 🗂 Project Structure
Phishing-Detection-CS/
│
├─ code/
│ └─ phishing_detection.ipynb # Main notebook with ML workflow
├─ data/
│ └─ phishing.csv # Dataset
├─ images/ # Generated plots
├─ README.md # Project description
└─ requirements.txt # Python dependencies

---

## 🚀 Workflow / What I Did

1. **Data Loading & Exploration**  
   - Loaded the dataset from `data/phishing.csv`  
   - Explored features and checked for missing values  

2. **Feature & Target Separation**  
   - Features (`X`) = all columns except `Result`  
   - Target (`y`) = `Result` column  

3. **Train-Test Split**  
   - Split dataset into 80% training and 20% testing data  

4. **Model Training**  
   - **Decision Tree:** trained on all features  
   - **Random Forest:** trained as baseline model  
   - **RFE + Random Forest:** selected **top 15 features** using Recursive Feature Elimination and trained Random Forest on reduced feature set  

5. **Model Evaluation**  
   - Calculated **accuracy** for all models  
   - Generated **confusion matrix** and **classification report**  
   - Compared results to select the best model  

6. **Visualization**  
   - Plotted **Accuracy Comparison** between all models  
   - Plotted **Confusion Matrix** for RFE + RF 

7. **Results**  
   - Decision Tree Accuracy: 94.5%  
   - Random Forest Accuracy: 96.0%  
   - **RFE + Random Forest Accuracy: 97.2%** → Best performing model  

---

## 📊 Results Summary

| Model                   | Accuracy   |
|-------------------------|-----------|
| Decision Tree           | 94.5 %    |
| Random Forest           | 96.0 %    |
| **RFE + RF (Proposed)** | **97.2 %** |


---

## 🔗 GitHub Repository

[https://github.com/AnushaBanavath/Phishing_Detection_CS](https://github.com/AnushaBanavath/Phishing_Detection_CS)



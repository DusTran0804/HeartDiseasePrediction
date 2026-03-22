# 🫀 Heart Disease Clustering & Classification

## 📌 Overview
This project analyzes a large-scale heart disease dataset (270,000 records) using both **unsupervised learning (clustering)** and **supervised learning (classification)** techniques.  
The objective is to uncover hidden patterns and identify key factors that distinguish different patient risk groups.

---

## 📊 Dataset
The dataset consists of **14 medical features**, including:

- **Demographics**: Age, Sex  
- **Clinical measurements**: Blood Pressure (BP), Cholesterol, Max Heart Rate  
- **Diagnostic indicators**: Chest Pain Type, EKG Results, ST Depression, Thallium  
- **Other features**: Exercise Angina, Number of vessels (fluoroscopy)

✔ No missing values  
✔ Fully numerical after encoding  

---

## ⚙️ Data Processing
- One-hot encoding for categorical variables  
- Feature scaling using `StandardScaler`  
- Dimensionality reduction using **PCA (2 components)**  

---

## 🔍 Clustering (Unsupervised Learning)
- PCA used for visualization  
- Data split into **2 clusters**

### 🔑 Insights
**Cluster 1 (Higher Risk Group):**
- Higher age  
- Higher cholesterol  
- Higher ST depression  
- More vessels affected  
- More exercise-induced angina  

**Cluster 0 (Lower Risk Group):**
- Lower ST depression  
- Higher max heart rate  
- Fewer abnormal indicators  

---

## 📈 Visualization
- PCA scatter plot shows cluster separation  
- Boxplots & histograms for:
  - Age  
  - Cholesterol  
  - Max Heart Rate  
  - ST Depression  

---

## 🤖 Classification (Random Forest)
- Model: `RandomForestClassifier`  
- Task: Predict cluster labels  

### 📊 Performance
**Accuracy: ~98.9%**

→ Indicates strong separability between clusters  

---

## 🔑 Feature Importance
Top important features:
1. Chest pain type (Type 4)  
2. Thallium (Level 7)  
3. ST depression  
4. Exercise angina  
5. Slope of ST  
6. Max heart rate  
7. Number of vessels  

---

## 🧠 Key Takeaways
- Data naturally forms **2 distinct patient groups**  
- Important medical indicators strongly influence clustering  
- Machine learning effectively identifies high-risk patients  

---

## 🚀 Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  

---

## 📌 Future Work
- Try advanced clustering (DBSCAN, Hierarchical)  
- Validate with real labels (if available)  
- Deploy as a healthcare prediction system  





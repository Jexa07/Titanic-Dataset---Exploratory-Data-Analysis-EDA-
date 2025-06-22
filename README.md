<!-- Project Banner -->
<p align="center">
  <img src="https://i.postimg.cc/9QZZpwSJ/Untitled-design-5.png" width="80%" alt="Titanic EDA Banner" />
</p>

<h1 align="center">🚢 Titanic Dataset - Exploratory Data Analysis (EDA)</h1>

<p align="center"><i>A data-driven voyage into survival insights from one of the most iconic datasets in ML history.</i></p>

---

## 📁 Dataset Overview

- **Rows:** 891
- **Columns:** 12 (`Survived`, `Pclass`, `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Ticket`, `Fare`, `Cabin`, `Embarked`)

---

## 📌 Key Objectives

- 🧼 Handle missing values effectively  
- 📊 Understand distributions of numerical & categorical features  
- 🚩 Identify outliers  
- 🔍 Explore relationships between survival and other variables  

---

## 🔍 EDA Breakdown

### 1️⃣ Data Loading and Inspection
- Verified shape, columns, and data types
- Major missing values in **Age** and **Cabin**

### 2️⃣ Missing Values Visualization
- Used `missingno` for heatmap visuals  
- `Cabin`: ~77% missing → dropped or binned  
- `Age`: ~20% missing → imputation suggested  

### 3️⃣ Univariate Analysis

**Numerical Features**
- `Fare`: Right-skewed with multiple outliers
- `Age`: Bimodal; concentration under 40

**Categorical Features**
- `Sex`: Males (577) > Females (314)
- `Embarked`: Most from **Southampton (S)**

### 4️⃣ Outlier Detection
- Boxplots show high `Fare` outliers (mostly 1st class)
- `Age` has outliers at extremes (infants + elderly)

### 5️⃣ Correlation Matrix
- 📈 Positive: `Fare` ↔ `Survived`
- 📉 Negative: `Pclass` ↔ `Survived`

### 6️⃣ Bivariate Visualizations
- `Sex` ↔ `Survived`: Females had higher survival rate
- `Pclass` ↔ `Survived`: 1st class survived most
- `Age` ↔ `Survived`: Younger passengers had better chances
- `Fare` ↔ `Pclass`: Median fare increases with class

---

## 📊 Key Findings

| Feature    | Insight                                      |
|------------|----------------------------------------------|
| **Sex**    | Females had a much higher survival rate      |
| **Pclass** | Higher class → Higher survival               |
| **Age**    | Younger passengers more likely to survive    |
| **Fare**   | Higher fare correlates with better survival  |
| **Embarked** | Port ‘C’ passengers survived more than ‘S’ |

---

## 🧠 Suggestions for Modeling

- Encode categorical vars: `Sex`, `Embarked`, `Pclass`  
- Impute `Age` using median or regression  
- Drop/bin `Cabin` feature  
- Normalize/scale `Fare`  

---

## 🛠 Technologies Used

![Python](https://img.shields.io/badge/-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=for-the-badge&logo=pandas)
![Seaborn](https://img.shields.io/badge/-Seaborn-004B87?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557C?style=for-the-badge)
![Google Colab](https://img.shields.io/badge/-Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

---

## ▶️ How to Run

1. Open the `.ipynb` notebook in Google Colab  
2. Upload the Titanic dataset CSV  
3. Run each cell to explore insights

---

## 📬 Contact

Made with 💜 by **Arpita Pani**  
📧 [arpita.pani2018@gmail.com](mailto:arpita.pani2018@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/arpitapani07/)

---

## 📜 License

This project is released under the **MIT License**.

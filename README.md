# Titanic Dataset - Exploratory Data Analysis (EDA)

## 📁 Dataset Overview

- Source: Titanic dataset (Kaggle)
- Rows: 891
- Columns: 12 (Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked)


## 📌 Key Objectives

- Handle missing values effectively
- Understand distributions of numerical and categorical features
- Identify outliers
- Explore relationships between survival and other features


## 🔍 Exploratory Data Analysis Steps

### 1. Data Loading and Inspection
- Verified shape, columns, and data types.
- Found major missing values in Age and Cabin.

### 2. Missing Values Visualization
- Used missingno to visually analyze missing data patterns.
- Cabin: ~77% missing → dropped or categorized
- Age: ~20% missing → imputation suggested

### 3. Univariate Analysis
#### Numerical Features
- Fare: Highly right-skewed with outliers
- Age: Bimodal distribution, concentrated under 40

#### Categorical Features
- Sex: More males (577) than females (314)
- Embarked: Most passengers from Southampton (644)

### 4. Outlier Detection
- Boxplots show high fare outliers (mostly 1st class)
- Age has outliers at both extremes (infants and seniors)

### 5. Correlation Matrix
- Positive correlation: Fare ↔ Survived
- Negative correlation: Pclass ↔ Survived

### 6. Bivariate Visualizations
- *Survival vs Sex*: Higher survival rate among females  
- *Survival vs Pclass*: 1st class had the highest survival  
- *Age vs Survival*: Younger people had better chances  
- *Fare vs Pclass*: Median fare rises with class


## 📊 Key Findings

| Feature     | Insight |
|-------------|--------|
| Sex     | Females had much higher survival rate |
| Pclass  | Higher class = Higher survival rate |
| Age     | Younger passengers more likely to survive |
| Fare    | Higher fare correlates with better survival |
| Embarked| Port 'C' passengers had higher survival than 'S' |


## 🧠 Suggestions for Modeling

- Encode categorical variables: Sex, Embarked, Pclass
- Impute Age using median or regression
- Drop or bin Cabin feature
- Normalize/standardize Fare for ML models


## 🛠 Technologies Used

- Python (pandas, seaborn, matplotlib, missingno)
- Google Colab
- Word + Markdown for reporting


## 📌 How to Run

1. Open the provided .ipynb file in Google Colab
2. Upload the Titanic dataset CSV
3. Run each cell for visualizations and insights


## 📬 Contact

For improvements or collaboration:
Arpita Pani | Data Science Enthusiast  
📧 [arpita.pani2018@gmail.com]   
🔗 [LinkedIn](https://www.linkedin.com/in/arpitapani07/)


## 📜 License

This project is released under the MIT License.

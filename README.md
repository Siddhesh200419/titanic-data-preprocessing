# 🧼 Task 1: Data Cleaning & Preprocessing - Titanic Dataset

This repository contains my submission for **Task 1** of the **AI & ML Internship**: focused on **data cleaning and preprocessing** using the Titanic dataset.

---

## 📌 Objective

To clean and prepare raw Titanic dataset for Machine Learning models. This includes:
- Handling missing data
- Encoding categorical features
- Scaling numerical values
- Outlier detection and removal

---

## 🛠️ Tools & Technologies Used

- Python 🐍
- Pandas & NumPy 📊
- Matplotlib & Seaborn 📈
- Scikit-learn 🔧

---

## 📁 Dataset

- [Titanic Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- File used: `titanic.csv`

---

## 🔍 Steps Performed

### 1. **Imported and Explored Data**
- Checked data types, null values, and structure of the dataset.

### 2. **Handled Missing Values**
- Filled `Age` with **median**.
- Filled `Embarked` with **mode**.
- Dropped `Cabin` due to excessive missing values.

### 3. **Categorical Encoding**
- Encoded `Sex` using binary mapping (male=0, female=1).
- Applied **One-Hot Encoding** to `Embarked`.

### 4. **Feature Scaling**
- Standardized `Age` and `Fare` using `StandardScaler`.

### 5. **Outlier Detection and Removal**
- Plotted boxplots for `Age` and `Fare`.
- Removed outliers from `Fare` using the **IQR method**.

### 📊 Outlier Boxplot

![Boxplot for Age and Fare]
![image](https://github.com/user-attachments/assets/c30f6d78-c659-4fa8-9385-63d8a5419f2b)


---

## 🧠 Key Learnings

- Real-world datasets are messy — preprocessing is a critical step before model training.
- Learned various techniques like median/mode imputation, encoding, and standardization.
- Visualized and cleaned outliers for better model input.

---

## ❓ Sample Interview Questions Answered

1. **Types of missing data:** MCAR, MAR, MNAR  
2. **Handling categorical variables:** Label and One-Hot Encoding  
3. **Normalization vs Standardization:** 
   - Normalization → scales to [0, 1]  
   - Standardization → zero mean, unit variance  
4. **Outlier detection:** Boxplot, IQR  
5. **Importance of preprocessing:** Ensures model quality, avoids bias  
6. **Data imbalance handling:** SMOTE, Resampling, Class weights  
7. **Encoding methods:** One-Hot (independent binary columns), Label (ordinal values)  
8. **Effect on model accuracy:** Strong impact — better preprocessing leads to better models

---

## ✅ Final Output Snapshot
<img width="566" alt="image" src="https://github.com/user-attachments/assets/d171f6fc-de48-4880-9212-fa08628bff81" />


Here’s a sample of the cleaned dataset:

Data Preprocessing Completed 
   PassengerId  Survived  Pclass  \
0            1         0       3   
2            3         1       3   
3            4         1       1   
4            5         0       3   
5            6         0       3   

                                           Name  Sex       Age  SibSp  Parch  \
0                       Braund, Mr. Owen Harris    0 -0.565736      1      0   
2                        Heikkinen, Miss. Laina    1 -0.258337      0      0   
3  Futrelle, Mrs. Jacques Heath (Lily May Peel)    1  0.433312      1      0   
4                      Allen, Mr. William Henry    0  0.433312      0      0   
5                              Moran, Mr. James    0 -0.104637      0      0   

             Ticket      Fare  Embarked_Q  Embarked_S  
0         A/5 21171 -0.502445       False        True  
2  STON/O2. 3101282 -0.488854       False        True  
3            113803  0.420730       False        True  
4            373450 -0.486337       False        True  
5            330877 -0.478116        True       False


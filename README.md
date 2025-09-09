# 🛳 Titanic Survival Prediction

## 📌 Project Overview  
This project analyzes the famous **Titanic dataset** to explore passenger demographics, travel classes, and survival rates.  
We perform **Exploratory Data Analysis (EDA)** to uncover patterns in the data, followed by building a **Logistic Regression model** to predict survival outcomes.  

---

## 📂 Dataset  
The dataset used is from the **[Kaggle Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)** competition.  

**Columns include:**  
- `PassengerId` : Unique ID for each passenger  
- `Survived` : Target variable (0 = Not Survived, 1 = Survived)  
- `Pclass` : Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)  
- `Name` : Passenger name  
- `Sex` : Gender  
- `Age` : Passenger age  
- `SibSp` : Number of siblings/spouses aboard  
- `Parch` : Number of parents/children aboard  
- `Ticket` : Ticket number  
- `Fare` : Passenger fare  
- `Cabin` : Cabin (many missing values)  
- `Embarked` : Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)  

---

## 🔎 Exploratory Data Analysis (EDA)  
### 1. Handling Missing Data  
- Imputed missing `Age` values based on `Pclass`  
- Filled missing `Embarked` with the most common port (`S`)  
- Dropped `Cabin` due to too many missing values  

### 2. Univariate Analysis  
- Distribution of Age & Fare  
- Count plots of Survived vs Not Survived  
- Passenger Class distribution  

### 3. Bivariate Analysis  
- Survival by **gender**  
- Survival by **class**  
- Heatmap of correlations  

📊 **Example Visualization:**  
![Survival Count Example](images/survival_count.png)  
*(Add your plots in an `images/` folder and link them here)*  

---

## 🤖 Modeling: Logistic Regression  
**Steps followed:**  
1. Converted categorical variables (`Sex`, `Embarked`) to numeric using dummy encoding.  
2. Split data into **train (70%) / test (30%)**.  
3. Trained a **Logistic Regression model**.  
4. Evaluated with accuracy score and confusion matrix.  

---

## 📊 Results  
- Logistic Regression accuracy: **~78–82%** (depending on preprocessing).  
- Key findings:  
  - Females had a much higher survival rate.  
  - Higher-class passengers survived more often.  
  - Age and family size also influenced survival chances.  

📊 **Confusion Matrix Example:**  
![Confusion Matrix](images/confusion_matrix.png)  

---

## 🚀 Tools & Libraries  
- **Python 3.x**  
- **Pandas, NumPy** (data wrangling)  
- **Matplotlib, Seaborn** (visualization)  
- **Scikit-learn** (ML model & evaluation)  

---

## 📌 Future Improvements  
- Test advanced models: **Random Forest, XGBoost, SVM**.  
- Feature engineering: extract titles from names, family size, etc.  
- Hyperparameter tuning with GridSearchCV.  

---

## 🏆 Acknowledgements  
- Kaggle for the dataset  
- Scikit-learn for ML tools  
- Seaborn/Matplotlib for visualization  

---

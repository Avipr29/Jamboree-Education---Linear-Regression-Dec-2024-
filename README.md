# 🎓 Jamboree Education: Linear Regression for Graduate Admissions  

## 📌 Context  
**Jamboree Education** has helped thousands of students achieve top scores in exams like **GMAT, GRE, and SAT**. Recently, they introduced a **graduate admission probability predictor**, designed specifically for Indian students aiming for **Ivy League colleges**.  

This project explores **factors influencing graduate admissions** and builds a **Linear Regression model** to predict admission chances based on various parameters.  

---

## 📊 Dataset  

📂 **Dataset:** `jamboree_admission.csv`  

### 🔢 Column Profiling:  
- **Serial No.** - Unique row identifier (to be dropped)  
- **GRE Scores** - Standardized test scores (out of 340)  
- **TOEFL Scores** - English proficiency scores (out of 120)  
- **University Rating** - Rating of the university (1 to 5)  
- **SOP & LOR Strength** - Statement of Purpose and Letter of Recommendation (rated 1 to 5)  
- **Undergraduate GPA** - CGPA (out of 10)  
- **Research Experience** - Binary (0 = No, 1 = Yes)  
- **Chance of Admit** - Admission probability (0 to 1)  

---

## 🛠️ Concepts Used  
✅ **Exploratory Data Analysis (EDA)**  
✅ **Linear Regression (Statsmodels & Scikit-learn)**  
✅ **Multicollinearity Check (VIF Score)**  
✅ **Regression Assumptions Validation**  
✅ **Model Evaluation (MAE, RMSE, R², Adjusted R²)**  
✅ **Lasso & Ridge Regression**  

---

## 📈 Methodology  

### 1️⃣ Exploratory Data Analysis (EDA)  
✔ **Data Structure Analysis:** Checked missing values, duplicates, and outliers.  
✔ **Univariate Analysis:** Distribution plots for **GRE, TOEFL, CGPA, SOP, LOR, and Admission Probability**.  
✔ **Bivariate Analysis:** Correlation heatmap & scatterplots to explore relationships.  
✔ **Dropped Unique Row Identifier** (Serial No.).  

### 2️⃣ Data Preprocessing  
✔ **Checked for missing values and handled them appropriately.**  
✔ **Outlier treatment using IQR & Z-score analysis.**  
✔ **Feature Engineering:** Normalized/standardized variables where necessary.  

### 3️⃣ Model Building  
✔ **Built a Linear Regression Model (Statsmodels)**  
✔ **Evaluated Model Coefficients**  
✔ **Tried Lasso & Ridge Regression to improve performance**  

### 4️⃣ Regression Assumptions Testing  
✅ **Multicollinearity Check:** Dropped variables with **VIF > 5**  
✅ **Mean of Residuals:** Verified it is close to zero  
✅ **Linearity Check:** Ensured **no pattern** in the residual plot  
✅ **Homoscedasticity Test:** Residuals have **constant variance**  
✅ **Normality Check:** Residuals follow a **normal distribution**  

### 5️⃣ Model Evaluation  
🔹 **Mean Absolute Error (MAE)**  
🔹 **Root Mean Squared Error (RMSE)**  
🔹 **R² & Adjusted R² Score**  
🔹 **Train vs Test Performance Comparison**  

---

## 📊 Key Insights  

🔹 **Most Crucial Factors:**  
✔ **CGPA, GRE Score, and TOEFL Score** have the highest impact on admission chances.  
✔ **SOP, LOR, and University Rating** contribute but are **less significant**.  
✔ **Research Experience** is **critical for higher-rated universities** but less relevant for lower-rated ones.  

🔹 **Statistical Observations:**  
✔ **High University Ratings make admission highly competitive.**  
✔ **Non-normality of residuals affects statistical reliability, suggesting non-linear models could be explored.**  
✔ **Linear Regression outperforms Lasso and Ridge in terms of R² but may be sensitive to outliers.**  

---

## 🎯 Recommendations  

📌 **Enhancing the Model:**  
- **Include additional features** (e.g., Alumni data, Extra-curriculars, Essay Analysis).  
- **Use real university rankings** (e.g., **QS World Rankings** instead of a simple rating scale).  
- **Explore non-linear models** (e.g., Decision Trees, Random Forest).  
- **Perform Hypothesis Testing** on essay sentiment and sports achievements to measure impact.  
- **Regular Model Retraining** with fresh admission data.  

📌 **Business Impact:**  
- **Helps students** assess **realistic** admission chances.  
- **Optimizes marketing strategies** for Jamboree based on high-impact factors.  
- **Enhances admissions consultancy services** by providing **data-driven insights**.  

---

---

## 🚀 Tools & Technologies  
- **Python** (`pandas`, `numpy`, `seaborn`, `matplotlib`, `scipy.stats`)  
- **Regression Models** (`statsmodels`, `sklearn.linear_model`)  
- **Feature Selection** (`Variance Inflation Factor - VIF`)  
- **Evaluation Metrics** (`MAE`, `RMSE`, `R²`, `Adjusted R²`)  

---

## 📢 Conclusion  
This project successfully predicts **graduate admission chances** using **Linear Regression**. The analysis provides Jamboree with **valuable insights** into key factors affecting admissions, helping students make **informed decisions**.  

🔗 **Explore the full analysis in the Jupyter Notebooks!** 🚀  

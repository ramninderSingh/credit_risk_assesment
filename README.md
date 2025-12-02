# Credit Risk Classification using Machine Learning

This project builds an end-to-end **credit risk classification system** to predict customer approval categories (**P1, P2, P3, P4**) using machine learning techniques. It includes data cleaning, feature engineering, statistical tests, model building, hyperparameter tuning, and feature importance extraction.

---

##  Project Workflow

### **1. Data Preprocessing**
- Load datasets from Excel files  
- Remove invalid entries (e.g., `-99999`)  
- Merge datasets using `PROSPECTID`  
- Identify and process categorical + numerical features  

### **2. Statistical Feature Selection**
- **Chi-Square Test** for categorical feature significance  
- **VIF (Variance Inflation Factor)** to remove multicollinearity  
- **ANOVA** to keep numerical features with significant variance  

### **3. Feature Engineering**
- Ordinal encoding for EDUCATION  
- One-hot encoding for categorical variables  
- Standard scaling for selected numerical columns  

### **4. Machine Learning Models**
Implemented and compared:
- **Random Forest Classifier**
- **XGBoost (best performing)**
- **Decision Tree Classifier**

### **5. Hyperparameter Tuning**
Used GridSearchCV to optimize:
- `n_estimators`
- `max_depth`
- `learning_rate`

### **6. Model Saving**
The final best model is saved using Joblib:


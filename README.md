# 🏠 House Price Prediction Analysis

## 📌 Overview
In this project we explore residential property listings from major cities in Bangladesh and builds machine learning models to predict house prices based on property features. It includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and evaluation.

---

## 📊 Dataset
The dataset contains property listings from the following cities in Bangladesh:
- Dhaka  
- Chattogram  
- Cumilla  
- Narayanganj City  
- Gazipur  

### Features
- **Title**: Property description  
- **Bedrooms**: Number of bedrooms  
- **Bathrooms**: Number of bathrooms  
- **Floor_no**: Floor number  
- **Occupancy_status**: Vacant or occupied  
- **Floor_area**: Area in square feet  
- **City**: City name  
- **Location**: Specific area/address  
- **Price_in_taka**: Property price in BDT  

---

## 🧹 Data Preprocessing
- Converted `Floor_no` and `Price_in_taka` from object to numeric types  
- Handled missing values  
- Detected and treated outliers  
- Encoded categorical variables  
- Prepared dataset for machine learning models  

---

## 📈 Exploratory Data Analysis (EDA)

### Key Insights
- Average house has **3 bedrooms** (range: 1–27)  
- Average house has **3 bathrooms** (range: 1–10)  
- Most properties are located on the **4th floor** (range: 1–18)  
- Average floor area: **1,476 sq. ft.** (range: 84–24,000 sq. ft.)  
- Average price: **৳11.66 million** (range: ৳1.05M–৳363.2M)  

---

## 🔗 Correlation with Price

| Feature      | Correlation |
|--------------|------------:|
| Floor Area   | 0.78        |
| Bathrooms    | 0.59        |
| Bedrooms     | 0.49        |

👉 Floor area is the strongest predictor of house price.

---

## 🤖 Model Performance

| Model                    | R² Score |
|-------------------------|---------:|
| Random Forest           | 0.75     |
| Gradient Boosting       | 0.74     |
| K-Nearest Neighbors     | 0.71     |
| Decision Tree           | 0.68     |
| Support Vector Regressor| 0.61     |
| Ridge Regression        | 0.49     |
| Linear Regression       | 0.49     |
| AdaBoost                | 0.18     |

---

## 🏆 Best Model
The **Random Forest Regressor** achieved the best performance with an **R² score of 0.75**, capturing non-linear relationships in the dataset effectively.

---

## 🛠️ Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 📌 Conclusion
The study shows that **floor area, bathrooms, and bedrooms** are the most important factors influencing house prices. Ensemble models (Random Forest, Gradient Boosting) performed significantly better than linear models, indicating strong non-linear patterns in the data.

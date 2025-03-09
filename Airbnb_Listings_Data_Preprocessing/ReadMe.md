# **Barcelona Airbnb Data Preprocessing & Analysis**

## Project Overview
This project focuses on **cleaning, transforming, and structuring Barcelona Airbnb listings data** to prepare it for further analysis and predictive modeling. The dataset initially contained **75 columns and 17,231 rows**, which were **filtered, optimized, and engineered** to retain only meaningful features.

---
## **Tools Used**
- JMP

## **Techniques Used**
### **1️⃣ Data Cleaning**
- Dropped **63 columns** with no predictive value (IDs, URLs, redundant text fields).
- Removed missing values from critical variables and performed imputations where necessary.
- Standardized categorical values to ensure consistency.

### **2️⃣ Feature Engineering**
- Extracted **structured numerical features** from text-based columns (e.g., bedrooms count from listing names).
- Created **binary indicator columns** for key amenities (`has_wifi`, `has_parking`, etc.).
- One-hot encoded categorical variables (e.g., `room_type`, `neighborhood`).

### **3️⃣ Outlier Handling**
- Used **IQR & Z-score filtering** to remove extreme values in `beds`, `bathrooms`, and `review_scores_rating`.
- Checked **multivariate outliers** using **Mahalanobis Distance** and removed extreme cases.

### **4️⃣ Data Transformation**
- Normalized numerical features using **Min-Max Scaling** where required.
- Applied **log transformation** on price to handle skewness.

### **5️⃣ Final Dataset**
- Reduced to **10,725 rows and 21 key columns** after preprocessing.
- Removed **inconsistent records** to improve data quality.

---

## **Potential Use Cases**
- **Price Prediction Model** – Train a regression model to predict Airbnb listing prices.
- **Market Analysis** – Identify pricing trends and competitive factors in Barcelona.
- **Host Performance Evaluation** – Assess host responsiveness and credibility.

---



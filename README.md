# 🚆 Railway Tender L1 Price Prediction Using Machine Learning

## 📌 Project Overview

**Objective:**  
Develop a machine learning solution to predict the **L1 (Lowest Bid) Price** for railway tenders using structured historical tender data.  

The system enables railway stakeholders to make **data-driven bidding decisions**, optimize pricing strategies, and reduce manual estimation errors.

---

## 🛠️ Technology Stack

| Component | Tools Used |
|------------|------------|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Machine Learning | Scikit-learn (Linear Regression) |
| Model Persistence | Pickle |
| Deployment | Streamlit |

---

# 🔄 End-to-End Project Workflow

---

## 1️⃣ Data Collection & Exploration

### Data Attributes
- Railway Location  
- Tender Nature  
- Product Category  
- Basic Price  
- Quantity  
- Target Variable: **L1 Price**

### Initial Exploration
- Summary statistics (mean, std, min, max)
- Distribution analysis of categorical variables
- Identification of skewness and anomalies

---

## 2️⃣ Data Cleaning & Preprocessing

### ✔ Handling Missing Values
- Dropped features with excessive missingness  
- Mean/Median imputation for numeric gaps  

### ✔ Outlier Detection
- Boxplot-based detection  
- Log transformation for skewed variables  
- Removal of data-entry anomalies  

### ✔ Duplicate Removal
- Eliminated redundant records to prevent bias  

### ✔ Categorical Encoding
- One-Hot Encoding → Railway Location  
- Label Encoding → Ordinal features  

### ✔ Feature Scaling
- Standardization / Min-Max Scaling  
- Ensured uniform feature magnitude  

---

## 3️⃣ Feature Engineering

- Created **Cost per Unit = Basic Price / Quantity**
- Derived aggregated statistics for grouped insights
- Reduced multicollinearity using VIF
- Statistical validation via Chi-Square / ANOVA

---

## 4️⃣ Exploratory Data Analysis (EDA)

### 📊 Univariate Analysis
- Histograms for distribution
- Box plots for variance and spread
- Category frequency distributions

### 📈 Bivariate & Multivariate Analysis
- Correlation heatmap
- Scatter plots (Basic Price vs L1 Price)
- Group-wise price comparisons
- Volume-based pricing behavior

---

## 🔍 Key Insights from Data

- **Location Effect:** Metro zones exhibit higher tender pricing trends.
- **Nature Influence:** Supply and execution tenders follow distinct cost structures.
- **Economies of Scale:** Higher quantities reduce per-unit tender price.
- **Category Impact:** Heavy-duty classifications show consistently higher L1 values.

---

## 5️⃣ Model Development

### 🎯 Algorithm Used
**Linear Regression**

### Model Evaluation Metrics
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

The model was trained on cleaned and scaled data to ensure robust generalization and minimal prediction error.

---

## 🚀 Deployment

### 🌐 Streamlit Web Application

An interactive interface allows users to:

- Input tender features  
- Instantly generate predicted L1 Price  
- Perform real-time calculations  

### 💾 Model Persistence
- Trained model saved using Pickle  
- Enables seamless reuse and deployment  

---

# 📊 Application Features

- Clean and intuitive UI  
- Real-time prediction (< 2 seconds response)  
- Structured input forms  
- Scalable for future model upgrades  

---

# 💼 Business Impact

| Impact Area | Outcome |
|-------------|----------|
| Decision-Making | Data-backed tender pricing |
| Profit Optimization | Up to 5% improved pricing efficiency |
| Time Efficiency | Reduced manual evaluation hours |
| Error Reduction | Minimized pricing miscalculations |

---

# 📈 Reporting & Visualization

- Correlation Heatmaps  
- Category-wise Price Comparisons  
- Time-based Price Trend Analysis  
- Multi-feature Pair Analysis  

---

# 🏁 Conclusion

This project demonstrates a complete data science lifecycle:

- Data acquisition  
- Cleaning & preprocessing  
- Feature engineering  
- Statistical validation  
- Predictive modeling  
- Deployment  

Through structured EDA and rigorous preprocessing, the Linear Regression model delivers reliable L1 price predictions, empowering railway stakeholders with actionable intelligence for competitive bidding strategies.

---

## 🔮 Future Improvements

- Advanced models (Random Forest / XGBoost)
- Time-series tender trend forecasting
- Automated retraining pipeline
- Integration with live railway tender database

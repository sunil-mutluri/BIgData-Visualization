# 🌬️ Big Data Visualization and Analysis of Renewable Wind Energy Consumption using PySpark in Amazon S3

## 📘 Abstract

This project analyzes wind energy consumption patterns across Europe using large-scale datasets processed with PySpark and stored in Amazon S3. It identifies temporal and regional trends in wind power generation, utilizing statistical and machine learning methods, and delivers insights through powerful visualizations. These findings can help inform policy-making and future investment in renewable energy.

---

## 🛠️ Tech Stack

- **PySpark** – for distributed data processing
- **Amazon S3** – cloud storage for large datasets
- **Matplotlib / Seaborn** – visual analytics and trend discovery
- **scikit-learn** – predictive modeling (Random Forest)
- **Google Colab** – cloud-based computation

---

## 📦 Dataset

- **Source**: [EMHIRES dataset via Kaggle](https://www.kaggle.com/datasets/alistairking/renewable-energy-consumption-in-the-u-s)
- **Type**: Hourly wind energy generation across European regions (1986–2015)
- **Key Features**:
  - `Year`, `Region`, `Wind Power (MW)`
  - Region codes (e.g., UKC1, DE11)
  - Hourly & monthly patterns
  - Predictive features like time-of-day, seasonality

---

## 📈 Key Results

### ✅ Monthly Wind Power Generation

UKC1 shows strong seasonal patterns with higher generation in winter. DE11 maintains a lower and consistent pattern across the year.

![Monthly Pattern](./monthly_generation_pattern.png)

---

### ✅ Top Countries by Wind Power Output

UK leads with the highest average generation, followed by Germany and France.

![Top Countries](./top_countries_generation.png)

---

### ✅ Predictive Modeling

- **Model Used**: RandomForestRegressor
- **Evaluation Metrics**:
  - RMSE: ~2.35
  - R² Score: 0.89
- **Important Features**: Time of day (Hour), Month, Region code
- **Feature Engineering**: Sine/Cosine transformations for cyclic temporal features

---

### 🔍 Correlation Analysis

- Strongest: FR10–ITC1 (0.65), DE11–ITC1 (0.62)
- Weakest: ES11–UKC1 (0.11)
- Interpretation: Weather/geographic similarities impact correlation

---

## 🔬 Analytics Used

| Type            | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| Descriptive     | Mean, standard deviation, distributions by region/month                    |
| Diagnostic      | Correlation matrices, anomaly detection                                     |
| Predictive      | Random forest model with feature importance and performance validation     |

---

## ✅ Use Cases

- 📊 **Policy Making**: Support investment decisions with generation stability trends  
- ⚡ **Energy Planning**: Forecast production levels by region & season  
- 🛠 **Infrastructure**: Guide expansion in high-output zones like UKC1 or FR10

---

## 📋 Test Cases Executed

1. ✅ Data import and structure validation  
2. ✅ Cleaning missing values and outlier removal  
3. ✅ Time-series visualizations  
4. ✅ Model training with performance tracking  
5. ✅ Regional comparison via correlation heatmaps

---

## 📂 Directory Structure

📁 project-root/
├── Data_Cleaning.ipynb
├── Data_Combining.ipynb
├── Data_Analytics_and_Modeling.ipynb
├── Data_Visualization.ipynb
├── project_report.pdf
├── monthly_generation_pattern.png
├── top_countries_generation.png

yaml
Copy
Edit

---

## 🙌 Contributors

- **Name**: Sunil Kumar Mutluri  
- **University**: University of Missouri–Kansas City  
- **Tools Used**: PySpark, AWS S3, Python (Pandas, Sklearn, Seaborn)

---

## 📚 References

- https://www.kaggle.com/datasets/pythonafroz/wind-and-solar-power-generation-data  
- https://aws.amazon.com/s3/  
- https://scikit-learn.org/  
- https://www.geeksforgeeks.org/types-of-analytics/  

---

> "Empowering clean energy planning through big data and intelligent systems."

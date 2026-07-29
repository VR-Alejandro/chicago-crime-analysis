# 🏙️ Chicago Crime Prediction & Analysis

> End-to-end Data Analytics project focused on analyzing more than **1.4 million crime records** from Chicago (2020–2024) and developing a **Machine Learning model** to predict crime levels by Community Area for **2025–2027**.

<p align="center">
  <img src="dashboard/dashboard_preview.png" width="900">
</p>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

---

# 📖 Overview

This project was developed as the **final project of the Neoland Data Analytics Bootcamp**.

Using more than **1.4 million crime records**, socioeconomic indicators and Machine Learning techniques, we built a predictive model capable of estimating crime levels by **Community Area** for the years **2025–2027**.

The final solution combines:

- 📊 Exploratory Data Analysis (EDA)
- 🗄 SQL Server analytics
- 📈 Socioeconomic data integration
- 🤖 Random Forest regression model
- 📍 Interactive Power BI dashboard

---

# 👥 Team

This project was developed by a team of **4 Data Analytics students**.

## My Contributions

- ✅ Data Cleaning & Preprocessing
- ✅ Exploratory Data Analysis (EDA)
- ✅ SQL Server development (CTEs & Window Functions)
- ✅ Geographic heatmaps with Folium
- ✅ Temporal and seasonal crime analysis
- ✅ Feature Engineering
- ✅ Power BI Dashboard development
- ✅ Co-development of the final Random Forest model

---

# 📂 Repository Structure

```text
chicago-crime-analysis/

│
├── data/
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_exploracion_modelos.ipynb
│   └── 03_modelo_final.ipynb
│
├── dashboard/
│   └── dashboard_preview.png
│
├── outputs/
│
├── presentacion/
│   └── Chicago_Crime_Presentacion.pdf
│
└── README.md
```

---

# 📊 Dataset

The main dataset contains approximately **1.45 million crime records** collected from the **Chicago Data Portal (2020–2024)**.

Additional socioeconomic variables include:

- Population
- Poverty Rate
- Unemployment Rate
- Per Capita Income
- Education Level

These variables were obtained from the **Chicago Health Atlas**.

> Due to GitHub size limitations, the main crime dataset is not included in this repository.

---

# 🔍 Methodology

## 1️⃣ Exploratory Data Analysis

- Missing values treatment
- Duplicate removal
- Feature extraction
- Temporal analysis
- Geographic visualization
- Crime rate normalization
- SQL analytical queries

### Main Findings

- Crime decreased between 2020 and 2024.
- Theft and Battery were the most frequent crimes.
- Summer months showed higher crime activity.
- Crime intensity varied significantly across Community Areas.

---

## 2️⃣ Model Exploration

Several approaches were evaluated before selecting the final model.

| Model | R² | Main Limitation |
|------|------:|----------------|
| PCA + Linear Regression | 0.30 | Socioeconomic variables at record level |
| PCA + Linear Regression (Aggregated) | 0.51 | Only 77 observations |
| Linear Trend | Low | Very limited historical data |
| 10-Year Dataset | ≈0 | Socioeconomic variables lacked yearly resolution |

### Key Learning

> The main bottleneck was **data granularity**, not the Machine Learning algorithm itself.

---

## 3️⃣ Final Model

Random Forest Regressor (300 Trees)

### Features

- Year
- Population
- Poverty Rate
- Unemployment Rate
- Per Capita Income
- Education Level

| Model | MAE | RMSE | R² |
|------|------:|------:|------:|
| 🥇 Random Forest | **331.3** | **541.5** | **0.977** |
| Linear Regression | 1390.7 | 1880.6 | 0.633 |
| Dummy Regressor | 2636.7 | 3601.1 | -0.0004 |

---

# 📈 Key Results

- ✅ R² = **0.977**
- ✅ Predictions generated for **2025–2027**
- ✅ Significant improvement over Linear Regression
- ✅ Interactive Power BI dashboard developed
- ✅ More than **1.4 million records analyzed**

---

# 📊 Power BI Dashboard

The dashboard allows users to explore crime patterns through:

- 🗺 Crime Risk Map
- 📈 KPIs
- 🚔 Arrest Rate
- 🏘 Community Area filters
- 📊 Top Crime Types
- 🎯 Crime Risk Index

### Featured Areas

- 🔴 **Fuller Park** → Highest predicted crime index (94.06/100)
- 🟢 **Forest Glen** → Lowest predicted crime index (1.69/100)

---

# 💡 Business Insights

The project identified several insights that may support public safety planning:

- Crime activity peaks during summer months.
- Theft and Battery consistently remain the most common crimes.
- Socioeconomic indicators significantly improve predictive performance.
- Some Community Areas remain consistently above average, even after population normalization.

---

# 🛠 Tech Stack

### Programming

- Python
- Pandas
- NumPy

### Visualization

- Matplotlib
- Seaborn
- Folium
- Power BI

### Machine Learning

- Scikit-learn
- Random Forest
- Linear Regression

### Database

- SQL Server
- T-SQL
- CTEs
- Window Functions

---

# 🚀 Future Improvements

- Compare Random Forest with XGBoost and LightGBM.
- Deploy the model using Streamlit.
- Automate data extraction through the Chicago API.
- Include yearly socioeconomic variables.

---

# ▶️ How to Run

```bash
git clone https://github.com/VR-Alejandro/chicago-crime-analysis.git

cd chicago-crime-analysis

pip install pandas numpy matplotlib seaborn folium scikit-learn statsmodels openpyxl

jupyter notebook notebooks/01_eda.ipynb
```

---

# 👨‍💻 Author

**Alejandro Villodres Romero**

Junior Data Analyst

📍 Málaga, Spain

💼 LinkedIn

💻 GitHub

📧 alejandrovillodres.job@gmail.com

---

⭐ If you found this project interesting, feel free to leave a star or connect with me on LinkedIn.

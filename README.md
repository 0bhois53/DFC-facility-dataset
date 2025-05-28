# Dialysis Facility Dataset Analysis and Visualization

![Project Status](https://img.shields.io/badge/status-completed-brightgreen)

## 📊 Overview

This project analyzes and visualizes the **CMS Dialysis Facility Compare (DFC)** dataset to evaluate the performance of dialysis centers across the United States. The project includes data preprocessing, exploratory data analysis, predictive modeling, and interactive dashboards to help healthcare stakeholders make informed decisions.

---

## 🎯 Objectives

- Perform univariate, bivariate, and multivariate analysis on the DFC dataset.
- Create interactive dashboards and visualizations for key insights.
- Predict Five-Star Ratings for dialysis facilities using machine learning.

---

## 🧾 Dataset

**Source:** [CMS Dialysis Facility Dataset](https://data.cms.gov/provider-data/dataset/23ew-n7w9)

The dataset includes:
- Facility info (e.g., name, location, profit status)
- Clinical outcomes (e.g., mortality, readmission, infection rates)
- Service offerings (e.g., home hemodialysis training)
- Quality metrics including Five-Star Ratings

---

## ⚙️ Workflow

### 1. Data Preparation
- Reduced original 7574-row dataset to 2500 rows for efficiency.
- Dropped non-essential or high-missing-value columns (from 140 → 46).
- Applied both **Simple Statistical Imputation** and **KNN Imputation**.

### 2. Exploratory Data Analysis (EDA)
- Visualized rating distributions, service types, geographic clustering, etc.
- Used `matplotlib`, `seaborn`, and `plotly` for data visualizations.

### 3. Dashboards
- Created with **Tableau**
- Includes:
  - Statewise metrics
  - Facility ownership distribution
  - Service availability
  - Mortality/hospitalization rates
  - Interactive filters

### 4. Prediction Model
- Target: `Five Star Rating`
- Models:
  - Random Forest (Accuracy: ~85%)
  - Gradient Boosting (Accuracy: ~58%)
- Included classification report and feature importance analysis
- Interactive script for real-time prediction by CMS ID

---

## 📂 Repository Structure

```plaintext
├── data/
│   ├── dfc_facility.csv            # Original dataset
│   └── dfc_reduced.csv             # Cleaned dataset
│
├── notebooks/
│   ├── eda.ipynb                   # Exploratory Data Analysis
│
├── dashboards/
│   └── dialysis_dashboard.twbx     # Tableau dashboard file
│
├── README.md
└── requirements.txt                # Python dependencies


```
## 🚧 Limitations
- High percentage of missing data in some critical metrics.
- Imputation required careful handling of mixed data types.
- Prediction less accurate for facilities with extreme ratings (1-star or 5-star).

## 📈 Future Work
- Incorporate multi-year trends for time-series analysis.
- Deploy ML model as an API for public access.
- Explore patient feedback via sentiment analysis.

## 👨‍💻 Author
Sanket Suresh Bhoir
Course: COM-724 | AE2 Assignment (2024–25)
Module Leader: Raza Hasan

## 🧪 Tools & Libraries
- Python (pandas, sklearn, seaborn, matplotlib)
- Tableau for dashboard visualizations
- Jupyter Notebook for code development

## 📄 References
- CMS Dataset: Dialysis Facility Compare
- Bhatnagar, A., Reaves, A. C., Weiner, D. E., & Erickson, K. F. (2025). Commercial
 Health Insurance and Quality of Care in US Dialysis Facilities. Kidney Medicine, 7(5),100992.
- Flanagin, E. P., Chivate, Y., & Weiner, D. E. (2020). Home Dialysis in the United
 States: A Roadmap for Increasing Peritoneal Dialysis Utilization. American Journal of
 Kidney Diseases, 75(3), 413-416.
- Kim, S., Wu, F., Dahlerus, C., Chyn, D., Li, Y., & Messana, J. M. (2019). Comparative
 effectiveness analysis of Medicare dialysis facility survey processes. PLoS ONE, 14(4),
 e0216038.
- Patzer, R. E., Plantinga, L., Krisher, J., & Pastan, S. O. (2014). Dialysis Facility and
 Network Factors Associated With Low Kidney Transplantation Rates Among United
 States Dialysis Facilities. American Journal of Transplantation, 14, 1562-1572.
- Pozniak, A., & Pearson, J. (2018). The Dialysis Facility Compare Five-Star Rating
 System at 2 Years. Clinical Journal of the American Society of Nephrology, 13, 474-476.
- Nazik Alturki, Abdulaziz Altamimi, Muhammad Umer, Oumaima Saidani, Amal Al
shardan, Shtwai Alsubai, Marwan Omar, Imran Ashraf, Improving Prediction of Chronic
 Kidney Disease Using KNN Imputed SMOTE Features and TrioNet Model, CMES
Computer Modeling in Engineering and Sciences, Volume 139, Issue 3,2024,Pages 3513
3534,ISSN 1526-1492, https://doi.org/10.32604/cmes.2023.045868.



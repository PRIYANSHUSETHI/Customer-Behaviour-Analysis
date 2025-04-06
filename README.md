
# 📊 Customer Behavior Analysis

This project analyzes ecommerce customer behavior to uncover insights, identify churn, and segment customers based on engagement and lifetime value. It uses Python for data processing, visualization, and customer analytics.

---

## 📁 Project Structure

```
customer_behavior_analysis/
├── customer_behavious_analysis.py
├── ecommerce_customer_data.csv  # (Assumed input dataset)
└── README.md
```

---

## 🚀 Key Features

### 1. Data Loading & Preprocessing
- Loads customer interaction data using `pandas`
- Cleans missing values and prepares data for analysis

### 2. Descriptive Statistics
- Summarizes numerical and categorical columns with `describe()`

### 3. Visualizations
- Age distribution histogram
- Gender and device usage bar charts
- Browsing vs. viewing scatter plot
- CLV box plots
- Customer funnel (Visitors → Purchasers)
- Churn analysis across demographics

### 4. Customer Lifetime Value (CLV)
- Feature selection:
  - `Total_Purchases`
  - `Items_Added_to_Cart`
  - `Product_Browsing_Time`
- Feature scaling with `StandardScaler`
- Dimensionality reduction using `PCA`
- CLV scoring and segmentation into 4 tiers: Low, Medium, High, Very High

### 5. Customer Funnel Analysis
- Tracks user journey:
  - Visited site
  - Viewed products
  - Added to cart
  - Completed purchase
- Funnel chart using `plotly.express`

### 6. Churn Analysis
- Defines churn as `Total_Purchases == 0`
- Analyzes churn rates by:
  - Gender
  - Device Type
  - Location
- Visualized using `seaborn.barplot`

---

## 📦 Dependencies

Install required packages with:

```bash
pip install pandas plotly seaborn matplotlib scikit-learn
```

---

## 🧪 How to Run

1. Clone the repo:

```bash
git clone https://github.com/yourusername/customer_behavior_analysis.git
cd customer_behavior_analysis
```

2. Place your dataset (`ecommerce_customer_data.csv`) in the project folder.

3. Run the script:

```bash
python customer_behavious_analysis.py
```

> Note: Some visualizations open in a browser or Jupyter environment.

---

## 🧠 Libraries Used

- `pandas`: Data loading and transformation
- `numpy`: Numerical computations
- `matplotlib`, `seaborn`: Data visualization
- `plotly.express`, `plotly.graph_objects`: Interactive visualizations
- `sklearn.preprocessing.StandardScaler`: Feature normalization
- `sklearn.decomposition.PCA`: Principal Component Analysis for CLV

---

## 🛠️ Future Enhancements

- Predictive churn modeling with classification algorithms
- Cohort analysis for retention tracking
- Streamlit or Dash dashboard for live KPIs

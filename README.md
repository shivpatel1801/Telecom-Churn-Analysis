Telecom Customer Churn Analysis

Project Overview
This project focuses on **exploring and understanding customer churn behavior** in a telecom company.  
Using exploratory data analysis (EDA), visualizations, and summary statistics, the goal is to **identify key drivers that influence customer retention and churn**.

---

Objectives
- Analyze customer demographics and service usage patterns.
- Understand how contract types, tenure, and payment methods affect churn.
- Visualize churn distribution across key categories.
- Provide actionable business insights to improve customer retention.

---

Data Preparation
- Replaced missing or blank values in `TotalCharges` with `0` (representing new customers with zero tenure).
- Converted `SeniorCitizen` from binary (0/1) to categorical (`Yes`/`No`) for better readability.
- Cleaned categorical variables for consistent formatting.
- Performed univariate and bivariate analysis to understand patterns driving churn.

---

Key Insights

| Factor | Observation | Churn Impact |
|:--|:--|:--|
| **Overall Churn Rate** | 26.54% of total customers churned | – |
| **Senior Citizens** | 42% churned vs. 24% non-seniors | High risk |
| **Contract Type** | Month-to-month: 43% churn; One-year: 11%; Two-year: 3% | Strong negative correlation |
| **Tenure** | < 12 months: >50% churn; >3 years: <10% churn | High early churn |
| **Internet Service** | Fiber optic users: ~42% churn; DSL users: ~19% | Fiber users more likely to churn |
| **Payment Method** | Electronic checks: 45% churn; others: 15–20% | Electronic check users churn more |

---

Visualizations
The notebook includes several visualizations:
- **Churn distribution pie chart** showing total churn rate (26.54%).
- **Bar charts** comparing churn by:
  - Senior citizen status  
  - Contract type  
  - Tenure group  
  - Payment method  
  - Internet service type
  **Stacked bar plots** displaying churn vs. non-churn percentages per category.

---

Recommendations
1. Focus retention efforts on new customers (tenure < 1 year).
2. Encourage migration from month-to-month to longer-term contracts via loyalty discounts.
3. Create senior-friendly plans to reduce churn among older customers.
4. Promote bundled add-ons (e.g., Online Security, Tech Support) that improve satisfaction.
5. Investigate high churn among electronic check users and promote stable payment methods.

---

Files in This Repository
| File | Description |
|------|--------------|
| `Teleco_churn_anylsis.ipynb` | Jupyter notebook with full exploratory data analysis |
| `Telecom_Churn_Executive_Summary.docx` | Executive summary report for management |
| `README.md` | Project overview and documentation |

---

 Technologies Used
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Jupyter Notebook
- Microsoft Word(for the final report)
- GitHub (for version control and sharing)

---

How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/telecom-churn-analysis.git

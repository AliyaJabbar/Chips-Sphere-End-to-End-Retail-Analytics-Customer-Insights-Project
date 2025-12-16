# Chips-Sphere-End-to-End-Retail-Analytics-Customer-Insights-Project


#🏆 Chip Sphere Retail : Margin Optimization through Statistical Customer Segmentation
##📝 Project Overview:
This project delivers an end-to-end data analysis solution for a competitive chip retail market. The core objective was to move beyond generalized marketing and promotion strategies by performing rigorous statistical segmentation. The outcome is a dynamic Power BI dashboard that identifies the highest-value customer segment, quantifies their product preferences (Affinity), and provides clear, actionable recommendations for sales, inventory, and merchandising teams to maximize profit margins.

##❓ Problem & Solution| Area | Description |
| --- | --- |
| **Business Problem** | General promotions and undifferentiated stocking of product categories lead to suboptimal profit margins and inefficient marketing spend in a fiercely competitive market. The lack of granular insight meant low-value customers often received premium product promotions. |
| **Analytical Solution** | **1. Segmentation:** Merged transaction and customer demographic data (\text{72,000+} customers, \text{2.64} lakh transactions). **2. Validation:** Used hypothesis testing (T-Test) to statistically isolate the most price-tolerant segment. **3. Strategy:** Developed an Affinity Index to determine the specific brands and pack sizes to be exclusively targeted to this high-value group. |
| **Key Insight** | The **Mainstream Young Singles/Couples** segment is the most profitable, exhibiting a **highest Average Price Paid of \text{\$4.07}**, confirming their high price tolerance compared to other groups. |

##📊 Key Insights & Product Strategy| Insight Category | Finding | Actionable Strategy |
| --- | --- | --- |
| **High-Value Target** | **Mainstream Young Singles/Couples** were statistically confirmed as the highest value group based on Avg Price Per Unit. | Focus promotional budget entirely on this segment to maximize margin. |
| **Brand Affinity** | Target segment shows an Affinity Index > 1.23 for premium brands like **TYRRELLS** and **KETTLE**. | Prioritize premium brand placement (eye-level shelves, end-caps) and limit discounts to value-add promotions only. |
| **Pack Size Affinity** | Target segment shows an Affinity Index > 1.27 for **large pack sizes (\text{270g}+).** | Increase inventory allocation for larger, higher-margin pack sizes, especially in high-penetration stores. |
| **Geographic Performance** | Identified stores with the **Highest Target Segment Penetration Rate** via a custom DAX measure. | Direct sales force efforts and specialized merchandising activities to these high-performing geographic locations. |

##💻 Technical Stack & Methodology###Python (Data Preparation & Statistical Modeling)| Library | Use Case |
| --- | --- |
| **Pandas** | Data cleaning, merging two disparate datasets (`customer_data` & `transaction_data`), feature engineering (e.g., calculating Price Per Unit). |
| **NumPy** | Numerical operations and array handling for efficient data manipulation. |
| **SciPy/Statsmodels** | Execution of the **Two-Sample T-Test** to rigorously validate the statistical significance (p < 0.05) of the average price difference between the target segment and the general market. |

###Power BI & DAX (Visualization & KPI Generation)The final analysis is presented in a **4-Page Power BI Dashboard** (Market Pulse, Segmentation Validation, Affinity Strategy, Geographic Exploration).

| DAX Function | Purpose in Project |
| --- | --- |
| **`CALCULATE`** | Core function used with `FILTER` to isolate metrics for the specific target segment (e.g., `[Target Segment Total Sales]`). |
| **`DIVIDE`** | Created robust KPI measures, such as the `[Target Segment Avg Price]` ratio: \text{SALES / QTY} (includes safe division). |
| **`DISTINCTCOUNT`** | Calculated unique customers and transactions, crucial for the `[Target Segment Penetration Rate]` and segment size scatter plots. |
| **`MAXX / TOPN`** | Used for identifying the non-numeric ID of the top-performing store: `[Top Performing Store ID (Sales)]`. |

##🚀 Impact & Value DeliveredThe project delivers a clear ROI pathway for the business:

* **Strategic Focus:** Identified the **top 5% of customers** responsible for the highest margin potential.
* **Operational Efficiency:** Provided store teams with the **Target Segment Penetration Rate**, enabling smart inventory allocation and targeted planogram adjustments.
* **De-risked Strategy:** Used **statistical validation** (T-Test) and visual confirmation (Scatter Plot, Box Plot) to ensure recommendations were based on rigorous analysis, not just descriptive statistics.

---

[Link to Power BI Dashboard (Web Link/Video Demo)]

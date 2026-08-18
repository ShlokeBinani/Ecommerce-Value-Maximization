# E-Commerce Value Maximization: An RFM & Behavioral Clustering Approach

**Author:** Shloke Binani

## Project Overview
This project demonstrates a full-cycle, professional data analytics workflow, transforming raw transactional e-commerce data into a high-impact, actionable strategic plan. By combining advanced SQL data warehousing, unsupervised machine learning (hybrid DBSCAN + K-Means clustering), and an interactive Microsoft Power BI dashboard, this project uncovers hidden buyer segments and provides concrete revenue growth strategies.

**Dashboard Preview:**
![Dashboard Screenshot](dashboard_screenshot.png) 

---

## Technology & Architecture
This project utilizes a multi-tiered architecture to mirror a professional enterprise data environment:

* **Data Warehouse & Transformation:** **SQL** (via SQLite) for relational data storage, cleaning, and the calculation of Recency, Frequency, and Monetary (RFM) metrics using advanced Common Table Expressions (CTEs).
* **Advanced Analytics & Machine Learning:** **Python** (Pandas, Scikit-learn) for feature scaling, outlier handling via DBSCAN, unsupervised K-Means customer segmentation, and cluster validation using Silhouette Scores.
* **Business Intelligence & Storytelling:** **Microsoft Power BI** for creating an interactive dashboard that visualizes segmentation metrics, customer lifetime value, and strategic recommendations.

---

## Key Findings: Customer Personas
The hybrid machine learning pipeline successfully identified four distinct and statistically significant customer personas based on their purchasing behavior:

| Persona | Data Profile & Characteristics |
| :--- | :--- |
| **High-Value Reseller** | Very recent, highly frequent, and high-spending core customers driving significant platform revenue. |
| **Loyal Homemaker** | The largest group of consistent, moderately recent, and regular shoppers. |
| **At-Risk Shopper** | A substantial segment of buyers who have experienced extended periods of inactivity and are high-probability churn risks. |
| **Anomalous Shopper** | A niche, high-value outlier group characterized by erratic or bulk purchasing patterns. |

---

## Actionable Business Recommendations
Grounded in the behavioral profiles of each cluster, a multi-faceted commercial strategy was developed to optimize retention and maximize lifetime value (LTV):

| Persona | Recommended Business Action |
| :--- | :--- |
| **High-Value Reseller** | Launch a dedicated **"Business Program"** offering tiered bulk pricing, dedicated account management, and early access to product lines. |
| **Loyal Homemaker** | Introduce automated **"Smart Bundles"** and a flexible "Subscribe & Save" feature to drive predictable repeat orders. |
| **At-Risk Shopper** | Execute a targeted **"Win-Back" campaign** utilizing personalized, time-sensitive incentive structures to re-engage dormant accounts. |
| **Anomalous Shopper** | **Isolate and Investigate** transaction logs to vet for potential B2B partnership opportunities or anomalies. |

---

## Repository Structure & Usage

1. **`customer_segmentation.ipynb`**: Contains the complete Python workflow, including data preprocessing, feature engineering, DBSCAN outlier filtering, K-Means clustering optimization, and evaluation metrics.
2. **`rfm_query.sql`**: Houses the advanced SQL queries and CTE structures used for transactional aggregation and RFM score derivation.
3. **`customer_segments_final.csv`**: The final processed dataset containing assigned cluster labels and RFM metrics, optimized for direct import into Power BI or other visualization tools.
# Customer Segmentation via Unsupervised Learning

This project applies unsupervised machine learning to segment customers based on behavioral and demographic attributes. The aim is to uncover distinct customer groups to support personalized marketing, product targeting, and operational decisions.

---

## 📁 Dataset

- **Source:** [Mall Customers Dataset on Kaggle](https://www.kaggle.com/datasets/shwetabh123/mall-customers)
- **Fields:** Includes gender, age, annual income, and spending score for each customer.

---

## ⚙️ Clustering Techniques

Three clustering algorithms were applied and compared:

1. **K-Means Clustering**
2. **Agglomerative (Hierarchical) Clustering**
3. **DBSCAN (Density-Based Spatial Clustering)**

---

## Model Evaluation

Evaluation was performed using the **Silhouette Score**, which measures how well data points fit within their assigned clusters.

| Model                   | Silhouette Score | Interpretation                                                  |
|-------------------------|------------------|------------------------------------------------------------------|
| K-Means                 | 0.4166           | Best-defined clusters; well-separated and compact               |
| Agglomerative Clustering| 0.3900           | Good structure; slightly less compact than K-Means              |
| DBSCAN                  | 0.1099           | Weak structure; mostly detects outliers or noise                |

---

---

## ✅ Final Model: K-Means Clustering

After evaluating all models, **K-Means** was selected as the final clustering algorithm due to its superior Silhouette Score and well-defined segments.

### 🔹 K-Means Cluster Profiles

| Cluster | Size | Description                                                  | Business Relevance                                                   |
|---------|------|--------------------------------------------------------------|------------------------------------------------------------------------|
| 4       | 54   | Most common cluster; moderate spend, duration, and frequency | Represents the bulk of customers; this is a stable segment             |
| 0       | 47   | High transaction count, moderate value                       | Regular customers; consider retention and loyalty strategies           |
| 2       | 40   | Low value, short interaction durations                       | Possibly bargain seekers or new users; potential upsell target         |
| 1       | 39   | High-value, short-duration customers                         | Fast and premium service segment; prioritize efficiency                |
| 3       | 20   | Long interaction durations, varied spend                     | May indicate service delays or complex interactions; investigate        |

---

## Business Insight

- **K-Means** provided the most interpretable and actionable customer segments.
- Clusters reveal opportunities for retention, upselling, operational efficiency, and issue resolution.
- Future strategies can be tailored to each cluster to maximize customer satisfaction and business performance.


---

## 🛠 Environment

- Python with `venv` virtual environment (included in repo)
- To run:
  ```bash
  python -m venv .venv
  .venv\Scripts\activate  # Windows
  pip install -r requirements.txt
  jupyter notebook

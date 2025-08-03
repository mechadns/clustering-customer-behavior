# Mall Customer Segmentation

This project applies **unsupervised machine learning** techniques to segment customers of a shopping mall based on their spending patterns and demographic details.  
It compares multiple clustering algorithms to identify distinct customer groups, enabling targeted marketing strategies.

---

## 📌 Project Overview

Customer segmentation is crucial for businesses to:
- Understand customer behavior.
- Improve marketing efficiency.
- Personalize customer experiences.

In this project, we:
1. **Load and explore** mall customer data.
2. **Preprocess** the dataset.
3. **Apply multiple clustering algorithms** to identify customer segments.
4. **Visualize** and compare the results for actionable insights.

---

## 📂 Dataset

The dataset contains the following columns:
- **CustomerID** – Unique ID assigned to each customer.
- **Gender** – Customer gender (`Male` / `Female`).
- **Age** – Age of the customer.
- **Annual Income (k$)** – Annual income in thousands.
- **Spending Score (1-100)** – Score assigned based on spending behavior.

> The dataset is typically available as `Mall_Customers.csv`.

---

## ⚙️ Methods Used

### 1. **K-Means Clustering**
- Partitions customers into `k` clusters by minimizing variance within clusters.
- Requires choosing `k` (found using the **Elbow Method**).

### 2. **Agglomerative Hierarchical Clustering**
- Builds a hierarchy of clusters by iteratively merging the closest pairs.
- Dendrograms are used to decide the number of clusters.

### 3. **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**
- Groups together customers with high density of points.
- Detects outliers as noise.
- Does not require specifying the number of clusters.

---

## 🛠️ Technologies

- Python
- NumPy, Pandas
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🚀 How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/mall-customer-segmentation.git
   cd mall-customer-segmentation
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook**:
   ```bash
   jupyter notebook mall_customer_segmentation.ipynb
   ```

---

## 📊 Results

- **K-Means**: Clear, well-separated clusters based on spending score and income.
- **Agglomerative Clustering**: Similar grouping to K-Means, but reveals hierarchical relationships.
- **DBSCAN**: Detected smaller dense groups and flagged outliers, useful for identifying niche customer segments.

---

## 📈 Sample Visualizations

| Algorithm | Example Output |
|-----------|---------------|
| K-Means | ![K-Means Clusters](images/kmeans_clusters.png) |
| Agglomerative | ![Agglomerative Clusters](images/agglomerative_clusters.png) |
| DBSCAN | ![DBSCAN Clusters](images/dbscan_clusters.png) |

---

## 📜 License

This project is licensed under the MIT License.

---

## ✨ Author

- **Your Name** – [your.email@example.com](mailto:your.email@example.com)  
  GitHub: [@yourusername](https://github.com/yourusername)

---

> 💡 *Tip: You can extend this project by adding more features (e.g., purchase history), testing other clustering algorithms (e.g., Mean Shift, Birch), or combining clustering with supervised learning for predictive analytics.*

# Mall Customer Segmentation

This project applies **unsupervised machine learning** techniques to segment customers of a shopping mall based on their spending patterns and demographic details.  
It compares multiple clustering algorithms to identify distinct customer groups, enabling targeted marketing strategies.

---

## Project Overview

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

> The dataset is obtained from [Mall_Customers](https://www.kaggle.com/datasets/shwetabh123/mall-customers).
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

##  How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/mechadns/clustering-customer-behavior.git
   cd clustering-customer-behavior
   ```

2. **Install dependencies**:
   - Python 3.11+

3. **Run the notebook**:
   ```bash
   jupyter notebook mall_customer_segmentation.ipynb
   ```

---

## Results

- **K-Means**: Clear, well-separated clusters based on spending score and income.
- **Agglomerative Clustering**: Similar grouping to K-Means, but reveals hierarchical relationships.
- **DBSCAN**: Detected smaller dense groups and flagged outliers, useful for identifying niche customer segments.

---

## Model Evaluation

- Evaluated using silhouette scores. 
- **K-Means** had the best performance and interpretability, and was selected as the final clustering method.
  
---

## 📜 License

This project is licensed under the MIT License.

---

## ✨ Author

- **Dennis Mecha** – [Reach out via email](mailto:dennismecha4.com)  
  GitHub: [@mechadns](https://github.com/mechadns)

---

> 💡 *Tip: You can extend this project by adding more features (e.g., purchase history), testing other clustering algorithms (e.g., Mean Shift, Birch), or combining clustering with supervised learning for predictive analytics.*

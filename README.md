# Mall Customer Segmentation

This project applies **unsupervised machine learning** techniques to segment customers of a shopping mall based on their spending patterns and demographic details.  
It helps identify distinct customer groups, enabling targeted marketing strategies.

---

## 📌 Project Overview

Customer segmentation is crucial for businesses to:
- Understand customer behavior.
- Improve marketing efficiency.
- Personalize customer experiences.

In this project, we:
1. **Load and explore** mall customer data.
2. **Preprocess** the dataset.
3. **Apply K-Means clustering** to identify customer segments.
4. **Visualize** the clusters for actionable insights.

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

- **Exploratory Data Analysis (EDA)**:
  - Summary statistics
  - Distribution plots
  - Pair plots
- **Clustering**:
  - **K-Means algorithm**
  - Elbow method to determine optimal `k`
- **Visualization**:
  - 2D scatter plots
  - Cluster visualizations with color-coded segments

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

- Identified **distinct customer clusters** based on spending score and income.
- Visualized segments to interpret demographic and behavioral patterns.
- Provided actionable insights for **targeted marketing**.

---

## 📈 Sample Visualization

![Clusters Visualization](images/clusters.png)

---

## 📜 License

This project is licensed under the MIT License.

---

## ✨ Author

- **Your Name** – [your.email@example.com](mailto:your.email@example.com)  
  GitHub: [@yourusername](https://github.com/yourusername)

---

> 💡 *Tip: You can extend this project by testing other clustering algorithms like DBSCAN or hierarchical clustering, or by adding more customer features for deeper segmentation.*

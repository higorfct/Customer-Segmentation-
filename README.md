# Customer Segmentation Project

## 📝 Introduction
This project aims to segment customers based on demographic and behavioral characteristics, enabling more targeted and strategic action from the marketing area.

We used **KMeans Clustering** techniques, preceded by **data standardization and dimensionality reduction with PCA**, to identify **distinct groups of customers** based on variables such as age, income, spending score, and region.

---

## 📊 Data

The data used is contained in the `segmentacao.csv` file and covers the following variables:

- `customer_id` — Unique identifier for each customer  
- `age` — Age  
- `income` — Annual income (in thousands of dollars)  
- `spending_score` — Propensity to consume index (1 to 100)  
- `region` — Geographical region

### Steps performed:
- Analysis of missing values  
- Outlier detection  
- Transformation of categorical variables into dummies  
- Standardization with `StandardScaler`  
- Dimensionality reduction with PCA (retaining 95% of the variance from the original data)  
- Clustering with `KMeans`

---

## 🤖 Modeling with KMeans

Clustering was performed using the **KMeans** algorithm, with input data processed by **PCA**. The optimal number of clusters was determined based on the following metrics:

- **Elbow Method**
- **Silhouette Index**

📌 **Optimal number of clusters**: **4**

Each customer was classified into one of the 4 clusters, allowing the identification of **behavioral patterns and demographic profiles**.

---

## 🔍 Cluster Characteristics

| Cluster | Average Age | Average Income (k$) | Average Spending Score | Behavior                                |
|---------|-------------|---------------------|-----------------------|-----------------------------------------|
| 0       | 25 years    | 30                  | 80                    | Young with high consumption             |
| 1       | 45 years    | 80                  | 40                    | High income, moderate consumption       |
| 2       | 32 years    | 50                  | 20                    | Customers with low engagement           |
| 3       | 60 years    | 40                  | 70                    | Older with recurring consumption        |

---

## 📈 Visualizations

- Distribution charts (histograms and boxplots) to understand variables like `age`, `income`, `spending_score`
- Scatter plot of clusters in the principal components space (PCA)
- **Elbow method** and **silhouette index** plots to define the optimal number of clusters

---

## 🛠️ Tools Used

- **Python** – Main programming language  
- **Pandas** – Data manipulation  
- **Matplotlib / Seaborn** – Visualizations  
- **Scikit-learn** – Preprocessing, PCA, KMeans, metrics  
- **Google Colab** – Development environment

---

## ✅ Results

- Four distinct customer segments were identified.  
- The model enables more targeted marketing actions for specific profiles.  
- Clustering revealed useful patterns of consumption behavior by age group, income, and region.

---

## 🧠 Conclusions

The project demonstrates how clustering can:

- **Identify hidden patterns** in customer databases  
- **Improve marketing strategies** and personalization  
- Support data-driven business decisions

---

## 🔄 Next Steps

- Add behavioral variables (purchase frequency, channels, etc.)  
- Test alternative algorithms such as DBSCAN or Hierarchical Clustering

---

🧑‍💻 **Author & Contact**

Higor Roberto Coutinho Caetano  
**LinkedIn**: [https://www.linkedin.com/in/higor-caetano-049521136/](https://www.linkedin.com/in/higor-caetano-049521136/)  
**Email**: higorfct@gmail.com

# Customer Segmentation using RFM and KMeans

This project applies **RFM (Recency, Frequency, Monetary)** analysis combined with **KMeans clustering** to segment customers based on purchasing behavior. The goal is to identify valuable customer groups to improve marketing strategy, personalization, and business decision-making.

---

## 📌 Project Highlights

- ✅ Cleaned and preprocessed real-world e-commerce data
- ✅ Engineered RFM features from transaction records
- ✅ Removed outliers using the IQR method
- ✅ Standardized features for clustering
- ✅ Applied KMeans algorithm to discover 3 distinct customer segments
- ✅ Visualized clusters by Amount, Frequency, and Recency
- ✅ Model saved using `pickle` for future use

---

## 📂 Files Included

| File Name                  | Description                                      |
|---------------------------|--------------------------------------------------|
| `rfm_kmeans_pipeline.py`  | Main script: RFM creation, clustering, plotting |
| `kmeans_model.pkl`        | Saved clustering model                           |
| `customerSegmentation.csv`| Input dataset                                    |
| `README.md`               | Project documentation                            |

---

## 📊 Techniques Used

- 🧼 Data Cleaning & Transformation (Pandas, NumPy)
- 📊 RFM Feature Engineering
- 🚫 Outlier Removal (IQR method)
- ⚖️ Feature Scaling (StandardScaler)
- 📈 Unsupervised Learning (KMeans)
- 🖼 Data Visualization (Seaborn, Matplotlib)
- 💾 Model Serialization (Pickle)

---

## 📁 Dataset

The dataset contains historical transactions from an e-commerce platform, including:

- `InvoiceNo`: Transaction ID  
- `CustomerID`: Unique customer identifier  
- `InvoiceDate`: Date of purchase  
- `Quantity`, `UnitPrice`: Purchase details  

> This data was parsed and transformed into an RFM matrix for clustering.

---

## 🔍 Clustering Results (Sample Insights)

After applying KMeans with `n_clusters=3`, customers were grouped into:

- **Cluster 0**: High-value customers (high monetary, frequent, recent)
- **Cluster 1**: One-time buyers or dormant users
- **Cluster 2**: Moderate spenders or semi-active users

Each cluster was visualized to compare distributions of key metrics.

---

## 📦 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/customer-segmentation-rfm-kmeans.git
   cd customer-segmentation-rfm-kmeans

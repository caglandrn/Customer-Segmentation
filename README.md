# Customer Segmentation using K-Means Clustering  

 **This project applies the K-Means clustering algorithm to segment customers based on Age, Annual Income, and Spending Score.**  
By analyzing customer behavior, businesses can improve marketing strategies and customer retention.  

---

## 📂 Project Overview  

This project includes:  
 -Data Preprocessing (Scaling, Cleaning)  
 -K-Means Clustering Implementation  
 -Visualizing Customer Segments in 2D & 3D  

---

### Dataset Information  

Source: [Kaggle: Mall Customers Dataset](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)  

**Features:**  

- **CustomerID** → Unique customer identifier  
- **Gender** → Male / Female  
- **Age** → Age of the customer  
- **Annual Income (k$)** → Yearly income in thousands of dollars  
- **Spending Score (1-100)** → Customer spending behavior (1 = Low, 100 = High)  

---

##  Installation  

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```
##  How To Run

1. Clone the repository  
```bash
git clone https://github.com/your-username/customer-segmentation.git
```
```bash
cd customer-segmentation
```

2. Open and run the Jupyter Notebook
```bash
jupyter notebook
```

---

### **Visualizing Customer Segmentation (Raw Markdown)**  

```md
## Visualizing Customer Segmentation
```
### Finding the Optimal K with the Elbow Method  
The optimal number of clusters (`k`) is determined using the **Elbow Method**, which helps minimize the within-cluster sum of squares (WCSS).  

**Key Insight:** The optimal value of `k` is where the "elbow" or sharp bend occurs.  

<p align="center">
  <img src="results/kmeans_elbowmethod.png" width="600">
</p>

---

### Customer Segmentation (2D Scatter Plot)  
After selecting the optimal `k`, we apply **K-Means clustering** and visualize the segments in a **2D scatter plot**.  

**Key Insight:** Customers with similar **Annual Income** and **Spending Score** are grouped into the same cluster.  

<p align="center">
  <img src="results/kmeans_2d_scatter.png" width="600">
</p>

---

### 3D Visualization of Customer Segmentation  
For a more detailed view, we visualize the segmentation in **3D**, considering `Age`, `Annual Income`, and `Spending Score`.  

**Key Insight:** Distinct customer groups can be observed based on income levels and spending behaviors.  

<p align="center">
  <img src="results/kmeans_3d_scatter.png" width="600">
</p>

---

### Cluster-Wise Mean Values (Heatmap)  
To understand each segment’s characteristics, we calculate and visualize the **average Age, Income, and Spending Score for each cluster**.  

**Key Insight:**  
- Some groups have high income but **low spending** (conservative customers).  
- Other groups have **low income but high spending** (younger, impulsive buyers).  

<p align="center">
  <img src="results/kmeans_heatmap.png" width="600">
</p>

---

## Contact  

For any questions or suggestions, feel free to reach out.  

**Email:** [caglandurand@gmail.com]  
**LinkedIn:** [linkedin.com/in/caglanduran]  

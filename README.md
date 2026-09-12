# Customer Segmentation Using K-Means

## 📌 Project Overview

Customer Segmentation Using K-Means is a machine learning project that groups customers into different segments based on their **Annual Income** and **Spending Score**.

The **K-Means Clustering** algorithm is used to identify customers with similar purchasing behavior. This type of segmentation can help businesses understand their customers and develop targeted marketing strategies.

## 🎯 Objective

The main objective of this project is to:

* Analyze customer data.
* Identify different customer groups.
* Determine the optimal number of clusters using the **Elbow Method**.
* Apply the K-Means clustering algorithm.
* Visualize the resulting customer segments.

## 📊 Dataset

The project uses the **Mall Customers Dataset**, which contains information about 200 customers.

### Features

| Feature                | Description                                   |
| ---------------------- | --------------------------------------------- |
| CustomerID             | Unique identification number of each customer |
| Gender                 | Gender of the customer                        |
| Age                    | Age of the customer                           |
| Annual Income (k$)     | Annual income in thousands of dollars         |
| Spending Score (1-100) | Spending score assigned to the customer       |

For clustering, the project uses only:

* **Annual Income (k$)**
* **Spending Score (1-100)**

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* K-Means Clustering

## 🔄 Project Workflow

1. Import the required Python libraries.
2. Load the `Mall_Customers.csv` dataset.
3. Explore the dataset using:

   * `head()`
   * `shape`
   * `info()`
   * Missing-value analysis
4. Extract Annual Income and Spending Score.
5. Determine the optimal number of clusters using the **Elbow Method**.
6. Train the K-Means clustering model.
7. Assign customers to clusters.
8. Visualize the clusters and their centroids.

## 📈 Elbow Method

The Elbow Method is used to determine the appropriate number of clusters.

The **Within-Cluster Sum of Squares (WCSS)** is calculated for different numbers of clusters. Based on the resulting elbow graph, **5 clusters** were selected for this project.

## 🤖 K-Means Clustering

The K-Means algorithm was trained with:

```python
KMeans(
    n_clusters=5,
    init='k-means++',
    random_state=0
)
```

The model divides the customers into **5 distinct groups** based on their annual income and spending score.

## 📊 Results

The final clusters represent different customer segments, such as:

* Customers with lower income and lower spending scores
* Customers with lower income and higher spending scores
* Customers with average income and spending behavior
* Customers with higher income and lower spending scores
* Customers with higher income and higher spending scores

The clusters and their centroids are visualized using a scatter plot.

## 📁 Project Structure

```text
Customer-Segmentation/
│
├── Mall_Customers.csv
├── customer_segmentation.py
├── README.md
└── requirements.txt
```

> Replace `customer_segmentation.py` with the actual name of your Python file if it is different.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Customer-Segmentation.git
```

### 2. Navigate to the project directory

```bash
cd Customer-Segmentation
```

### 3. Install the required libraries

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### 4. Run the Python program

```bash
python customer_segmentation.py
```

## 💡 Conclusion

This project demonstrates how **K-Means clustering** can be used for customer segmentation. By analyzing annual income and spending scores, customers can be divided into meaningful groups that may help businesses understand customer behavior and improve marketing decisions.


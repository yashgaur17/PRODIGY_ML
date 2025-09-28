# Customer Segmentation using K-Means Clustering

## 📌 Project Overview
This project applies *K-Means clustering* to segment customers of a retail store based on their *Annual Income* and *Spending Score*.  
The dataset is taken from [Kaggle – Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).

The goal is to identify distinct customer groups to help businesses target marketing strategies effectively.

---

## 📂 Dataset
- *File:* Mall_Customers.csv
- *Features:*
  - CustomerID – Unique ID
  - Gender – Male/Female
  - Age – Customer age
  - Annual Income (k$) – Income in thousands
  - Spending Score (1–100) – Store-assigned score based on behavior

---

## ⚙ Workflow
1. *Data Preprocessing*  
   - Load dataset, inspect structure, select relevant features.
2. *Elbow Method*  
   - Determine optimal number of clusters.
3. *K-Means Clustering*  
   - Apply clustering on selected features.
4. *Visualization*  
   - Plot clusters and centroids for interpretation.
5. *Insights*  
   - Interpret customer groups (e.g., high income–high spenders, budget customers, etc.).

---

## 📊 Results
- *5 clusters* were identified:
  - High Income, High Spending → Target Customers
  - High Income, Low Spending → Careful Spenders
  - Low Income, High Spending → Impulsive Buyers
  - Low Income, Low Spending → Budget Customers
  - Middle Income, Middle Spending → Average Customers

(Insert your cluster visualization plots here as images or screenshots)

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/customer-segmentation-kmeans.git
   cd customer-segmentation-kmeans
2. Install dependencies:
   `bash
   pip install -r requirements.txt
   `
3. Open the Jupyter Notebook:
   `bash
   jupyter notebook customersegmentationkmeans.ipynb
   `
📦 Project Structure
`
customer-segmentation-kmeans/
├── data/
│   └── Mall_Customers.csv
├── images/
│   └──cluster.png
├── customer_segmentation_kmeans.ipynb
├── requirements.txt
├── README.md

🙋‍♂ Author
Yash  
Aspiring machine learning practitioner and web developer  
Connect with me on LinkedIn or check out my GitHub

🎯 Applications
- Targeted marketing campaigns
- Customer loyalty programs
- Personalized recommendations
- Business strategy optimization
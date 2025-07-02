# Customer Segmentation using K-Means Clustering

## 📌 Project Overview
This project applies **K-Means Clustering** on the **Online Retail dataset** (Kaggle) to group customers based on their purchasing behavior.  
The goal is to identify distinct customer segments that businesses can target with personalized marketing strategies.

---

## 📊 Dataset
- **Source:** [Online Retail Dataset - Kaggle](https://www.kaggle.com/)  
- **File:** `onlineretail.csv`  
- **Description:** The dataset contains transactional data from a UK-based online retail store, including:
  - `InvoiceNo` – Transaction number
  - `StockCode` – Product code
  - `Description` – Product description
  - `Quantity` – Number of items purchased
  - `InvoiceDate` – Date of transaction
  - `UnitPrice` – Price per item
  - `CustomerID` – Unique customer ID
  - `Country` – Customer’s country

---

## ⚙️ Steps Performed
1. **Data Loading & Cleaning**
   - Loaded dataset with proper encoding (`latin1`).
   - Removed missing values (`CustomerID`).
   - Filtered out canceled transactions (negative quantities).

2. **Feature Engineering**
   - Calculated **Total Spending** (`Quantity * UnitPrice`).
   - Aggregated customer-level data: frequency, monetary value, and recency.

3. **Clustering**
   - Selected key features (e.g., Annual Spend, Frequency, Recency).
   - Applied **K-Means** clustering.
   - Determined the optimal number of clusters using the **Elbow Method**.

4. **Visualization**
   - Scatter plots of customer segments.
   - Cluster centroids highlighted.
   - Distribution plots to analyze segments.

---

## 📈 Results
- Customers were grouped into distinct clusters:
  - **High-value frequent buyers**
  - **Low-spend occasional buyers**
  - **Medium-value regular buyers**
- Visualizations help in understanding spending patterns across clusters.

---

## 🖥️ How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/customer-segmentation.git
   cd customer-segmentation

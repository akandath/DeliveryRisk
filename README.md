# Optimizing Delivery Efficiency: KMeans Clustering for Late Deliveries

### Problem Statement
Late deliveries can degrade customer satisfaction, increase costs, and harm a company's reputation. Understanding the patterns and factors that lead to delayed deliveries is essential for improving logistics and enhancing overall service quality.

### Project Description

- **Brief Description:**  
  This project leverages KMeans clustering to analyze orders with late deliveries. By identifying distinct groups within the data, the aim is to uncover underlying factors contributing to delivery delays and provide actionable insights to optimize delivery processes.

- **Relevance:**  
  Timely deliveries are critical for maintaining customer trust and operational efficiency. Analyzing late deliveries helps businesses identify bottlenecks, improve logistics, and enhance customer satisfaction.

  **Data Source(s)**

  DataCO Supply Chain Dataset (Kaggle)['https://www.kaggle.com/datasets/saicharankomati/dataco-supply-chain-dataset']

- **Affected Parties:**
  - **Customers:** Experience delays in receiving their orders, leading to dissatisfaction.
  - **Logistics Teams:** Responsible for managing deliveries and addressing issues causing delays.
  - **Business Stakeholders:** Interested in improving delivery performance and reducing operational costs.

- **Occurrence:**  
  The analysis focuses on orders marked as 'COMPLETE' with a 'Delivery Status' of 'Late delivery'. This subset of data is used to identify patterns and factors associated with delivery delays.

- **Motivation:**  
  The motivation behind this project is to utilize data-driven insights to reduce the incidence of late deliveries, thereby improving customer satisfaction and operational efficiency.

### Dataset Description
The dataset (`data_cleaned.csv`) contains information about orders, including:

- **Categorical Features:**  
  Such as `Order Status`, `Delivery Status`, `Customer City`, `Customer Country`, `Customer Segment`, `Department Name`, `Markete`, `Order City`, `Order Region`, `Order State`, and `Shipping Mode`.
  
- **Numeric Features:**  
  Including `total_lead_time_scheduled`, `total_lead_time_real`, `Benefit per order`, `Days for shipping (real)`, `Order Item Product Price`, `Order Item Profit Ratio`, `Sales per customer`, `Order Item Total`, `Sales`, `order_month`, `shipping_month`, `order_year`, and `shipping_year`.

The dataset has been preprocessed to remove irrelevant columns, handle missing values, and focus on relevant features that contribute to delivery delays.

### Future Scope

- **Clustering Refinement:**  
  Explore different clustering algorithms (e.g., DBSCAN, hierarchical clustering) and validate the optimal number of clusters using additional metrics like silhouette scores.
  
- **Predictive Modeling:**  
  Develop predictive models to forecast the likelihood of a delivery being late based on identified patterns and features.
  
- **Real-Time Monitoring:**  
  Implement the clustering model in a real-time system to continuously monitor and analyze delivery performance.
  
- **Actionable Insights:**  
  Translate cluster characteristics into specific operational strategies to mitigate factors leading to late deliveries.

### Model Evaluation

- **Clustering Approach:**  
  Utilized KMeans clustering to group similar late delivery instances based on preprocessed numeric and categorical features.
  
- **Inertia Analysis:**  
  Calculated the Within-Cluster Sum of Squares (WCSS) for different numbers of clusters (ranging from 2 to 10) to determine the optimal cluster count using the elbow method.
  
- **Cluster Interpretation:**  
  Analyzed cluster centroids by inverse transforming scaled numeric features and decoding one-hot encoded categorical features. This helped in understanding the distinct characteristics of each cluster.
  

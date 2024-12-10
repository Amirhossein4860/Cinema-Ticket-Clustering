# Cinema-Ticket-Clustering
The Cinema Ticket Clustering dataset contains customer purchase information, including attributes like age, ticket type, and time of purchase. It is designed for analyzing customer behavior and segmenting audiences into distinct clusters for targeted marketing and personalized services.

## Overview
This project leverages clustering techniques to analyze cinema ticket sales data. By applying various clustering algorithms, the aim is to uncover hidden patterns and insights that can assist cinema operators, distributors, and other stakeholders in decision-making.

The insights gained from this analysis can improve cinema performance, optimize pricing strategies, enhance customer satisfaction, and help in better resource allocation.

---

## Objectives

**1. Cinema Performance Analysis**
. Group cinemas based on performance metrics such as total sales, tickets sold, and occupancy rates.
. Optimize cinema operations by understanding regional and demographic patterns.

**2. Time-Based Grouping**
. Identify trends influenced by time variables (e.g., month, day of the week).
. Inform marketing and scheduling strategies.

**3. Pricing and Capacity Utilization**
. Cluster cinemas based on ticket pricing, capacity, and usage.
. Adjust ticket prices dynamically for revenue maximization.

**4. Customer Behavior Segmentation**
. Segment based on metrics like showtime preferences and occupancy rates.
. Personalize marketing campaigns and screening schedules.

**5. Outlier Detection**
. Detect abnormal behaviors such as high/low sales or irregular occupancy rates.
. Investigate inefficiencies or anomalies for improvement.

---

## Dataset Description

The dataset consists of cinema ticket sales data, with the following key columns:

. **film_code:** Unique identifier for films.
. **cinema_code:** Unique identifier for cinemas.
. **total_sales:** Total revenue from ticket sales.
. **tickets_sold:** Number of tickets sold.
. **tickets_out:** Reserved but unsold tickets.
. **show_time:** Number of screenings for a given day.
. **occu_perc:** Occupancy percentage of the cinema.
. **ticket_price:** Price of one ticket.
. **ticket_use:** Number of attendees.
. **capacity:** Cinema seating capacity.
. **date:** Screening date.
. **month/quarter/day:** Time features derived from the date.

---


## Data Preprocessing

**1. Data Cleaning**
Handled missing values and outliers.
Removed duplicates for unbiased clustering.

**2. Feature Engineering**
Derived new features such as revenue per seat and occupancy efficiency.

**3. Standardization**
Ensured features are on the same scale for better algorithm performance.

**4. Dimensionality Reduction**
Used PCA to reduce dataset dimensions, retaining critical features.


---


## Clustering Algorithms

**1. K-Means Clustering**

. Efficient for numerical data.
. Explored optimal k using the Silhouette Score and the Elbow Method.

**2. K-Medoids Clustering**

. More robust to outliers compared to K-Means.
. Explored distance metrics (Euclidean, Manhattan) for better performance.

**3. DBSCAN**

. Ideal for identifying outliers and clusters of varying density.
. Tuned eps (neighborhood radius) and min_samples for optimal clustering.

**4. Mean Shift**

. No need to pre-define the number of clusters.
. Dynamically adjusted bandwidth to detect dense regions.

**5. Hierarchical Clustering**

. Visualized cluster hierarchies using dendrograms.
. Determined clusters based on cutting the dendrogram tree.

---


## Visualization

. **Pair Plots:** Explored relationships between key metrics.
. **Box Plots:** Highlighted outliers in features like ticket price and occupancy rates.
. **Correlation Heatmaps:** Identified strong/weak correlations among features.
. **Cluster Scatterplots:** Visualized data clusters and centroids.

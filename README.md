# Customer-Segmentation-Project
## Project Overview
This project aims to segment customers based on their transactional behavior and demographic features using unsupervised machine learning techniques. The goal is to identify customer groups that share similar behaviors and use these segments to develop strategies for offering coupons to increase loyalty and satisfaction.

## Model Approach
### Data Preparation
- Data Loading: Loaded customer and transaction data from an Excel workbook.
- Data Aggregation: Aggregated transactional data to calculate total transactions, claimed and burnt coupons, and recency for each customer.
- Feature Selection: Selected relevant features including demographic (gender, city) and transactional (transaction count, claimed and burnt coupons, recency) data.
- Data Normalization: Normalized the data to ensure all features contribute equally to the clustering process.

### Clustering Algorithm
- Algorithm Used: K-means clustering.
- Number of Clusters: Determined the optimal number of clusters using the Elbow Method and trained the model with 6 clusters.

### Steps
- Load Data: Loaded the Customers and Transactions sheets from the Excel workbook into pandas DataFrames.
- Aggregate Data: Grouped transactions by customer_id and calculated the total number of transactions, the date of the last transaction, and the count of claimed and burnt coupons for each customer.
- Calculate Recency: Calculated the number of days since the last transaction for each customer.
- Merge Data: Merged the aggregated transactional data with the Customers table to include demographic features.
- Select Features: Selected the relevant features for clustering.
- Normalize Data: Normalized the data.
- Train Model: Trained the K-means clustering model with 6 clusters.
- Analyze Segments: Analyzed the characteristics of each segment and made recommendations.

## Evaluation Metrics
- Sum of Squares (SSE): Used to determine the optimal number of clusters.
- Cluster Analysis: Analyzed the mean values of features within each cluster to understand customer behavior.

## Key Findings
### Segment Analysis and Recommendations
#### Segment 0:
- Average Transaction Count: 5.2
- Average Recency (days): 30.5
- Average Claimed Coupons: 3.1
- Average Burnt Coupons: 2.8
-Recommendation: Offer exclusive discounts and loyalty rewards to retain these customers.

#### Segment 1:
- Average Transaction Count: 2.3
- Average Recency (days): 90.2
- Average Claimed Coupons: 1.5
- Average Burnt Coupons: 0.8
- Recommendation: Send reminders and limited-time offers to encourage coupon usage.

#### Segment 2:
- Average Transaction Count: 8.7
- Average Recency (days): 15.4
- Average Claimed Coupons: 6.5
- Average Burnt Coupons: 6.0
- Recommendation: Provide loyalty rewards and personalized recommendations.

#### Segment 3:
- Average Transaction Count: 1.1
- Average Recency (days): 120.7
- Average Claimed Coupons: 0.5
- Average Burnt Coupons: 0.2
- Recommendation: Implement targeted marketing campaigns and special offers to increase activity.

#### Segment 4:
- Average Transaction Count: 4.0
- Average Recency (days): 45.0
- Average Claimed Coupons: 2.0
- Average Burnt Coupons: 1.5
- Recommendation: Offer seasonal promotions and loyalty programs to maintain engagement.

#### Segment 5:
- Average Transaction Count: 6.0
- Average Recency (days): 25.0
- Average Claimed Coupons: 4.0
- Average Burnt Coupons: 3.5
- Recommendation: Provide exclusive access to new products and special events to reward loyalty.

### Conclusion
This project successfully segmented customers into six distinct groups based on their transactional behavior and demographic features. By understanding the characteristics of each segment, we can develop targeted strategies to increase customer loyalty and satisfaction through personalized coupon offers and marketing campaigns.

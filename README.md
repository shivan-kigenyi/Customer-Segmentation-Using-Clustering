# Customer Segmentation Using Clustering

This project uses unsupervised machine learning (clustering) to segment mall customers based on demographic and behavioral data such as age, income, and spending score.

The aim is to uncover distinct customer profiles for better targeting and decision-making.

## Business Objective
To segment customers into distinct groups based on their demographic and behavioral pattern, enabling business to:
- Understand customer diversity
- Identify high-value segments
- Enable smarter marketing and product decisions

Key Research Questions
1. "How can we group similar customers together based on thier behavior and demographics?"
2. "What are the defining features of each customer group(cluster)?"
3. "Which customer segments are high-value(e.g high spenders or loyal customers)?"
4. "How can the business use these segments to improve decision-making?"

## Project workflow
1. Load and explore the dataset
2. Clean and preprocess the data (Handle missing values , fix categorical issues)
3. Perform exploratory data analysis(EDA)
4. Apply K-means Clustering
5. Evaluate and visualize the clusters (2D plot)
6. Interprete the business value of each segment

## Tools and Technologies
Python (Pandas, Matplotlit, numpy, Seaborn, Plotly)
Machine Learning: 'scikit-learn' (kMeans)
Environment: Jupyter Notebook

## Key Finding 
*Research question 1:*
"How can we group similar customers together based on thier behavior and demographics?"

**K-Means Clustering** is applied to group customers using features:
Age - Tells us about the life stage (student, professionals, mature)
Income (k$) - Financial capability
Spending Score - Reflects actual behavior (high vs low spender)

- The **Elbow Method** and silhouette scores suggested **4 clusters** as the optimal choice


*Research question 2:*
"What are the defining features of each customer group(cluster)?"

| Cluster | Segment Name              | Avg Age | Income (k$) | Spending Score  | Description |
|--------:|---------------------------|--------:|------------:|----------------:|-------------|
| 0       | Frugal Mid-Aged           | 38.8    | 41.6        | 33.2            | Older customers with moderate income and low spending habits 
| 1       | Young Big Spenders        | 27.7    | 54.1        | 88.5            | Young customers who spend heavily despite moderate income 
| 2       | Young High Earners, Low Sp| 29.1    | 74.4        | 30.5            | High-income young adults with conservative spending behavior 
| 3       | Affluent Loyal Customers  | 44.6    | 70.6        | 65.6            | Wealthy, older customers with consistent high spending 


*Research Question 3*
"Which customer segments are high-value(e.g high spenders or loyal customers)?"
- **Cluster 1** (Young big Spenders): Higly active spenders; Ideal for trend-driven campaigns
- **Cluster 3** (Affluenct Loyal Customers): High Income + high Spenders; valuable for VIP programs and brand loyalty strategies

*Research Question 4*
"How can the business use these segments to improve decision-making?"
| Segment | Strategy |
|--------:|----------|
| **Young Big Spenders**         | Promote seasonal sales, lifestyle products, and mobile-first campaigns 
| **Affluent Loyal Customers**   | Offer VIP programs, exclusive previews, and premium services 
| **High Earners, Low Spenders** | Encourage spend through personalized offers and exclusive deals 
| **Frugal Mid-Aged**            | Focus on value messaging, loyalty points, and essentials 

## Deliverables
- Cleaned dataset with labled clusters: Segmented_customers.csv'
- Code notebook: 'Analysis.ipynb'
- Visuals folder 
- Project report: 'README.md'


## Author
- Shivan Violet - [LinkedIn](https://www.linkedin.com/in/Shivan-Kigenyi
)


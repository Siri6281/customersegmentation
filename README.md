Customer Segmentation Analysis
Synent Technologies — Data Science Internship | Task 06

Problem Statement:

Retail businesses often struggle to understand their diverse customer base. 
This project aims to segment mall customers into distinct groups based on 
their annual income and spending score using unsupervised machine 
learning — enabling targeted marketing strategies for each segment.

Dataset Details:

Dataset- Mall Customer Segmentation Data 
Source - [Kaggle — Vijay Choudhary](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) 
File - `Mall_Customer.csv` 
Rows - 200 customers 
Features - CustomerID, Gender, Age, Annual Income (k$), Spending Score (1-100) 

Approach :

1. Data Cleaning & Preprocessing
- Checked for missing values — none found
- Removed duplicates — none found
- Renamed columns for clarity
- Encoded Gender column (Male=0, Female=1)
- Scaled features using StandardScaler

2. Exploratory Data Analysis (EDA)
- Gender distribution analysis
- Age, Income and Spending Score distributions
- Correlation heatmap between all features

3. Elbow Method
- Tested K values from 1 to 10
- Plotted inertia vs number of clusters
- Identified **K=5** as the optimal number of clusters

4. K-Means Clustering
- Applied K-Means with K=5
- Clustered based on Annual Income and Spending Score
- Visualized clusters using scatter plot

Results :

5 distinct customer segments were identified:

| Cluster | Segment | Avg Income | Avg Score | Strategy |

1 - High Income, Low Spender | ~87k$ | ~17 | Premium loyalty programs |
2 - High Income, High Spender | ~86k$ | ~82 | Retain with VIP offers |
3 - Average Everything | ~55k$ | ~49 | Seasonal deals |
4 - Low Income, High Spender | ~26k$ | ~79 | EMI & budget deals |
5 - Low Income, Low Spender | ~26k$ | ~20 | Minimal spend |

Tools & Technologies

Language: Python 3
IDE: VS Code + Jupyter Notebook
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
Algorithm: K-Means Clustering
Dashboard: HTML + Chart.js


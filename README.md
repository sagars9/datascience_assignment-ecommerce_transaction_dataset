# Customer Analysis and Recommendation System

This project analyzes customer data, performs customer segmentation, and builds a lookalike recommendation system using various data science techniques.

## Dataset Description

The analysis uses three main CSV files:

1. **Customers.csv**: Contains customer profile information
   - CustomerID
   - CustomerName
   - Region
   - SignupDate

2. **Transactions.csv**: Contains transaction records
   - TransactionID
   - CustomerID
   - ProductID
   - Quantity
   - TotalValue
   - TransactionDate

3. **Products.csv**: Contains product information
   - ProductID
   - ProductName
   - Category
   - Price

## Analysis Components

### 1. Exploratory Data Analysis (SAGAR_SINGH_EDA.ipynb)
- Analyzes sales patterns across different regions and product categories
- Visualizes temporal trends in sales
- Key findings:
  - Electronics (smartwatches and headphones) show strong performance
  - South America leads in sales across categories
  - Seasonal peaks observed in June-September
  - Asia shows high demand for premium clothing

### 2. Customer Segmentation (SAGAR_SINGH_Clustering.ipynb)
- Implements K-means clustering for customer segmentation
- Features used:
  - Customer profile information
  - Transaction history
  - Purchase patterns
- Techniques used:
  - PCA for dimensionality reduction
  - Silhouette score for optimal cluster selection
  - Davies-Bouldin index for cluster validation

### 3. Lookalike Customer Recommendation (SAGAR_SINGH_Lookalike.ipynb)
- Builds a recommendation system to find similar customers
- Methodology:
  - Feature engineering from customer profiles and transaction history
  - Similarity calculation using distance metrics
  - Top-3 similar customers identification
- Output:
  - Generates Lookalike.csv with customer similarity scores

## Technologies Used
- Python
- Pandas for data manipulation
- NumPy for numerical operations
- Scikit-learn for machine learning algorithms
- Seaborn and Matplotlib for visualization

## Key Insights
- Strong regional variations in product preferences
- Clear seasonal patterns in sales
- Distinct customer segments based on purchasing behavior
- Effective identification of similar customers for targeted marketing

## Usage
1. Ensure all required CSV files are in the same directory
2. Run notebooks in the following order:
   - SAGAR_SINGH_EDA.ipynb
   - SAGAR_SINGH_Clustering.ipynb
   - SAGAR_SINGH_Lookalike.ipynb

## Requirements
- Python 3.x
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib

# Online Sales Analysis

**Author**: Yaman Shadid

## Introduction

The objective of this project is to analyze online sales transactions across different product categories to uncover insights related to sales trends, product performance, and regional preferences. The dataset contains transactions involving various product categories such as Electronics, Home Appliances, Clothing, Books, Beauty Products, and Sports. This analysis involves:

- Exploring and visualizing sales trends over time to identify seasonal patterns and growth opportunities.
- Evaluating the popularity and performance of different product categories across regions.
- Investigating the impact of different payment methods on sales volume and revenue.
- Applying machine learning models, such as Decision Tree Classifier and K-Nearest Neighbors (KNN) Regressor, to predict product categories and sales volume.
- Using K-Means clustering to segment customers based on their purchase behavior for targeted marketing strategies.

## Data Collection and Source Selection

The data was obtained from an online sales dataset, chosen for its comprehensive coverage and relevance to the project's objectives. Each row represents a single transaction with columns for order ID, date, product category, product name, quantity sold, unit price, total price, region, and payment method.

## Columns:

Order ID: Unique identifier for each sales order.

Date: Date of the sales transaction.

Category: Broad category of the product sold (e.g., Electronics, Home Appliances, Clothing, Books, Beauty Products, Sports).

Product Name: Specific name or model of the product sold.

Quantity: Number of units of the product sold in the transaction.

Unit Price: Price of one unit of the product.

Total Price: Total revenue generated from the sales transaction (Quantity * Unit Price).

Region: Geographic region where the transaction occurred (e.g., North America, Europe, Asia).

Payment Method: Method used for payment (e.g., Credit Card, PayPal, Debit Card).

## Methods

1. **Data Collection and Source Selection**: The data was obtained from an online sales dataset, chosen for its comprehensive coverage and relevance to the project's objectives.

2. **Data Cleaning**: The dataset was cleaned to handle missing values, outliers, and inconsistencies, ensuring the quality and integrity of the data.

3. **Data Analysis and Visualization**: Exploratory data analysis (EDA) was conducted to understand sales trends, product performance, and regional preferences. Visualizations were created to present key insights.

4. **Machine Learning Models**:
    - **Decision Tree Classifier**: Used to predict the product category based on features like region, payment method, unit price, and quantity sold.
    - **K-Nearest Neighbors (KNN) Regressor**: Used to predict the sales volume (units sold) based on features like region, product category, payment method, and unit price.
    - **K-Means Clustering**: Applied to segment customers based on their purchase behavior.

## Key Visuals

**1. Monthly Sales Trends**

![Monthly Sales Trends](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Monthly%20Sales%20Trends.png)

This plot displays the monthly sales trends, revealing that sales peak in January and have a downward trend from April onwards. This indicates potential seasonality and suggests focusing marketing efforts in early months.

**2. Quarterly Sales Trends**

![Quarterly Sales Trends](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Quarterly%20Sales%20Trend.png)

This plot shows that the first quarter has the highest sales, followed by a decline in the second and third quarters. This seasonal trend can help in planning inventory and promotions.

**3. Revenue by Product Category**

![Revenue by Product Category](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Revenue%20by%20Product%20Category.png)

Electronics generate the highest revenue, followed by home appliances and sports. This insight can guide where to focus marketing and inventory resources.

**4. Sales by Product Category and Region**

![Sales by Product Category and Region](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Sales%20by%20Product%20Category%20and%20Region.png)

North America leads in electronics sales, while Europe has a significant share in home appliances. This helps tailor regional marketing strategies and stock allocation.

**5. Sales Volume and Revenue by Payment Method**

![Sales Volume and Revenue by Payment Method](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Sales%20Volume%20and%20Revenue%20by%20Payment%20Method.png)

Credit cards are the most popular payment method both in terms of sales volume and revenue, indicating that promotions for credit card payments might be effective.

**6. Average Order Value by Payment Method**

![Average Order Value by Payment Method](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Average%20Order%20Value%20by%20Payment%20Method.png)

Credit cards also lead in the average order value, suggesting that customers are likely to spend more per transaction when using credit cards.

**7. Correlation Matrix Heatmap**

![Correlation Matrix Heatmap](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Correlation%20Matrix%20Heatmap.png)

There is a strong positive correlation between unit price and total revenue, indicating that higher-priced items significantly contribute to overall sales.

**8. Boxplot of Units Sold**

![Boxplot of Units Sold](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Boxplot%20of%20Units%20Sold.png)

Most transactions involve selling 1 to 3 units, with a few outliers selling up to 10 units. This helps in understanding the typical sales volume per transaction.

**9. Histogram of Unit Price**

![Histogram of Unit Price](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Histogram%20of%20Unit%20Price.png)

Most products are priced under $500, with a long tail of high-priced items. This distribution can inform pricing strategies and inventory management.

**10. Confusion Matrix for Decision Tree Classifier**

![Confusion Matrix for Decision Tree Classifier](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Confusion%20Matrix%20for%20Decision%20Tree%20Classifier.png)

The model accurately predicts most categories, with some confusion between similar categories like electronics and home appliances. Overall, it performs well in classification.

**11. Actual vs. Predicted Values for KNN Regressor**

![Actual vs. Predicted Values for KNN Regressor](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Actual%20vs.%20Predicted%20Values%20for%20KNN%20Regressor.png)

The scatter plot indicates that the KNN regressor predicts the sales volume reasonably well but with some variance, suggesting room for improvement.

**12. Elbow Method for Optimal Number of Clusters**

![Elbow Method for Optimal Number of Clusters](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Elbow%20Method%20for%20Optimal%20Number%20of%20Clusters.png)

The optimal number of clusters is determined to be 3, as indicated by the elbow point in the plot. This helps in effective customer segmentation.

**13. Customer Segmentation based on K-Means Clustering**

![Customer Segmentation based on K-Means Clustering](https://github.com/Yaman-Shadid/Online-Sales/blob/main/Visuals/Customer%20Segmentation%20based%20on%20K-Means%20Clustering.png)

Customers are segmented into three clusters based on total revenue and units sold, providing a basis for targeted marketing strategies.

## Models

**Decision Tree Classifier**: Achieved an accuracy of 95.83% in predicting product categories. The confusion matrix and classification report provide detailed insights into the model's performance.

**K-Nearest Neighbors (KNN) Regressor**: Achieved a Mean Squared Error of 0.812 and an R^2 Score of 0.216 in predicting sales volume. The scatter plot of actual vs. predicted values helps evaluate the model's accuracy.

**K-Means Clustering**: The elbow method was used to determine the optimal number of clusters, and the clustering results were visualized to segment customers based on their purchase behavior.

Although I did not use the models for all visualizations, I did visualize the models themselves to see how it would affect the data itself, and what kind of answers I could get.

## Recommendations

To determine the practical value of the model accuracy, stakeholders should evaluate the specific context of their application, understanding the trade-offs between precision, recall, and accuracy. Depending on the stakeholders' objectives, model parameters may need to be adjusted, or different algorithms may need to be chosen to optimize these metrics. It is advisable to work closely with domain experts to make informed decisions about model performance, especially when dealing with binary outcomes in scenarios with varying costs and class imbalances.

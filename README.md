# Customer Segmentation using RFM Analysis with PySpark

This project performs customer segmentation using RFM (Recency, Frequency, Monetary) analysis on an e-commerce dataset. The implementation uses Apache Spark with Python (PySpark) in a Jupyter Notebook environment.

## Project Overview

The goal of this project is to identify distinct customer groups based on their purchasing behavior. By segmenting customers, businesses can tailor marketing strategies, improve customer retention, and enhance personalization efforts. The RFM model is a widely used technique for this purpose.

**Key steps involved:**
1.  **Data Loading and Cleaning:** Ingesting the raw transaction data and performing necessary preprocessing steps.
2.  **RFM Feature Engineering:** Calculating Recency, Frequency, and Monetary values for each customer.
3.  **RFM Scoring:** Assigning scores to customers based on their RFM values.
4.  **Customer Segmentation:** Grouping customers into meaningful segments (e.g., Champions, Loyal Customers, At Risk) based on their combined RFM scores.
5.  **Output Generation:** Saving the cleaned dataset and the final RFM segmentation results for further analysis.

## Dataset

The dataset used is an e-commerce transactions dataset containing the following columns:

*   `InvoiceNo`: Invoice number. A 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'C', it indicates a cancellation.
*   `StockCode`: Product (item) code. A 5-digit integral number uniquely assigned to each distinct product.
*   `Description`: Product (item) name.
*   `Quantity`: The quantities of each product (item) per transaction.
*   `InvoiceDate`: Invoice Date and time. The day and time when each transaction was generated.
*   `UnitPrice`: Unit price. Product price per unit in sterling.
*   `CustomerID`: Customer number. A 5-digit integral number uniquely assigned to each customer.
*   `Country`: Country name. The name of the country where each customer resides.

*(You can add a link to the dataset source if it's publicly available, e.g., "Dataset sourced from UCI Machine Learning Repository: [Online Retail Dataset](link-to-dataset)")*

## Technologies Used

*   **Python 3.x**
*   **Apache Spark (PySpark)**: For distributed data processing and analysis.
*   **Jupyter Notebook / JupyterLab**: For interactive development and presentation.
*   **Pandas**: Primarily for data manipulation when saving/loading CSV files to/from the local filesystem.

## Project Structure
├── customer_segment.ipynb # Jupyter Notebook for data cleaning, RFM calculation, and segmentation.

├── analysis_notebook.ipynb # (Placeholder) Jupyter Notebook for further analysis of the results.

├── data/ # (Optional) Directory for raw input data.

│ └── online_retail.csv # Example raw data file name

│ └── cleaned_data.csv # Output: Cleaned transaction data.

│ └── rfm_df.csv # Output: RFM scores and customer segments.

└── README.md # This file.


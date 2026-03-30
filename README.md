# Data Preprocessing and Feature Engineering Project[cite: 1]

## Overview
This project demonstrates a foundational workflow for data acquisition, cleaning, exploratory data analysis (EDA), and automated data profiling using Python[cite: 1]. It utilizes customer data containing attributes like CustomerID, Name, Age, Gender, Income, Purchases, and Churn[cite: 1].

## Prerequisites
To run this notebook successfully, ensure you are using Python 3.13 (the notebook was built using Python 3.13.5)[cite: 1] and have the following libraries installed:
*   `pandas`[cite: 1]
*   `matplotlib`[cite: 1]
*   `seaborn`[cite: 1]
*   `ydata-profiling`[cite: 1]
*   `setuptools` (Required for Python 3.12+ to avoid missing package errors)

## Project Workflow

### 1. Data Acquisition (Part B)[cite: 1]
The project starts by loading data from multiple file formats:
*   **CSV & JSON:** Reads `customer_data.csv` and `customer_data.json` into pandas DataFrames[cite: 1].
*   **SQL:** Reads a SQL script (`customer_data.sql`) containing schema creation and data insertion commands[cite: 1].

### 2. Data Understanding & Cleaning (Part C)[cite: 1]
Initial data inspection and cleaning steps include:
*   Displaying the first few rows, dataframe info, statistical summaries, and null value counts[cite: 1].
*   Removing duplicate records using `drop_duplicates()`[cite: 1].
*   Handling missing data by filling empty numeric values with the column mean (`fillna(df.mean(numeric_only=True))`)[cite: 1].

### 3. Exploratory Data Analysis (Part D)[cite: 1]
Visualizing the cleaned data to find patterns and relationships:
*   **Histogram:** Visualizes the "Age Distribution" of customers[cite: 1].
*   **Scatter Plot:** Compares "Income" versus "Purchases"[cite: 1].
*   **Correlation Heatmap:** Attempts to plot a heatmap of feature correlations using Seaborn[cite: 1].

### 4. Data Profiling (Part E)[cite: 1]
Automated exploratory data analysis using `ydata_profiling`:
*   Generates a comprehensive `ProfileReport`[cite: 1].
*   Exports the interactive report to an external HTML file named `report.html`[cite: 1].

---

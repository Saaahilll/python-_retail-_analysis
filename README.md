# Synthetic Online Retail Data Analysis

## Objective

This Jupyter Notebook analyzes a synthetic online retail dataset to understand customer behavior, sales patterns, and key factors influencing sales performance. The analysis includes data loading, cleaning, exploration, and visualization to derive meaningful insights.

## Data Source

The dataset is a CSV file named `synthetic_online_retail_data_1.csv` containing synthetic data for an online retail store. It includes information on customer demographics, order details, product information, and reviews.

## Notebook Overview

The notebook is structured into the following sections:

### 1. Importing Libraries

*   **Description:** Imports necessary Python libraries such as `numpy`, `pandas`, `matplotlib`, and `seaborn`.
*   **Purpose:** These libraries are used for data manipulation, numerical calculations, data visualization, and statistical analysis.
*   **Code:**

    ```
    import numpy as np
    import pandas as pd
    import matplotlib.pyplot as plt
    %matplotlib inline
    import seaborn as sns
    ```

### 2. Loading the Data

*   **Description:** Reads the CSV file into a pandas DataFrame.
*   **Purpose:** To load the dataset for further analysis.
*   **Code:**

    ```
    df = pd.read_csv(r'C:\\Users\\LENOVO\\Documents\\New folder\\synthetic_online_retail_data_1.csv', encoding= 'unicode_escape')
    ```

### 3. Data Inspection

*   **Description:** Displays the shape of the DataFrame (number of rows and columns).
*   **Purpose:** Provides an overview of the dataset's size.
*   **Code:**

    ```
    df.shape #shows no of columns and rows in the file
    ```

*   **Description:** Shows the first few rows of the DataFrame.
*   **Purpose:** To understand the structure and content of the data.
*   **Output:** Displays the first 10 rows with columns such as `customer_id`, `order_date`, `product_id`, `category_id`, `category_name`, `product_name`, `quantity`, `price`, `payment_method`, `city`, `review_score`, `gender`, `age`, and `age_bracket`.

### 4. Data Cleaning

*   **Description:** Checks for missing values in the dataset.
*   **Purpose:** To identify and handle missing data that could affect the analysis.
*   **Code:** `df.isnull()`

### 5. Data Description

*   **Description:** Generates descriptive statistics for numerical columns in the DataFrame.
*   **Purpose:** Provides key statistical measures such as mean, median, standard deviation, and quartiles.
*   **Output:** Displays statistics for columns like `customer_id`, `product_id`, `category_id`, `quantity`, `price`, `review_score`, and `age`.

### 6. Gender-Based Analysis

*   **Description:** Calculates the sum of prices for each gender.
*   **Purpose:** To compare sales distribution between genders.
*   **Output:** Shows the total price for each gender category (Male, Female, Others).

## How to Use This Notebook

1.  **Environment Setup:**
    *   Ensure you have Python installed.
    *   Install the necessary libraries by running `pip install numpy pandas matplotlib seaborn`.
2.  **Data Loading:**
    *   Place the `synthetic_online_retail_data_1.csv` file in the appropriate directory.
    *   Update the file path in the `pd.read_csv()` function if necessary.
3.  **Execution:**
    *   Run the notebook cell by cell to reproduce the analysis.
    *   Modify the code to explore additional aspects of the dataset.

## Key Insights

*   The dataset contains 1000 rows and 14 columns representing various aspects of online retail transactions.
*   Descriptive statistics provide a quick overview of numerical features, such as the distribution of prices and customer ages.
*   The notebook serves as a starting point for further analysis and visualization of the synthetic online retail data.

## Further Analysis

Future steps could include:

*   Visualizing sales trends over time.
*   Analyzing customer demographics and their purchasing behavior.
*   Exploring the relationship between review scores and sales.
*   Building predictive models for sales forecasting.

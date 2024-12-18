
# Brazilian E-Commerce Analysis: Insights into Marketplace Trends with Python and Power BI

![E-Commerce Report](/assets/img/olist_e-commerce_teaser.gif)

## Table of Contents

- [Introduction](#introduction)
- [Project Objectives](#project-objectives)
- [Project Structure](#project-structure)
- [Data Source](#data-source)
- [Getting Started](#getting-started)
- [Python Analysis](#python-analysis)
- [Power BI Report](#power-bi-report)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)
- [Authors](#authors)


## Introduction

This project combines the analytical capabilities of Python and Power BI to explore around 100,000 orders from the Brazilian e-commerce marketplace Olist. By leveraging Python for data preprocessing and Power BI for visualization, the project provides a comprehensive view of marketplace performance, including customer behavior, delivery performance, and sales trends.


## Project Objectives

- Preprocess raw e-commerce data using Python.
- Identify sales and delivery performance, regional differences, customer preferences and sales trends.
- Derive actionable insights for improving marketplace strategies.
- Visualize key trends and insights with Power BI.


## Project Structure

```
brazilian-ecommerce-analysis/
│
├── assets/                     # Images, GIFs, and other media
├── datasets/                   # Raw and cleaned datasets
├── notebooks/                  # Jupyter notebook
├── power_bi_report/            # Power BI report file 
├── README.md                   # Project overview and instructions
└── LICENSE                     # License information
```


## Data Source

The dataset used in this project is the **Brazilian E-Commerce Public Dataset by Olist**, sourced from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce). Olist is Brazil's largest online marketplace for small and medium-sized businesses (SMBs). This dataset includes real, anonymized commercial data from approximately 100,000 orders. It provides a comprehensive view of the ecommerce process, covering multiple dimensions of customer and sales data. 

The dataset includes the following key components:
- **Orders**: Details of orders, including timestamps, statuses, and performance metrics like freight costs and delivery times.
- **Customers**: Metadata about customers, such as locations and anonymized identifiers.
- **Products**: Information about products, including categories, dimensions, and weights.
- **Reviews**: Customer satisfaction data, including review scores and optional written comments.
- **Payments**: Data on payment methods, amounts, and installment plans.
- **Geolocation**: Latitude and longitude mappings of Brazilian zip codes.

### Context
This dataset was generously provided by Olist and André Sionek in 2018. Olist operates as a platform connecting SMBs across Brazil with multiple marketplaces. Merchants use Olist’s logistics partners to fulfill orders, enabling them to sell their products hassle-free. Customer satisfaction surveys, conducted after delivery or on the estimated delivery date, capture customer feedback on their purchase experience.

### Citation
Olist, and André Sionek. (2018). Brazilian E-Commerce Public Dataset by Olist [Data set]. Kaggle. [https://doi.org/10.34740/KAGGLE/DSV/195341](https://doi.org/10.34740/KAGGLE/DSV/195341)



## Getting Started

### Prerequisites

To run this project locally, ensure you have the following installed:
- Python 3.x
- Jupyter Notebook
- Power BI Desktop
- Python libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `unidecode`, `re`

### Usage

1. Clone the repository
2. Open the Power BI `.pbix` file in Power BI Desktop for interactive analysis.


## Python Analysis

Key tasks performed in Python include:

- **Data Exploration**: Initial examination of dataset structures, schema visualization, and summary statistics.
- **Data Cleaning**: Addressing missing values, removing duplicates, correcting data types, and handling outliers to ensure data quality and consistency.
- **Data Validation**: Standardizing city names, verifying state abbreviations, mapping state names, and cleaning geolocation data.
- **Feature Engineering**: Adding new columns, such as delivery duration, late delivery flags, and approval times, to enhance analysis capabilities.
- **Data Translation**: Translating product categories from Portuguese to English for consistency and readability.
- **Key Integrity Checks**: Ensuring relational integrity between datasets by verifying and resolving missing or invalid foreign key references.


### Running Python Scripts

1.  Navigate to the `notebooks/` directory
2. Open the Jupyter Notebook: `ecommerce_analysis.ipynb`



## Power BI Report

The Power BI report includes the following pages:

1. **Overview**:
    - High-level metrics: total orders, revenue, average review scores, and sales trends.
    - Customer insights: locations, spending patterns, and repeat purchase rates.
    - Seller insights: locations, order distribution over time, and delivery delays.

2. **Orders**:
    - Order metrics: delivery delays by state and overall trends.
    - Time-based slicing: order data analyzed by year, quarter, and month.

3. **Products**:
    - Sales performance: product-level metrics, top categories, and revenue trends.
    - Time-based slicing: sales trends analyzed by year, quarter, and month.
    - Product details: comprehensive list of products, including dimensions, price ranges, and categories.

4. **Insights**:
    - Delivery performance: analysis of delivery duration and freight costs.
    - Customer experience: review score trends and key influencer analysis.
    - Regional differences: variations in product and sales metrics by region.

5. **Q&A**:
    - Interactive insights: ability to ask questions and generate on-demand visualizations based on the dataset.


## Dependencies

This project requires the following Python libraries:

-   `pandas`
-   `numpy`
-   `matplotlib`
-   `seaborn`
-   `unidecode`
-   `re`

Additional tools:

-   Power BI Desktop for `.pbix` report files.


## Contributing

Contributions are welcome! Fork the repository, make enhancements, and submit a pull request.


## License

This project is licensed under the [MIT License](LICENSE).


## Authors

- [Jan Dokoupil](https://github.com/jdok8)

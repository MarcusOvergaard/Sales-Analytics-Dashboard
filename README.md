# Sales Analytics Dashboard: End-to-End E-Commerce Business Intelligence with SQL and Power BI

## Project Overview

This project transforms the Olist Brazilian E-Commerce dataset into a PostgreSQL star schema and an interactive Power BI dashboard for sales analysis.

## Skills Demonstrated

- PostgreSQL
- SQL
- Power BI
- Star schema design
- Data validation
- Dashboard development

## Business Problem

How can an e-commerce marketplace better understand its sales performance?

- How is revenue changing over time?
- Which regions drive the most sales?
- Which product categories and products generate the most revenue?
- Which customers and sellers contribute most to order activity?
- Where are delivery delays or review-score problems likely to appear?

## Dataset

- Source: Olist Brazilian E-Commerce Public Dataset (Kaggle)
- Raw data: `data/raw/`
- Main tables: customers, orders, order_items, payments, reviews, products, sellers, and geolocation.

## Data Model

Fact Table

- fact_order_items

Dimensions

- dim_customer
- dim_product
- dim_seller
- dim_date

Grain

One row per order item.

## Dashboard

![Executive Overview](powerbi/screenshots/executive_overview.png)

The dashboard summarizes revenue, orders, average order value, top categories, top sellers, and sales by state with interactive filters.

## Key Findings

- Revenue is concentrated in a small number of product categories.
- Sales performance varies significantly across Brazilian states.
- A limited number of sellers contribute a disproportionate share of revenue.
- Monthly revenue trends reveal seasonality and growth patterns.

## Limitations

- The dataset represents a single Brazilian e-commerce marketplace.
- Customer demographics are not available.
- Product-level profitability cannot be analyzed because cost data is unavailable.
- The project focuses on sales performance and does not include advanced forecasting or predictive analytics.

## Future Improvements

- Incorporate payment and review fact tables into the dimensional model.
- Add delivery performance and customer satisfaction reporting.
- Create additional dashboard pages for seller performance and operations.
- Implement trend forecasting and anomaly detection.
- Deploy the dashboard using the Power BI Service.

## License

This project is licensed under the MIT License.

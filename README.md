# Madhav E-Commerce Sales Analysis Dashboard

An interactive Power BI dashboard for exploring e-commerce sales, profit, product mix, customer activity, payment methods, and geographic performance.

## Project overview

This project combines two CSV tables:
- **Orders**: order date, customer, state, and city (500 orders).
- **Details**: order-level product line items, amount, profit, quantity, category, sub-category, and payment mode (1,500 rows).

The tables are linked through `Order ID`. The Orders table has one row per order, while Details contains multiple product line items per order.

## Tools and techniques

- Microsoft Power BI
- DAX measures
- Power Query / CSV data import
- Data modelling and relationships
- KPI cards, bar charts, donut charts, and slicers

## Dashboard highlights

- State-wise sales analysis
- Quantity distribution by product category
- Profit by product sub-category
- Customer-level sales comparison
- Payment-mode distribution
- Profit trend by order date
- State slicer for interactive filtering

## Key figures from the supplied dataset

| Metric | Value |
|---|---:|
| Sales amount | 437,771 |
| Profit | 36,963 |
| Quantity sold | 5,615 |
| Distinct orders | 500 |
| Order detail rows | 1,500 |

The figures above are calculated directly from the supplied CSV files. They may appear rounded in the Power BI report.

## Data model

`Orders[Order ID]` is the unique order key and relates to `Details[Order ID]` as a one-to-many relationship. Use the Orders table for order/customer/geography/date attributes and Details for product and financial line-item metrics.

## Repository structure

```text
Madhav-Ecommerce-Sales-Analysis/
├── Dataset/
│   ├── Orders.csv
│   └── Details.csv
├── Dashboard/
│   └── Madhav_Ecommerce_Sales_Dashboard.pbix
├── Screenshots/
│   └── dashboard.png
└── README.md
```

## Dashboard preview

![Madhav E-Commerce Sales Dashboard](Screenshots/dashboard.png)

## How to use

1. Clone or download this repository.
2. Open `Dashboard/Madhav_Ecommerce_Sales_Dashboard.pbix` in Power BI Desktop.
3. If Power BI requests the source files, point the data sources to the CSV files in `Dataset/`.
4. Refresh the data to load the model.

## Author

**Ranvijay Singh**

- GitHub: https://github.com/ranvijaysinghln834-ctrl
- LinkedIn: https://www.linkedin.com/in/ranvijay-singh-24911b331/

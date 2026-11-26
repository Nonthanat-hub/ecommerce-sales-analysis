# Data Dictionary: Online Retail II

## 1. Dataset Overview

- Dataset: Online Retail II
- Source: UCI Machine Learning Repository
- Data Type: E-commerce transaction records
- Period: December 2009 – December 2011

## 2. Data Fields

| Column | Description | Data Type |
|---|---|---|
| Invoice | Invoice number identifying a transaction | String |
| StockCode | Unique product code | String |
| Description | Product name or description | String |
| Quantity | Number of products purchased | Integer |
| InvoiceDate | Date and time of transaction | Datetime |
| Price | Unit price of a product | Decimal |
| Customer ID | Unique customer identifier | String |
| Country | Customer's country | String |

## 3. Important Data Considerations

- Missing Customer ID values may exist.
- Negative Quantity values may represent cancellations or returns.
- Invoice numbers beginning with "C" indicate cancellations.
- Duplicate records should be investigated before removal.
- Revenue can be calculated as Quantity multiplied by Price.

## 4. Planned Derived Fields

| Field | Calculation | Purpose |
|---|---|---|
| Revenue | Quantity × Price | Sales analysis |
| Year | Extract from InvoiceDate | Yearly trends |
| Month | Extract from InvoiceDate | Monthly trends |
| Order Value | Sum of Revenue per Invoice | Order analysis |

## 5. Data Quality Checks

- Check missing values.
- Check duplicate records.
- Validate data types.
- Investigate negative quantities and prices.
- Check unusual transaction values.

## 6. Notes

Column definitions and data quality assumptions will be verified against the downloaded dataset before analysis.


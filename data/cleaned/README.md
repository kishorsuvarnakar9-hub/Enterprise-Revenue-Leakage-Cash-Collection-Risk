# Cleaned & Analytical Data

## Overview

This folder contains the cleaned and analysis-ready datasets
prepared for SQL, Python and Power BI analysis.

The data preparation process includes:

- Data type standardization
- Missing value validation
- Duplicate validation
- Date validation
- Referential integrity checks
- Payment aggregation
- Financial metric validation
- Revenue leakage validation
- Analytical transformations

## Data Preparation Flow

Raw Data
   ↓
Data Quality Checks
   ↓
Data Cleaning
   ↓
Data Transformation
   ↓
Analytical Dataset
   ↓
SQL / Python / Power BI

## Main Analytical Data

The cleaned analytical layer contains information required for:

### Revenue Analysis
- Invoice Amount
- Net Receivable
- Revenue

### Payment Analysis
- Total Paid
- Payment Count
- First Payment Date
- Final Payment Date
- Outstanding Amount

### Revenue Leakage
- Price Leakage
- Volume Leakage
- Discount Leakage
- Total Leakage
- Leakage Flag

### Collection Risk
- Outstanding Amount
- Days Past Due
- Aging Bucket
- Payment Status
- Risk Rating

### Customer Analysis
- Customer
- Industry
- Region
- Customer Segment
- Credit Score
- Risk Rating

## Analytical View

The main invoice-level analytical view used in the project is:

`vw_invoice_financial`

This view combines invoice information with aggregated payment
information to create an invoice-level financial dataset.

## Quality Checks

The cleaned data was validated for:

- Duplicate records
- Missing values
- Invalid dates
- Invalid customer references
- Invalid contract references
- Negative financial values
- Payment aggregation consistency

## Usage

The cleaned analytical data is used by:

- PostgreSQL / SQL
- Python / Pandas
- Power BI
- Business KPI analysis

# Sales Data Analysis – Power BI

## Project Overview
An interactive sales dashboard built using Power BI to analyze 2025 sales data.

## Dataset
- 1,000 records
- Sales data including orders, products, categories, regions, quantities, and payment methods.

## DAX Measures

**Total Sales**
```DAX
Total Sales = SUM('Sales Data'[Sales (SAR)])
```

**Total Orders**
```DAX
Total Orders = DISTINCTCOUNT('Sales Data'[Order ID])
```

**Total Quantity**
```DAX
Total Quantity = SUM('Sales Data'[Quantity])
```

**Average Order Value**
```DAX
Average Order Value =
DIVIDE(
    SUM('Sales Data'[Sales (SAR)]),
    DISTINCTCOUNT('Sales Data'[Order ID])
)
```

## Dashboard Visualizations
- Sales by Region
- Sales by Category
- Sales by Product
- Sales by Month
- Sales by Payment Method

## Interactive Filters
- Region
- Category
- Order Date

## Tools
- Microsoft Power BI
- DAX

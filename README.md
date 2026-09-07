# Shipment & Delivery Performance KPI Analysis

## Project Overview

I worked on this project to understand how well shipments are being delivered and where the main delivery problems are.

The analysis focuses on On-Time Delivery, In-Full delivery, OTIF performance, delivery delays, and carrier performance.

I used Excel to clean and analyze the shipment data, calculate the KPIs, and create a dashboard to present the results.

## Business Problem

The main question I wanted to answer was:

**Why is the overall OTIF performance low?**

Instead of looking only at the overall OTIF percentage, I broke the shipments into different categories to understand whether the problem was caused by late delivery, incomplete shipments, or both.

I also compared different carriers to see whether some carriers were performing better or worse than others.

## Dataset

The dataset contains shipment-level information such as:

- Shipment ID
- Order ID
- Supplier ID
- Ship Date
- Promised Delivery Date
- Actual Delivery Date
- Carrier
- Quantity Ordered
- Quantity Shipped
- Lead Time
- Delay
- On-Time indicator
- In-Full indicator
- OTIF indicator

**Analysis Period:** 09-Jan-2025 to 15-Jan-2026

**Total Shipments:** 2,429

## KPIs Analyzed

| KPI | Result |
|---|---:|
| Total Shipments | 2,429 |
| On-Time Delivery | 23% |
| In-Full | 82% |
| OTIF | 20% |
| Average Lead Time | 10.42 days |
| Average Delay | 6.92 days |

## OTIF Analysis

I divided the shipments into four categories to understand the reason behind the low OTIF performance.

| Category | Shipments |
|---|---:|
| OTIF | 475 |
| Late + In-Full | 1,506 |
| On-Time + Not In-Full | 90 |
| Late + Not In-Full | 358 |

The biggest finding from this analysis was the **Late + In-Full** category.

There were **1,506 shipments** that were fulfilled in full but delivered late.

This showed me that the major problem is related to **delivery timeliness**, rather than only quantity fulfillment.

## Carrier Analysis

I compared the five carriers in the dataset based on their On-Time %, OTIF %, and Average Delay.

| Carrier | Shipments | On-Time % | OTIF % | Avg Delay |
|---|---:|---:|---:|---:|
| DHL | 511 | 24% | 21% | 5.14 |
| FedEx | 446 | 24% | 20% | 4.50 |
| Ekart | 475 | 23% | 20% | 4.65 |
| BlueDart | 496 | 25% | 20% | 4.76 |
| Delhivery | 501 | 20% | 18% | 5.19 |

Delhivery had the **lowest OTIF percentage (18%)** and the **highest average delay (5.19 days)** among the carriers.

I treated this as an area that needs further investigation rather than directly concluding that the carrier is responsible for all delays.

## Dashboard

I created an Excel dashboard to make the results easier to understand.

The dashboard includes:

- Total Shipments
- On-Time Delivery %
- In-Full %
- OTIF %
- Average Lead Time
- Average Delay
- On-Time vs Late Shipments
- OTIF Performance
- Average Delay by Carrier
- Key Business Insights
- Business Recommendations

## Key Findings

- Only **23% of shipments were delivered on time**.
- **In-Full performance was 82%**, which was much better than On-Time performance.
- Overall **OTIF was around 20%**.
- **Late + In-Full** was the largest OTIF failure category with 1,506 shipments.
- Delhivery had the lowest OTIF and highest average delay among the five carriers.
- Delivery timeliness appears to be the main area that needs improvement.

## Business Recommendations

Based on the analysis, I would recommend:

1. Focus on reducing late deliveries.
2. Investigate the reasons behind the large number of Late + In-Full shipments.
3. Review Delhivery's delivery performance in more detail.
4. Look for ways to reduce overall lead time.
5. Track carrier performance regularly using OTIF, On-Time %, and Average Delay.

## Tools Used

- Microsoft Excel
- Excel formulas
- Pivot tables / analysis tables
- Charts
- KPI Dashboard

## Project Structure

```text
Shipment-Delivery-Performance-Analysis/
│
├── Shipment_Delivery_KPI_Analysis.xlsx
├── Project_Report.pdf
├── README.md
└── screenshots/
    └── KPI_Dashboard.png

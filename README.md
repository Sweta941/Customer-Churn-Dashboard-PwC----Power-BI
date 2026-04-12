# 📊 Customer Churn Dashboard — Power BI

A two-page interactive Power BI dashboard designed to monitor customer churn risk, analyze service usage patterns, and identify key drivers of customer attrition.

---

## 📁 File

| File | Description |
|------|-------------|
| `Customer_Churn_Dashboard.pbix` | Main Power BI report file |

> **Power BI Desktop version required:** 2.123.424.0 or later (November 2023 release)

---

## 🗂️ Dashboard Pages

### Page 1 — Customer Overview

Provides a high-level snapshot of the customer base and their service subscriptions.

**KPI Cards**
- Customers at Risk
- Total Monthly Charges
- Total Yearly Charges
- No. of Tech Support Tickets
- No. of Admin Tickets

**Demographics & Profile**
- % Senior Citizens
- % Customers with a Partner
- % Customers with Dependents
- Gender distribution (Donut Chart)

**Subscription & Billing**
- Subscription Time / Tenure in Years (Bar Chart)
- Types of Contract (Bar Chart)
- Payment Method breakdown (Bar Chart)
- Paperless Billing adoption (Donut Chart)
- Internet Service type (Donut Chart)
- Multiple Lines: % Yes vs % No (Cards)

**Add-on Services (Multi-Row Cards)**
- % Phone Service
- % Online Security
- % Online Backup
- % Device Protection
- % Tech Support
- % Streaming TV
- % Streaming Movies

---

### Page 2 — Churn Analysis

Deep-dive into churn metrics with interactive slicers for focused analysis.

**Slicers (Filters)**
- Internet Service type
- Risk of Churn
- Months Subscribed (Tenure)
- Contract Type

**KPI Cards**
- Total Customers
- Churn Rate %
- Yearly Charges

**Charts**
- Churn by Type of Internet Service (Column Chart)
- % Customers by Internet Service (Pie Chart)
- Sum of Monthly Charges by Internet Service (Pie Chart)
- Churn by Type of Contract (Line & Clustered Column Combo)
- Churn by Years of Contract / Tenure (Line & Clustered Column Combo)
- Churn by Payment Method (Line & Clustered Column Combo)

---

## 📐 Data Model

The report is built on a single dataset containing the following key fields and calculated measures:

**Dimensions / Attributes**
| Field | Description |
|-------|-------------|
| `InternetService` | Type of internet service (DSL, Fiber, None) |
| `Contract` | Contract type (Month-to-month, One year, Two year) |
| `PaymentMethod` | Payment method used |
| `PaperlessBilling` | Whether the customer uses paperless billing |
| `tenure` | Number of months subscribed |
| `Tenure (in years)` | Tenure grouped by year |
| `Churn` | Whether the customer has churned (Yes/No) |

**Calculated Measures**
| Measure | Description |
|---------|-------------|
| `% Churn Rate` | Percentage of customers who churned |
| `% of Senior Citizen` | Share of customers who are senior citizens |
| `% of Partner` | Share of customers with a partner |
| `% of Dependents` | Share of customers with dependents |
| `% Phone Service` | Share using phone service |
| `% of Online Security` | Share using online security |
| `% of Online Backup` | Share using online backup |
| `% of Device Protection` | Share using device protection |
| `% of Tech Support` | Share using tech support |
| `% of Streaming TV` | Share using streaming TV |
| `% of Streaming Movies` | Share using streaming movies |
| `% of Yes-Multiple Lines` | Share with multiple lines |
| `% of No-Multiple Lines` | Share without multiple lines |

---

## 🎨 Theme

- **Theme name:** Sunflower Twilight (built-in Power BI theme)
- **Background:** White 

---

## 🚀 Getting Started

### Prerequisites

- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free) — November 2023 release or newer
- A dataset compatible with the telecom churn schema described above

### How to Open

1. Clone or download this repository.
2. Open Power BI Desktop.
3. Go to **File → Open report** and select `Customer_Churn_Dashboard.pbix`.
4. If prompted, connect to your data source or load sample data matching the schema above.

### Refreshing the Data

1. In Power BI Desktop, go to **Home → Transform Data** to access Power Query.
2. Update the data source path or connection string to point to your data.
3. Click **Home → Refresh** to load new data.

---

## 📊 Use Cases

- **Customer Retention Teams** — Identify at-risk customers and prioritize outreach.
- **Business Analysts** — Understand which contract types, payment methods, or services correlate with higher churn.
- **Executive Reporting** — Track monthly/yearly charge trends and overall churn rate at a glance.
- **Product Teams** — Evaluate which add-on services (tech support, online security, etc.) are associated with lower churn.

---



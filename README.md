# Customer Churn Dashboard

A Power BI dashboard analyzing customer churn risk, service subscriptions, billing behavior, and demographics for a telecom-style customer base.

![Dashboard Overview](docs/images/dashboard-overview.png)

## Overview

The **Customer Churn Dashboard** gives a single view into churn risk and its drivers — support ticket volume, subscribed services, contract type, and billing method — so teams can identify which customer segments are most likely to churn and why.

## Top KPI Cards

| Metric | Value |
|---|---|
| Customers at Risk | 1,869 |
| # of Tech Tickets | 2,173 |
| # of Admin Tickets | 885 |
| Yearly Charges | $2.86M |
| Monthly Charges | 139.13K |

## Demographics by Gender

- **Churned Customers by Gender** — donut chart: Female 939 (50.24%), Male 930 (49.76%)
- **Senior Citizen** — 25% of churned customers
- **Partner** — 36% have a partner
- **Dependents** — 17% have dependents
- **Subscription Time** — distribution of churned customers by tenure:
  - < 1 Year: 55.48%
  - < 2 Years: 15.73%
  - < 3 Years: 9.63%
  - < 4 Years: 7.76%
  - < 5 Years: 6.42%
  - < 6 Years: 4.98%

## Subscribed Services

| Service | % Adoption |
|---|---|
| Tech Support | 17% |
| Streaming TV | 44% |
| Streaming Movies | 44% |
| Device Protection | 29% |
| Online Backup | 28% |
| Online Security | 16% |
| Phone Service | 91% |
| Multiple Lines | 50.03% Yes / 49.97% No |

### Internet Service Users

| Type | % |
|---|---|
| Fiber optic | 69.40% |
| DSL | 24.56% |
| No internet service | 6.05% |

## Customer Account Information

**Payment Method**
| Method | % |
|---|---|
| Electronic check | 57.30% |
| Mailed check | 16.48% |
| Bank transfer | 13.80% |
| Credit card | 12.41% |

**Paperless Billing** — Yes 74.91% / No 25.09%

**Type of Contract**
| Contract | % |
|---|---|
| Month-to-month | 88.55% |
| One year | 8.88% |
| Two year | 2.57% |

**Average Charges**
- Monthly: $74.44
- Total: $1,531.80

## Tech Stack

- **Power BI Desktop** — data modeling, DAX measures, and report layout
- Data source: customer churn dataset (demographics, account info, service subscriptions, billing)

## Repository Structure

```
customer-churn-dashboard/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── images/
│   │   └── dashboard-overview.png
│   └── CHANGELOG.md
└── pbix/
    └── (place your .pbix file here)
```

## Getting Started

1. Clone this repository.
2. Open the `.pbix` file (once added under `pbix/`) in Power BI Desktop.
3. Update data source connections under **Home > Transform data > Data source settings**.
4. Refresh the data model.

## Roadmap / Ideas

- [ ] Add churn prediction model / risk score breakdown
- [ ] Add trend view of churn over time
- [ ] Add segment drill-through (e.g., by contract type or payment method)
- [ ] Document DAX measures in `docs/dax-reference.md`

## License

See [LICENSE](LICENSE).

# Hero MotoCorp — Integrated DCF Valuation Model

An integrated financial modelling and discounted cash flow (DCF) valuation project for **Hero MotoCorp**, built around a three-statement financial model, FCFF valuation framework, WACC calculation and DCF sensitivity analysis.

---

## Project Overview

This project develops an integrated financial model for Hero MotoCorp by linking historical financial statements with operating assumptions and a five-year forecast period.

The model estimates intrinsic equity value using a **Free Cash Flow to Firm (FCFF) based Discounted Cash Flow (DCF)** methodology.

### Key Components

- Historical and forecast revenue modelling
- Operating EBIT and profitability forecasting
- Integrated P&L, Balance Sheet and Cash Flow Statement
- Working-capital modelling
- Capex and depreciation schedules
- Free Cash Flow to Firm (FCFF)
- WACC calculation
- Enterprise-to-equity value bridge
- DCF sensitivity analysis
- Integrated model checks
- Valuation visualizations

---

# Model & Reports

## Excel Financial Model

The complete integrated financial model is available here:

**[Open the Hero MotoCorp DCF Model](MODEL/Hero_MotoCorp_DCF_Model.xlsx)**

The workbook contains the complete financial model, including:

- Executive Summary
- Revenue Model
- Assumptions
- Supporting Schedules
- P&L
- Balance Sheet
- Cash Flow Statement
- FCFF
- WACC
- Model Checks
- DCF Sensitivity

---

## Detailed Analysis Report

A PDF version of the analysis and valuation is available here:

**[View Hero MotoCorp DCF Analysis Report](DOCS/Hero_MotoCorp_DCF_Analysis_Report.pdf)**

---

# Base-Case Valuation

| Metric | Base Case |
|---|---:|
| Enterprise Value | ₹156,037 Cr |
| Equity Value | ₹170,284 Cr |
| Intrinsic Value / Share | ₹8,514 |
| Reference Market Price | ₹5,000 |
| WACC | 10.23% |
| Terminal Growth | 5.00% |
| Terminal Value / EV | 83.25% |
| Model-implied upside vs. reference price | 70.3% |

> The valuation figures above are outputs of the model's stated assumptions. They are not a recommendation to buy or sell the security.

---

# Forecast Horizon

The explicit forecast period runs from **FY26E to FY30E**.

| ₹ Cr | FY26E | FY27E | FY28E | FY29E | FY30E |
|---|---:|---:|---:|---:|---:|
| Revenue | 50,468 | 61,363 | 74,217 | 91,046 | 111,500 |
| Operating EBIT | 5,982 | 7,387 | 9,047 | 11,249 | 13,931 |
| Net Profit | 5,051 | 6,254 | 7,670 | 9,550 | 11,836 |
| CFO | 6,658 | 7,662 | 9,220 | 11,289 | 13,769 |
| Capex | 1,072 | 1,118 | 1,212 | 1,320 | 1,422 |
| Closing Cash | 5,896 | 12,371 | 20,307 | 30,203 | 42,477 |

---

# DCF Methodology

The model values the operating business using Free Cash Flow to Firm:

**FCFF = EBIT × (1 − Tax Rate) + D&A − Capex − Change in NWC**

Forecast FCFF is discounted using WACC.

### Terminal Value

The Gordon Growth approach is used:

**Terminal Value = FCFFₙ₊₁ / (WACC − Terminal Growth)**

The resulting enterprise value is converted into equity value through the model's cash, debt and other balance-sheet adjustments.

The implied equity value is then divided by the stated share count to calculate the intrinsic value per share.

### Detailed Methodology

**[Read Model Methodology](DOCS/MODEL_METHODOLOGY.md)**

---

# WACC

The base-case WACC used in the model is **10.23%**.

The WACC calculation incorporates:

- Risk-free rate
- Beta
- Equity risk premium
- Cost of equity
- Cost of debt
- Tax rate
- Capital structure

The complete calculation is available in the WACC section of the Excel model.

---

# Sensitivity Analysis

The DCF model evaluates intrinsic value across different combinations of:

- **WACC: 9.0%–12.0%**
- **Terminal Growth: 3.0%–6.0%**

The sensitivity analysis demonstrates how DCF valuation changes under different discount-rate and terminal-growth assumptions.

**[View DCF Sensitivity Chart](images/04_dcf_sensitivity.png)**

---

# Model Quality Checks

The final workbook was checked for:

- Broken Excel references
- Formula errors
- Forecast balance-sheet reconciliation
- Cash-flow reconciliation
- FCFF linkage
- WACC calculation
- Enterprise-to-equity value bridge
- Share-count linkage
- Sensitivity-table consistency

No formula-error cells were identified in the final checked workbook.

### Detailed Model Checks

**[View Model Checks](DOCS/MODEL_CHECKS.md)**

---

# Important Assumptions & Limitations

This is an **academic and portfolio financial modelling project**, not an investment recommendation.

The model contains historical source-data discrepancies that are disclosed rather than silently overwritten.

In particular:

- Historical Balance Sheet discrepancies exist for FY24 and FY25.
- Historical D&A differs from the supporting schedule for FY22 and FY23.
- These disclosed historical differences do not create a forecast formula error; the forecast model checks reconcile.

Market-sensitive assumptions such as the risk-free rate, beta, equity risk premium and reference price should be independently refreshed before using the model for a live investment decision.

### Detailed Assumptions & Limitations

**[Read Assumptions & Limitations](DOCS/ASSUMPTIONS_AND_LIMITATIONS.md)**

---

# Visual Outputs

## FCFF Forecast

![FCFF Forecast](images/01_fcff_forecast.png)

**[Open FCFF Forecast](images/01_fcff_forecast.png)**

---

## Revenue Trend

![Revenue Trend](images/02_revenue_trend.png)

**[Open Revenue Trend](images/02_revenue_trend.png)**

---

## Operating EBIT Margin

![Operating EBIT Margin](images/03_ebit_margin.png)

**[Open EBIT Margin Chart](images/03_ebit_margin.png)**

---

## DCF Sensitivity

![DCF Sensitivity](images/04_dcf_sensitivity.png)

**[Open DCF Sensitivity](images/04_dcf_sensitivity.png)**

---

## Vehicle Volume

![Vehicle Volume](images/05_vehicle_volume.png)

**[Open Vehicle Volume Chart](images/05_vehicle_volume.png)**

---

# Valuation Snapshot

The detailed valuation snapshot is available in the documentation folder:

**[View Valuation Snapshot](DOCS/VALUATION_SNAPSHOT.md)**

---

# Repository Structure

```text
Hero-Motocorp-DCF-Valuation/
│
├── DOCS/
│   ├── Hero_MotoCorp_DCF_Analysis_Report.pdf
│   ├── ASSUMPTIONS_AND_LIMITATIONS.md
│   ├── MODEL_CHECKS.md
│   ├── MODEL_METHODOLOGY.md
│   └── VALUATION_SNAPSHOT.md
│
├── MODEL/
│   └── Hero_MotoCorp_DCF_Model.xlsx
│
├── images/
│   ├── 01_fcff_forecast.png
│   ├── 02_revenue_trend.png
│   ├── 03_ebit_margin.png
│   ├── 04_dcf_sensitivity.png
│   └── 05_vehicle_volume.png
│
├── .gitignore
├── LICENSE
└── README.md

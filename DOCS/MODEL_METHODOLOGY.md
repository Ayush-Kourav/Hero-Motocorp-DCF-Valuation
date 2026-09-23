# Model Methodology

## 1. Historical Financials

Historical financial statements are incorporated into the workbook and used as the foundation for the forecast.

The model separates historical actuals (`A`) from estimates (`E`).

## 2. Revenue Forecast

Revenue is projected through the operating/revenue model using the assumptions contained in the workbook.

The model also tracks vehicle-volume assumptions as an operating driver.

## 3. Profitability

Operating EBIT is forecast from revenue and operating-margin assumptions.

The forecast P&L then flows through:

Revenue → Operating Profit → Financing/Other Items → Tax → Net Profit.

## 4. Cash Flow

Cash generation is linked to:

- Net profit
- Depreciation & amortisation
- Working-capital movements
- Capital expenditure
- Other cash-flow items

## 5. FCFF

The DCF uses Free Cash Flow to Firm.

Formula:

FCFF = EBIT × (1 − Tax Rate) + D&A − Capex − Change in NWC

FCFF is discounted at the model's WACC.

## 6. Terminal Value

The terminal value uses the perpetual-growth method:

TV = FCFFₙ × (1 + g) / (WACC − g)

where:

- `g` = terminal growth rate
- `WACC` = weighted average cost of capital

## 7. Enterprise Value

Enterprise value is the sum of:

- Present value of explicit-period FCFF
- Present value of terminal value

## 8. Equity Value

The model then bridges Enterprise Value to Equity Value using the relevant cash, debt and other balance-sheet adjustments included in the workbook.

## 9. Intrinsic Value Per Share

Intrinsic value per share is calculated as:

Equity Value / Diluted Share Count

## 10. Sensitivity Analysis

The sensitivity table varies:

- WACC
- Terminal growth

This illustrates the impact of key DCF assumptions on intrinsic value per share.

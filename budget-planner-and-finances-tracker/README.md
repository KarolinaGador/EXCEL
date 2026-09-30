# Personal Finance Tracker

<img width="1000" height="400" alt="image" src="https://github.com/user-attachments/assets/bf88d33a-eac6-4654-a8dd-49aa4b433d0f" />


A transaction-based finance model built on **207 sample transactions from 2024**, covering 3 banks and 7 account types.

**File:** [`Finances.xlsx`](./Finances.xlsx)

## Structure

| Sheet | Purpose |
|---|---|
| `operations` | Transaction log. Type and month are filled in automatically with `XLOOKUP` and `MONTH` |
| `Dicionary` | Lookup tables for categories, banks and products, feeding the dropdown lists |
| `1` – `12` | Monthly view: account balances (opening → closing), income and expenses by category |
| `summary1`, `summary2` | Category × month summaries built with `SUMIFS` formulas |
| `summary3` | The same summary rebuilt with a Pivot Table |

## Techniques used
- Excel Tables, `SUMIFS`, `XLOOKUP`, `MONTH`
- Data validation (dropdown lists)
- Pivot Tables
  
# Monthly Budget Planner

<img width="1662" height="729" alt="image" src="https://github.com/user-attachments/assets/4234810a-8ad9-4acc-a462-1a1288cd06a7" />


A 12-month budget template, one sheet per month, comparing **planned vs. actual vs. left** for income, expenses and savings.

**File:** [`Budget.xlsm`](./Budget.xlsm)

## What it does
- Separate tables for income sources, expense categories, bills, subscriptions and savings.
- Automatic "left to spend" calculations for every category.
- 3 charts and conditional formatting per month, so overspending is easy to spot at a glance.
- A VBA macro, **`DuplicateWorksheet`** (Ctrl+Shift+D), builds sheets 2–12 from the template and renames all the tables automatically (`Income_2`, `Expenses_2`, ...), instead of copying each month by hand.

## Techniques used
- Excel Tables 
- Charts
- Conditional formatting
- VBA (macro-recorded and edited)

## How to use
1. Open the file and **enable macros**, you also need to have finances file opened.
2. Fill in the *Planned* column for month 1.
3. Press **Ctrl+Shift+D** to generate the remaining 11 months.



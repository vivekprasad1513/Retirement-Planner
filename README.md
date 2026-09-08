# NivrittiPlan

A privacy-first, fully offline retirement and pension what-if planner for India.

NivrittiPlan helps users explore retirement corpus requirements, pension sustainability, investment scenarios, portfolio allocation, healthcare costs, spouse protection, and the impact of inflation.

> **Financial disclaimer:** This application is an educational simulator. It does not provide investment, tax, legal, insurance, or regulated financial advice.

## Table of Contents

- #overview
- #features
- #quick-start
- #how-to-use
- #calculation-model
- #privacy
- #data-export
- #technology
- #admin-build
- #browser-support
- [limitations
- #disclaimer
- [license

## Overview

NivrittiPlan is delivered as a single self-contained HTML file. It runs directly in a modern browser with no installation, server, API, CDN, account, or internet connection required.

The planner is designed around Indian currency formatting and common retirement instruments such as mutual funds, NPS, PPF, debt investments, systematic withdrawal plans, or SWPs, and annuities.

## Features

- Retirement corpus and pension projections
- Inflation-adjusted retirement goals
- SIP, annual step-up, lump-sum, and employer contribution modelling
- Custom portfolio allocations and expected returns
- SWP and annuity income estimates
- Year-by-year accumulation and corpus-depletion tables
- Monte Carlo simulation with reproducible random seeds
- Scenario comparison and sensitivity analysis
- Spouse survivor-income analysis
- Healthcare inflation and insurance stress testing
- Illustrative retirement-income tax modelling
- Required SIP, return, step-up, and retirement-age calculators
- Recommendation engine and retirement milestones
- Built-in calculation and chart diagnostics
- Local scenario saving
- CSV and JSON export
- Printable A4 summary
- Browser-based PDF export

## Quick Start

1. Download or clone the repository.
2. Open the following file in a modern browser:

```text
NivrittiPlan-Retirement-Planner-ADMIN.html
```

No build process or installation is required.

### Optional Local Server

Start a local server using Python:

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000/NivrittiPlan-Retirement-Planner-ADMIN.html
```

## How to Use

1. Enter your current age, retirement age, life expectancy, and spouse details.
2. Define the monthly pension you want in today's rupees.
3. Add your current SIP, existing corpus, lump sums, and employer contributions.
4. Review the inflation, investment return, withdrawal, annuity, tax, and healthcare assumptions.
5. Ensure the total portfolio allocation equals 100%.
6. Explore the dashboard, projections, scenarios, and sensitivity results.
7. Run the Monte Carlo simulation to evaluate a range of possible outcomes.
8. Save, print, or export your retirement plan.

Results update automatically whenever an assumption changes.

## Calculation Model

### Future Pension Target

```text
Future Monthly Pension =
Today's Monthly Pension × (1 + Inflation Rate) ^ Years to Retirement
```

### Required Corpus

```text
Required Corpus =
Annual Pension Requirement ÷ Withdrawal Rate
```

An inflation-adjusted legacy goal is added when configured.

### Funding Percentage

```text
Funding Percentage =
Projected Corpus ÷ Required Corpus × 100
```

### Retirement Income

```text
Monthly Retirement Income =
SWP Income + Annuity Income
```

Projected corpus calculations combine:

- Monthly investments
- Annual SIP step-ups
- Employer contributions
- Existing investments
- Annual lump-sum investments
- One-time investments
- Portfolio allocations
- Asset-specific return assumptions

Calculations use full JavaScript precision internally. Values are rounded only for display.

## Privacy

NivrittiPlan is designed to keep financial assumptions on the user's device.

- All calculations run locally in the browser
- No financial information is transmitted to a server
- No account or sign-in is required
- No analytics or external APIs are used
- Saved scenarios use browser Local Storage
- Exported reports are generated locally on the user's device

> Clearing browser data may permanently remove locally saved scenarios.

## Data Export

NivrittiPlan can generate:

- Year-by-year retirement projection CSV
- Retirement scenario summary CSV
- Assumptions JSON
- Printable A4 retirement summary
- PDF through the browser print dialog

Previously exported assumptions can be restored using the JSON import feature.

## Technology

NivrittiPlan is built using:

- HTML5
- CSS3
- Vanilla JavaScript
- Canvas-based charts
- Browser Local Storage

The application has zero runtime dependencies and is contained entirely within one HTML file.

## Admin Build

This repository contains the administrative build of NivrittiPlan.

The admin build:

- Opens the application automatically
- Bypasses the disclaimer acceptance screen
- Enables text selection and printing
- Removes protected-distribution interface restrictions
- Includes administrative chart-rendering overrides
- Includes a printable one-page A4 report

Review these administrative overrides before distributing the application to end users.

## Browser Support

Recommended browsers:

- Microsoft Edge
- Google Chrome
- Mozilla Firefox
- Safari

JavaScript and Local Storage must be enabled.

A desktop or laptop browser is recommended for reviewing detailed tables and charts.

## Limitations

- Results depend entirely on user-provided assumptions
- Investment returns and pension outcomes are not guaranteed
- Monte Carlo simulations use a simplified investment-return model
- Tax calculations are illustrative and may not match actual tax liability
- Annuity results are estimates and not live insurer quotations
- PPF rates, inflation, taxation, and market conditions may change
- Healthcare projections cannot predict individual medical events
- Saved scenarios are limited to the current browser and device
- Clearing browser storage may delete saved scenarios
- Imported JSON files must follow the application's assumptions structure

## Disclaimer

NivrittiPlan is provided solely for educational and illustrative purposes.

It is not:

- Personalised financial advice
- Investment advice
- Tax advice
- Legal advice
- Insurance advice
- A recommendation to purchase or sell a financial product
- A guarantee of future investment returns
- A guarantee of retirement income or financial security

All projections are hypothetical and depend on the assumptions entered by the user.

Historical or assumed investment returns do not guarantee future performance. Inflation, interest rates, taxation, annuity rates, healthcare expenses, and market conditions may change significantly over time.

Consult appropriately qualified financial, tax, legal, and insurance professionals before making financial decisions.

The author and contributors accept no liability for any loss or damage arising from the use of, or reliance on, NivrittiPlan.

## License

No open-source license is granted unless this repository includes a separate `LICENSE` file stating otherwise.

For a proprietary release, the following notice may be used:

```text
Copyright © [YEAR] [OWNER NAME]. All rights reserved.

This software may not be copied, modified, redistributed, reverse-engineered,
resold, sublicensed, or used commercially without prior written permission
from the owner.
```

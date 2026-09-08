# WealthHorizon PRO

[![HTML5](https://img.shields.io/badge/HTML5-Single_File-E=html5&logoColor=white](https://developer.mozilla.org/docs/Web/HTML)
[![JavaScript](httpsio/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=black](https://developer.mozilla.org/docs/Web/JavaScript)
https://img.shields.io/badge/Mode-Fully_Offline-22c55e](#privacy)
[![No Dependencies](httpsdge/Dependencies-None-7c5cff](#technology)
[![India](https://img.shields.io/badge/Designed_for-India-ff993ew)
[![Educational Use](https://img.shields.iotional-blue](#disclaimer)

A privacy-first, fully offline retirement and pension what-if planner for India.

WealthHorizon PRO helps users explore retirement corpus requirements, pension sustainability, investment scenarios, portfolio allocation, healthcare costs, spouse protection, and the impact of inflation.

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
- [Admin Build
- #limitations
- [Disclaimer](##license

## Overview

WealthHorizon PRO is delivered as a single self-contained HTML file. It runs directly in a modern browser with no installation, server, API, CDN, account, or internet connection required.

The planner is designed around Indian currency formatting and common retirement instruments such as mutual funds, NPS, PPF, debt investments, SWP, and annuities.

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
- Printable A4 summary and browser-based PDF export

## Quick Start

1. Download or clone the repository.
2. Open the following file in a modern browser:

```text
WealthHorizon-Retirement-Planner-ADMIN.html
```

No build or installation is required.

### Optional Local Server

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000/WealthHorizon-Retirement-Planner-ADMIN.html
```

## How to Use

1. Enter your age, retirement age, life expectancy, and spouse details.
2. Define the monthly pension you want in today's rupees.
3. Add your SIP, existing corpus, lump sums, and employer contributions.
4. Review inflation, return, withdrawal, annuity, tax, and healthcare assumptions.
5. Ensure the portfolio allocation totals 100%.
6. Explore the dashboard, projections, scenarios, and sensitivity results.
7. Run the Monte Carlo simulation for a range of possible outcomes.
8. Save, print, or export the plan.

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

Projected corpus calculations combine monthly investments, SIP step-ups, employer contributions, existing investments, lump sums, portfolio allocations, and asset-specific return assumptions.

## Privacy

- All calculations run locally in the browser
- No information is transmitted to a server
- No analytics or external APIs are used
- No account or sign-in is required
- Saved scenarios use browser Local Storage
- Exported reports are generated on the user's device

> Clearing browser data may permanently remove locally saved scenarios.

## Data Export

The application can generate:

- Year-by-year retirement projection CSV
- Retirement scenario summary CSV
- Assumptions JSON
- Printable A4 summary
- PDF through the browser print dialog

Previously exported assumptions can be restored through JSON import.

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Canvas-based charts
- Browser Local Storage
- Zero runtime dependencies

The complete application is contained in one HTML file.

## Admin Build

This repository contains the administrative build of WealthHorizon PRO.

The admin build:

- Opens the application automatically
- Bypasses the disclaimer acceptance screen
- Enables text selection and printing
- Removes protected-distribution interface restrictions
- Includes administrative chart-rendering overrides
- Includes a printable one-page A4 report

Review these overrides before distributing the application to end users.

## Browser Support

Recommended browsers:

- Microsoft Edge
- Google Chrome
- Mozilla Firefox
- Safari

JavaScript and Local Storage must be enabled. A desktop browser is recommended for detailed tables and charts.

## Limitations

- Results depend entirely on user-provided assumptions
- Investment returns and pension outcomes are not guaranteed
- Monte Carlo simulations use a simplified return model
- Tax calculations are illustrative
- Annuity results are not live insurer quotations
- PPF rates, inflation, taxation, and market conditions may change
- Healthcare projections cannot predict individual medical events
- Saved scenarios remain limited to the current browser and device

## Disclaimer

WealthHorizon PRO is provided solely for educational and illustrative purposes.

It is not:

- Personalised financial advice
- Investment, tax, legal, or insurance advice
- A recommendation to purchase or sell a financial product
- A guarantee of future returns or retirement income

Consult appropriately qualified financial, tax, legal, and insurance professionals before making financial decisions.

The author and contributors accept no liability for loss or damage arising from use of, or reliance on, this application.

## License

No open-source license is granted unless this repository includes a separate `LICENSE` file stating otherwise.

If the project is proprietary, you may use:

```text
Copyright © [YEAR] [OWNER NAME]. All rights reserved.

This software may not be copied, modified, redistributed, reverse-engineered,
resold, or used commercially without prior written permission from the owner.
```

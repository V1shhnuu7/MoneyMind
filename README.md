# MoneyMind — Financial Literacy Guide

A complete, interactive personal finance guide built as a single self-contained HTML file. Covers all 12 essential topics of financial literacy with live calculators, clear explanations, and a clean dark aesthetic.
![HTML](https://img.shields.io/badge/HTML-single%20file-c8f07a?style=flat-square)
![No dependencies](https://img.shields.io/badge/dependencies-none-7af0c8?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-b07af0?style=flat-square)

-----

Hosted in netlify 
https://mmbyzex.netlify.app


## What’s Inside

### 12 Topics

|# |Topic                  |Key Concepts                                                  |
|--|-----------------------|--------------------------------------------------------------|
|01|*Budgeting*          |50/30/20 rule, zero-based budgeting, pay yourself first       |
|02|*Saving*             |Emergency fund, savings ladder, automation                    |
|03|*Debt Management*    |Good vs bad debt, avalanche vs snowball method                |
|04|*Investing Basics*   |Asset classes, SIPs, diversification, index funds             |
|05|*Compound Interest*  |Time value of money, Rule of 72, early start advantage        |
|06|*Retirement Planning*|25× rule, NPS, PPF, EPF, 4% withdrawal rule                   |
|07|*Insurance*          |Term life, health, critical illness — separated from investing|
|08|*Taxes*              |Old vs new regime, 80C/80D/NPS deductions                     |
|09|*Credit Score*       |Payment history, utilisation, building from zero              |
|10|*Real Estate*        |Price-to-rent ratio, hidden costs, REITs                      |
|11|*Net Worth*          |Assets vs liabilities, the four growth levers                 |
|12|*Money Mindset*      |Behavioural biases, hedonic treadmill, automating virtue      |

### 8 Interactive Calculators

- *Budget splitter* — 50/30/20 calculator with live amounts
- *Emergency fund tracker* — target, gap, and progress bar
- *Debt true cost* — EMI, total interest, and regime verdict
- *SIP compound growth* — animated Chart.js growth curve
- *Retirement corpus planner* — inflation-adjusted target + required SIP
- *Tax regime comparator* — old vs new regime with all major deductions
- *Price-to-rent ratio* — buy vs rent verdict for any property
- *Net worth calculator* — full assets and liabilities breakdown

-----

## Project Structure


moneymind/
├── financial-literacy.html   # The entire application — one file
└── README.md


Everything — HTML, CSS, JavaScript, and content — lives in financial-literacy.html. This was a deliberate design choice: maximum portability, zero setup friction.

-----

## Tech Stack

|Layer    |Choice                                                                          |Why                              |
|---------|--------------------------------------------------------------------------------|---------------------------------|
|Structure|HTML5                                                                           |Single-file portability          |
|Styling  |Vanilla CSS with CSS variables                                                  |No framework needed at this scale|
|Logic    |Vanilla JavaScript                                                              |No build toolchain required      |
|Charts   |[Chart.js 4.4.1](https://www.chartjs.org/) via CDN                              |Best balance of quality and size |
|Fonts    |[Google Fonts](https://fonts.google.com/) — Playfair Display + DM Sans + DM Mono|Loaded on first open             |

-----

## Calculators: Methodology Notes

All calculators use standard financial formulas for educational illustration. They are approximations — not financial advice.

- *SIP returns* use the standard future value of a recurring investment: FV = P × ((1+r)^n − 1) / r × (1+r)
- *Tax calculator* uses FY 2024-25 slabs with 4% cess (Health & Education). Old regime standard deduction ₹50,000; new regime ₹75,000.
- *Retirement corpus* uses the 25× rule against inflation-adjusted future expenses at a 12% nominal return assumption.
- *Debt EMI* uses the standard reducing-balance EMI formula.
- *Price-to-rent ratio* benchmarks: below 15 favours buying, 15–20 borderline, above 20 favours renting.

-----

## Customisation

To adapt this for a different country or context:

1. *Currency symbol* — search for ₹ and replace with your symbol
1. *Tax slabs* — update the calcTax() function with your country’s brackets
1. *Instruments* — replace PPF/NPS/EPF references in the retirement and savings sections
1. *Inflation assumption* — the retirement calculator defaults to 6%; adjust ret-inf slider default

-----

## Contributing

Contributions welcome. Some ideas:

- [ ] Add a goal-based savings calculator (house, car, education)
- [ ] Add a loan prepayment vs invest comparison calculator
- [ ] Add a FIRE (Financial Independence, Retire Early) number calculator
- [ ] Improve mobile layout for the net worth two-column input
- [ ] Add a dark/light mode toggle
- [ ] Translate content for other markets (US, UK, Singapore)

To contribute: fork → make changes → open a pull request.

-----

## Disclaimer

This guide is for *educational purposes only* and does not constitute financial advice. All calculators use simplified assumptions. Consult a SEBI-registered financial advisor for personalised investment guidance. Tax calculations are based on publicly available rules and may not reflect the latest amendments.

-----

## License

MIT License — use freely, modify freely, share freely.

-----

Built as part of a comprehensive financial literacy curriculum. The best time to start was yesterday. The second best time is today.

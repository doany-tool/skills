---
name: missed-call-revenue-calculator
displayName: Missed call revenue calculator
description: >-
  Estimate revenue and gross profit at risk from missed business calls using
  the share of new prospects, unrecovered calls, close rate, and first-year
  job value. Use to compare the economics of an answering service or call
  coverage change.
---

# Missed call revenue calculator

Use the [Missed call revenue calculator](https://doany.ai/tools/missed-call-revenue-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=missed-call-revenue-calculator&utm_content=missed-call-revenue-calculator) to enter phone-log counts, see the calculation for the selected period, and compare a monthly answering cost.

## Start with the call log

Get missed calls and their reporting period. Ask what fraction are new prospects, what fraction of those are unrecovered, and how often answered prospects become customers. Exclude calls that were answered from the starting count. Ask for average first-year job value per visit, visits per new customer, and gross margin.

## Calculate revenue and profit at risk

1. Multiply missed calls by the new-prospect share, unrecovered share, and close rate, in that order. Treat the result as expected customers at risk.
2. Multiply by average job value and jobs per new customer. Multiply revenue at risk by gross margin to estimate gross profit at risk. When starting from a weekly log, use 52 weeks per year and 52 ÷ 12 weeks per average month.
3. For an answering option, apply the owner's assumed recovery share to monthly gross profit at risk and subtract its monthly cost. Report assumptions and use a conservative recovery scenario.

## Browser workflow

When the page exposes browser actions, use `calculate_missed_call_revenue` with the user's call log and assumptions, then `get_missed_call_revenue` to verify the active period, caller shares, and answering-cost comparison.

## Example

Of 12 weekly missed calls, suppose 60% are new prospects and half never reconnect. At a 40% close rate, 1.44 customers are at risk per week. One $350 job each gives $504 weekly or $2,184 per average month. At 50% gross margin, $1,092 monthly gross profit is at risk before any recovery assumption.

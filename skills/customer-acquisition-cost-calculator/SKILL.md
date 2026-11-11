---
name: customer-acquisition-cost-calculator
displayName: Customer acquisition cost calculator
description: >-
  Calculate customer acquisition cost per new paying customer from sales and
  marketing expense. Use to compare blended or channel CAC, payback in jobs or
  months, and lifetime gross profit relative to CAC.
---

# Customer acquisition cost calculator

Use the [Customer acquisition cost calculator](https://doany.ai/tools/customer-acquisition-cost-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=customer-acquisition-cost-calculator&utm_content=customer-acquisition-cost-calculator) to compare two acquisition scenarios and export the cost and customer counts.

## Define the cohort and costs

Confirm the acquisition period, currency, channel scope, attribution rule, and count of unique new paying customers. Include attributable ads, agency costs, tools, payroll, and commissions where appropriate. Deduplicate shared expenses and use the same scope for cost and customer count.

## Calculate and interpret

1. Divide marketing plus sales costs by new paying customers. If there were none, report that CAC cannot be computed for that cohort.
2. Divide CAC by positive gross profit per job or month to estimate payback in the matching unit. If gross profit is zero, report that the entered figures cannot establish payback. If the user supplies lifetime jobs or months, multiply lifetime units by the corresponding gross profit. Show the lifetime gross profit to CAC ratio when CAC is positive.
3. Return the cost categories, denominator, CAC, and any optional payback or lifetime ratio. Compare two cohorts only after stating any attribution or timing difference.

## Browser workflow

When the page exposes browser actions, use `calculate_customer_acquisition_cost` and `get_customer_acquisition_cost` to confirm the two cost categories and paying-customer count. Read any payback and lifetime figures in their reported units.

## Example

With $800 marketing cost and $400 sales cost for 20 new paying customers, CAC is $60. At $30 gross profit per job, payback takes two jobs. If a customer averages five jobs, modeled lifetime gross profit is $150 and the ratio is 2.5×.

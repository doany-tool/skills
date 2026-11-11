---
name: roas-calculator
displayName: ROAS calculator
description: >-
  Calculate return on ad spend as a multiple and percentage, plus contribution
  after ads and break-even ROAS. Use to compare campaign scenarios with a
  consistent attribution window and pre-ad contribution margin.
---

# ROAS calculator

Use the [ROAS calculator](https://doany.ai/tools/roas-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=roas-calculator&utm_content=roas-calculator) to compare spend and attributed revenue in two scenarios and export the figures.

## Align the inputs

Get ad spend and revenue attributed to that spend, with the same campaign scope, reporting period, currency, and attribution rule. Record how returns and discounts were handled. If known, get the contribution margin before advertising, after variable costs such as fulfillment and payment fees. It can also be derived from a selling price and variable cost per sale.

## Calculate and compare

1. Divide attributed revenue by positive ad spend. Show the result as both a multiple and a percentage. Report zero spend as an unavailable ratio.
2. For a positive contribution margin, divide one by the margin fraction to find break-even ROAS. Calculate contribution after ads as attributed revenue × pre-ad margin − spend. If margin is missing, report ROAS and identify what is needed for the profit calculation.
3. For a second scenario, state which inputs changed. Keep attribution assumptions and cost basis consistent. Report any fixed costs left outside the calculation and treat future spend and revenue as assumptions.

## Browser workflow

When the page exposes browser actions, use `calculate_roas` for the selected scenario and `get_roas` to confirm that spend, attributed revenue, and any contribution margin are on the intended basis.

## Example

At $500 spend and $2,000 attributed revenue, ROAS is 4× or 400%. At a 30% contribution margin, break-even is about 3.33× and contribution after ads is $100.

---
name: cpm-calculator
displayName: CPM calculator
description: >-
  Calculate cost per thousand ad impressions, budget for a target, or
  impressions affordable at a specified CPM. Use to compare two campaign
  placements, quotes, or budget plans with consistent impression definitions.
---

# CPM calculator

Use the [CPM calculator](https://doany.ai/tools/cpm-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=cpm-calculator&utm_content=cpm-calculator) to choose the calculation direction and export both campaign scenarios if needed.

## Match the known inputs

Ask which result is missing. Get spend and impressions for actual CPM, the quoted CPM and target impressions for budget, or the budget and quoted CPM for affordable impressions. Confirm currency, measurement period, and whether the count is all served impressions or viewable impressions.

## Calculate

| Result | Formula |
| --- | --- |
| CPM | Spend ÷ impressions × 1,000 |
| Budget | CPM × target impressions ÷ 1,000 |
| Affordable impressions | Budget ÷ CPM × 1,000 |

For a budget to cover the whole target, round required currency upward at the smallest billable unit. For affordable impressions, round downward to whole impressions and keep any unrounded planning estimate separate. Check that any denominator is positive. Show CPM and the underlying spend and impression counts for each scenario.

## Browser workflow

When the page exposes browser actions, use `calculate_cpm` and `get_cpm` to check the active calculation direction, currency, and rounded result.

## Example

250,000 impressions at an $8 CPM need $2,000. A $1,000 budget at a $7 CPM buys up to 142,857 whole impressions at that assumed rate.

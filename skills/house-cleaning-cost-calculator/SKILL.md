---
name: house-cleaning-cost-calculator
displayName: House cleaning cost calculator
description: >-
  Price a house cleaning visit by square footage, room count, billable hours,
  or actual costs. Use to compare standard, deep, move-out, and recurring
  cleans with add-ons, discounts, and a minimum visit charge.
---

# House cleaning cost calculator

Use the [House cleaning cost calculator](https://doany.ai/tools/house-cleaning-cost-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=house-cleaning-cost-calculator&utm_content=house-cleaning-cost-calculator) to compare visit prices, crew time, and monthly amounts or carry the selected price into a cleaning estimate.

## Choose the pricing method

| Method | Inputs to confirm |
| --- | --- |
| By area | Cleanable square feet and the owner's standard price per square foot |
| By rooms | Bedrooms, bathrooms in half-bath increments, and separate rates per bedroom and bathroom |
| By time | Estimated cleaner-hours and the matching labor selling rate |
| From costs | Crew pay, payroll burden, paid travel, supplies, vehicle costs, overhead, client mix, and target margin |

## Work out each visit

1. Confirm the type of clean, property condition, and the crew's work rate or expected cleaner-hours. For deep or move-out work, use the user's multiplier. In the cost method, apply it to the cleaning time and price the resulting costs.
2. Add approved extras and the supplies or travel charges that apply. Confirm which line items are customer charges and which are already included in underlying costs.
3. In rate-based modes, apply the selected recurring discount to the subtotal, then enforce any minimum. One-off visits use the one-off terms. In the cost method, use the costs and target for each visit frequency, including overhead allocation and time.
4. Return per-visit price, estimated on-site time, extras, and average monthly amount with its frequency assumption. Distinguish cleaner-hours from elapsed crew time. Explain how the chosen frequency affects the result.

## Browser workflow

When the page exposes browser actions, use the action that matches the method: `price_cleaning_by_square_feet`, `price_cleaning_by_rooms`, `price_cleaning_by_the_hour`, or `price_cleaning_from_my_costs`. Read the current result with `get_house_cleaning_price`. Use `use_house_cleaning_price_in_estimate` when the owner asks to carry the reviewed visit price into the estimate.

## Example

At $0.15 per square foot, 1,000 square feet gives a $150 standard base. Add a $30 agreed extra for a $180 subtotal. A 10% recurring discount gives $162, then a $170 minimum sets the price to $170 per visit.

---
name: profit-margin-calculator
displayName: Profit margin calculator
description: >-
  Calculate profit margin and markup from selling price and cost, or solve for
  a target price, cost ceiling, or profit. Use to compare margins on a sale
  and check the effect of discounts or changing costs.
---

# Profit margin calculator

Use the [Profit margin calculator](https://doany.ai/tools/profit-margin-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=profit-margin-calculator&utm_content=profit-margin-calculator) to select the known figures, compare a target margin, and check the result in the chosen currency.

## Select the inputs

Use the realized selling price after discount and before sales tax. Gather costs for the same sale and state whether they include delivery, payment fees, or allocated overhead. Confirm currency and whether the user wants to check an existing sale or solve for a target.

## Solve and check

- With price and cost, calculate profit as price minus cost. Profit divided by price is margin. Profit divided by cost is markup. With price and profit, subtract profit from price to recover cost.
- With cost and target margin, divide cost by one minus the margin and round the required price upward to the currency unit. With price and target margin, multiply price by one minus the margin and round the allowable cost downward.
- With positive profit and positive target margin, divide profit by the margin to find the maximum selling price at that exact profit, then derive cost by subtraction. Round the price downward and recheck the achieved margin. A zero or missing denominator needs clarification.
- Return the input assumptions, price, cost, profit, margin, and markup. Show how a proposed change compares on the same cost basis.

## Browser workflow

When the page exposes browser actions, use `calculate_profit_margin` for the selected pair of known values and `get_profit_margin` to inspect the calculation. Verify the currency and direction of rounding before quoting the result.

## Example

At a $120 price and $72 cost, profit is $48 and margin is 40%. To reach 45% with the same cost, price at $130.91 or higher in cents.

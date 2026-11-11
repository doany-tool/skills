---
name: break-even-calculator
displayName: Break-even calculator
description: >-
  Calculate the break-even sales, jobs, or customers needed to cover fixed
  costs, plus units required for a target profit. Use to compare price,
  variable cost, fixed costs, or planned volume in two scenarios.
---

# Break-even calculator

Use the [Break-even calculator](https://doany.ai/tools/break-even-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=break-even-calculator&utm_content=break-even-calculator) to compare scenarios and inspect the break-even chart for the selected period.

## Gather compatible inputs

Get fixed costs for the period, realized pre-tax selling price per unit, variable cost per unit, and any expected volume or profit target. Use one consistent unit such as one job, product, or paying customer. For a mixed portfolio, use an explicitly weighted mix or calculate each product on a documented allocation basis.

## Solve for the threshold

1. Subtract variable cost from selling price to get contribution per unit. If contribution is nonpositive, extra sales cannot cover positive fixed costs under these assumptions.
2. Divide fixed costs by contribution to find the exact break-even point. Round up when units must be whole and report both figures. Multiply the rounded sales count by price if the user needs whole-unit break-even revenue.
3. For a target profit, add it to fixed costs before dividing and round required units up. For an expected volume, multiply volume by contribution and subtract fixed costs.
4. State the inputs and compare changes on the same period and unit basis. Label volume as a scenario assumption.

## Browser workflow

When the page exposes browser actions, use `calculate_break_even` and `get_break_even` to confirm the current contribution per unit, the whole-unit threshold, and the optional volume or profit target.

## Example

With $1,500 fixed costs, a $60 sale price, and $35 variable cost, contribution is $25 and break-even is 60 sales. A $500 profit goal needs 80 sales.

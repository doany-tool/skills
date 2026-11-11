---
name: contractor-markup-calculator
displayName: Contractor markup calculator
description: >-
  Calculate a contractor selling price from total job cost and markup, find
  the price for a target margin, or evaluate an existing quote. Use to compare
  markup, margin, and profit before tax and payment fees.
---

# Contractor markup calculator

Use the [Contractor markup calculator](https://doany.ai/tools/contractor-markup-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=contractor-markup-calculator&utm_content=contractor-markup-calculator) to check the markup-to-margin conversion and compare the result with a price you already quote.

## Confirm the inputs

Get total job cost including labor, materials, overhead allocation, equipment, and subcontractors that apply. Ask whether the user has a markup percentage, wants a margin, or already has a selling price. Keep all amounts on the same pre-tax basis and identify fees separately.

## Calculate the requested view

| Known inputs | Calculation |
| --- | --- |
| Cost and markup | Price = cost × (1 + markup) |
| Cost and target margin | Price = cost ÷ (1 − margin) |
| Cost and existing price | Profit = price − cost. Margin = profit ÷ price. Markup = profit ÷ cost |

Round a required selling price upward to the cent. A margin target must be below 100%. If the denominator is zero, leave the ratio unavailable. Show job cost, selling price, profit, and both percentages. State if the quoted price falls below the target or below cost.

## Browser workflow

When the page exposes browser actions, use `calculate_contractor_markup` for the chosen input mode and `get_contractor_markup` to inspect the result. Check that the target is entered as the intended ratio.

## Example

A $1,000 job with a 25% markup sells for $1,250, producing $250 profit and 20% margin. A 25% margin needs a selling price of $1,333.34 before any tax or processing fee.

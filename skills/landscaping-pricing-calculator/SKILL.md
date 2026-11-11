---
name: landscaping-pricing-calculator
displayName: Landscaping pricing calculator
description: >-
  Calculate what to charge for landscaping by job or crew-hour using labor,
  material units, waste, equipment, travel, overhead, and profit target. Use
  to evaluate a minimum charge, price per area, or recurring season totals.
---

# Landscaping pricing calculator

Use the [Landscaping pricing calculator](https://doany.ai/tools/landscaping-pricing-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=landscaping-pricing-calculator&utm_content=landscaping-pricing-calculator) to compare prices and carry the final job or visit into a landscaping estimate.

## Build the cost for this work

- Select the kind of landscaping work so the quote labels match the job. Record labor hours and matching person or crew rate, material quantity and cost per unit, and travel, equipment, disposal, or subcontractors. Label the units for each material.
- Round the base materials line to cents, calculate waste on that line, and include allocated overhead. Apply contingency to the resulting subtotal, then identify any minimum job or visit charge.
- Confirm the target as selling-price margin, cost markup, or dollar profit, and ask for any percentage, fixed, and capped processing fee on the payment.

## Price and compare

1. Calculate the minimum pre-tax price that meets the target after costs and payment fee. For margin, evaluate the actual profit divided by price. With no fee, divide job cost by one minus the margin and round up to cents.
2. Apply a higher confirmed minimum charge and recompute fee and profit. For hourly billing, round up the rate and recheck the billed total against the target and minimum. Report current and alternative quotes on the same cost and fee basis.
3. Use the final price for any area calculation. If the displayed rate per square foot rounds below $0.10, report a rate per 1,000 square feet. For recurring service, multiply price per visit by visits in the season. Divide by season months and round the monthly amount up to cents.
4. Return the cost breakdown, break-even, quote, fee, and profit with the applicable billing unit. Transfer one job or visit into the estimate after the owner reviews it.

## Browser workflow

When the page exposes browser actions, use `get_service_price` to check current landscaping inputs and `calculate_service_price` to set confirmed job details and compare alternatives. If the user requests an estimate, `use_service_price_in_estimate` carries the final job or single visit into the matching template.

## Example

A $198 visit scheduled 15 times gives $2,970 for the season. Across seven months, the monthly amount rounds up to $424.29. Use the single-visit amount for the visit estimate.

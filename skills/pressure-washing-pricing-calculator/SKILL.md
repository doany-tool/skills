---
name: pressure-washing-pricing-calculator
displayName: Pressure washing pricing calculator
description: >-
  Price a pressure washing job by surface rates or from measured area, crew
  production, chemicals, overhead, and a target margin. Use for multi-surface
  power washing quotes, minimum charges, and a per-surface rate card.
---

# Pressure washing pricing calculator

Use the [Pressure washing pricing calculator](https://doany.ai/tools/pressure-washing-pricing-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=pressure-washing-pricing-calculator&utm_content=pressure-washing-pricing-calculator) to compare the two pricing methods, download a rate card, or open a pressure washing estimate with the result.

## Gather the measurements

List surfaces separately, including their dimensions or area, material, and condition. For each one, enter the whole crew's production rate in square feet per hour if pricing from costs. Get any extra percentage for access, staining, height, or steepness. Use the owner's observed rates.

## Choose a pricing method

- **Price per square foot**. Multiply each area by the owner's selling rate. Apply its surface adjustment, round the line, and sum the lines. Use a higher confirmed minimum charge when applicable.
- **From costs**. Divide each surface's area by its crew production rate and allow extra time where specified. Add setup and cleanup once. Multiply elapsed crew-hours by crew size and loaded cost per worker-hour. Calculate the mixed chemical cost for each area at the supplied cost per 100 square feet, then add equipment, vehicle, and job overhead.
- Divide total cost by one minus the target margin and round up to cents, then compare with the minimum. Use the higher price. To reconcile the surface breakdown, account for each surface's chemicals and distribute the remaining amount by crew time. Assign rounding cents by largest remainder so the lines sum to the job price.

## Check and report

Show the method, all surface quantities, crew assumptions if used, cost and margin where available, and whether the minimum sets the price. Carry measured surfaces and the reviewed price into the estimate. Confirm site and water access separately from the price.

## Browser workflow

When the page exposes browser actions, use `calculate_pressure_washing_price` with the chosen method and measured surface rows, then `get_pressure_washing_price` to inspect the breakdown. If requested, use `use_pressure_washing_price_in_estimate` to open the matching estimate with the reviewed price.

## Example

With $410.16 of total cost and a 35% margin, the target rounds up to $631.02. A $650 minimum makes the quote $650 and the modeled profit $239.84.

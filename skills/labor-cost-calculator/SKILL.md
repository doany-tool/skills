---
name: labor-cost-calculator
displayName: Labor cost calculator
description: >-
  Calculate loaded labor cost per paid hour and billable hour from wages,
  employer burden, fixed benefits, and productive hours. Use to price a crew
  or individual, allocate overhead, or find a selling rate that reaches a
  target margin.
---

# Labor cost calculator

Use the [Labor cost calculator](https://doany.ai/tools/labor-cost-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=labor-cost-calculator&utm_content=labor-cost-calculator) to model worker groups over a week, month, or year and carry an agreed labor cost into service pricing.

## Get consistent period inputs

- Group workers with the same pay, paid hours, billable hours, employer burden, and fixed benefits. Enter headcount and per-person values for each group. Paid travel, training, and leave can increase paid hours without increasing billable hours.
- Gather employer taxes and other wage-based costs as the owner's burden rate, plus benefits paid as fixed money for the period. Count the same benefit once. Include the owner's wage equivalent when their work is part of the job.
- Get company overhead for the same period and the margin target. Ask for jointly billable crew hours if the entire crew is sold as a unit. Use one period across all rows.

## Work out the rates

1. For each group, calculate wages as headcount × paid hours × hourly wage. Add wage burden and fixed benefits for those workers. Sum the results and both hour counts.
2. Divide loaded payroll by paid hours to show the employer cost per paid hour. Divide by billable person-hours to find the loaded cost per billable hour. Positive billable capacity is required, and billable hours per person must fit within paid hours.
3. Add company overhead to loaded payroll and divide by the same billable hours for break-even. Divide break-even by one minus the desired margin and round the selling rate upward to cents. If using joint crew hours, divide by that capacity and label the resulting rate per crew-hour.
4. Return wages, burden, benefits, utilization, overhead, and the three rates. Carry the loaded cost or overhead-inclusive cost into a quote and account for overhead and profit once.

## Browser workflow

When the page exposes browser actions, use `get_labor_cost` to inspect current worker groups and the period. Use `calculate_labor_cost` with the owner's confirmed inputs, replacing any flagged example values. When carrying an agreed cost into pricing, `use_labor_cost_in_pricing` transfers a cost basis for the selected unit.

## Example

Two workers each earn $25 for 160 paid hours, of which 80 are billable. A 20% employer burden and zero fixed benefits give $9,600 loaded payroll. With $2,000 overhead, 160 billable person-hours give $60.00 in labor and $72.50 break-even per person-hour. A 30% margin requires $103.58 per billable person-hour.

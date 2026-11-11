---
name: automation-roi-calculator
displayName: Automation ROI calculator
description: >-
  Estimate automation ROI from manual effort, automatable share, human review,
  loaded hourly cost, and realizable savings. Use to compare setup cost,
  recurring cost, payback, and net benefit over an automation's lifespan.
---

# Automation ROI calculator

Use the [Automation ROI calculator](https://doany.ai/tools/automation-roi-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=automation-roi-calculator&utm_content=automation-roi-calculator) to compare a base case with a more conservative scenario and export the assumptions.

## Measure the work and costs

Get observed manual hours per active week, share the automation handles, review and exception hours, active weeks, and the loaded hourly value. Ask what share of freed capacity will translate into financial value. Gather upfront build, integration, and training cost plus monthly usage, maintenance, and support costs.

## Build the business case

1. Calculate annual released hours as (manual hours × automated share − review hours) × active weeks. Keep a negative result visible as a time shortfall.
2. Multiply by hourly value and then by realizable share. Report released capacity and modeled financial benefit separately.
3. Subtract 12 months of operating cost for annual ongoing net benefit. Subtract setup once for first-year net. Divide first-year net by first-year costs for first-year ROI if the cost denominator is positive.
4. For positive monthly ongoing net benefit, divide setup by that unrounded monthly figure for payback. Over the chosen life, multiply annual ongoing net benefit by years and subtract setup. Compute lifetime ROI against setup plus running costs over that life.
5. Compare at least one sensitivity the user cares about, such as lower automation coverage or additional review time.

## Browser workflow

When the page exposes browser actions, use `calculate_automation_roi` and `get_automation_roi` to read the assumed weeks, realization share, and setup and running costs before quoting payback.

## Example

20 manual hours per active week, 70% coverage, 2 review hours, and 48 active weeks free 576 hours per year. At $40 an hour and 50% realizable value, modeled annual benefit is $11,520. With $200 monthly cost and $3,000 setup, first-year net is $6,120 and payback is about 3.95 months.

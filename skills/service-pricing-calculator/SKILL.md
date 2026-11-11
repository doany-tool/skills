---
name: service-pricing-calculator
displayName: Service price calculator
description: >-
  Calculate a job quote or billable hourly rate for cleaning, landscaping,
  pressure washing, and other services. Use when someone asks how much to
  charge, wants a break-even price, or needs to compare prices after labor,
  materials, overhead, and card fees at a target margin, markup, or profit.
---

# Service price calculator

Build a cost-based quote in USD before tax. Use the [Service price calculator](https://doany.ai/tools/service-pricing-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=service-pricing-calculator&utm_content=service-pricing-calculator) to try different prices, download a CSV or PDF summary, or carry the chosen price into an estimate.

## Define the work and billing unit

- For a **fixed-price job**, gather costs for the entire scope. Calculate labor from crew size, paid hours per worker, and hourly pay when the user gives those inputs. Add separate worker groups if their pay or hours differ.
- For an **hourly quote**, get the billable hours for this job and the labor cost per matching hour. Two workers on site for three hours give six person-hours or three crew-hours. For a crew-hour, include the cost of everyone working that hour. Apply labor and overhead using consistent units.
- Ask for the profit target and whether it is a margin, a markup, or a dollar amount. Ask only for missing inputs that materially affect the quote. Keep any provisional assumptions visible and use the owner's figures for their job.

## Build the job cost

| Type of work | Materials calculation |
| --- | --- |
| General service | One materials total for the job |
| Cleaning | Number of visits × supplies per visit |
| Landscaping | Material units × cost per matching unit, such as bags of mulch or cubic yards of gravel |
| Pressure washing | Square feet being cleaned × detergent cost per square foot |

- Include the owner's time in labor when its cost is known. If it is missing, explain that the profit shown still has to cover that time.
- Use the job's share of overhead. If the user has a monthly overhead figure, divide it by the month's billable hours and multiply by this job's hours on the same basis. Check whether an imported labor rate already includes overhead before adding a separate amount.
- Count travel, equipment, and subcontractors once. Apply waste to the materials line, then add contingency to the full cost subtotal, including waste. Keep both amounts visible in the breakdown.

## Calculate the quote and check alternatives

Let `C` be total job cost and `P` be the pre-tax selling price. Use exact decimals and integer cents for settled amounts. For a single card payment, calculate `fee(P)` by rounding `P × fee rate` to cents, adding the fixed fee, then applying any cap. Use the payment terms the user supplies. For split payments, get the schedule and calculate each fee separately before evaluating profit. The linked calculator models one payment for the job.

| Target | Required price with the fee at the candidate price |
| --- | --- |
| Margin `m` | `(C + fee(P)) / (1 − m)` |
| Markup `k` | `C × (1 + k) + fee(P)` |
| Dollar profit `d` | `C + d + fee(P)` |
| Break-even | `C + fee(P)` |

1. Enter rates as fractions in the formulas. Start the quote at `C` and round the required price upward to cents. If it exceeds the candidate, move to that price and recalculate the fee. Repeat until the actual profit meets the target. For an uncapped fee, flag a margin target that reaches 100% together with the fee rate. A margin target must be below 100%.
2. For an hourly quote, divide the job target by billable hours and round the rate up to cents. Multiply the rate by those hours and round the billed total to cents. Recheck the fee and profit on that total, then raise the rate if the rounded total falls short.
3. Calculate profit as `P − C − fee(P)`, margin as `profit / P`, and markup as `profit / C`. Show a ratio as unavailable if its denominator is zero. For a current price or a proposed alternative, use the same job costs and recalculate the fee on each price. Multiply each hourly rate by the same hours before comparing totals.

For landscaping, apply an optional minimum charge when it exceeds the computed job or visit price. Round the corresponding hourly rate upward when applicable, then recompute the fee and profit at the resulting total. If an area is provided, divide the final price by the square footage and use a per-1,000-square-foot figure when the rounded price per square foot is below $0.10. For recurring work, multiply the final visit price by visits per season and divide by the number of months, rounding the monthly amount upward to cents.

## Work in the browser when site tools are available

Open the linked calculator and inspect its current state with `get_service_price`. Use `calculate_service_price` with the confirmed job inputs. The page opens with example figures and keeps any fields the call omits. Check that the result uses the user's figures, zero out confirmed non-applicable costs, and clear unused comparison prices. If the page flags a conflict with the user's edits, show the conflict and ask which values to use.

Return the quote with its unit, job total, cost breakdown, break-even total, processing fee, profit, margin, and markup. Include the current and proposed prices when provided. If the user asks for an estimate, use `use_service_price_in_estimate` when exposed, or direct them to the estimate button. The transfer opens the matching estimate with the chosen price and billing quantity. For seasonal landscaping, it transfers one visit. Review the result before handing it off. When the browser tools are unavailable, calculate from the confirmed inputs in the conversation.

## Worked example

A cleaning job needs two visits, four billable person-hours at $25 in labor cost per hour, and $8 of supplies per visit. Add 10% material waste, $12 for travel, and the job's share of $900 monthly overhead across 120 billable person-hours. The overhead share is $30. The subtotal is $159.60. Add $7.98 of contingency at 5%, bringing total cost to **$167.58**.

With a 25% margin target and a single card fee of 2.9% plus $0.30, break-even is **$172.89** for the job.

| Scenario | Per person-hour | Job total | Card fee | Profit | Margin |
| --- | ---: | ---: | ---: | ---: | ---: |
| Current | $55.00 | $220.00 | $6.68 | $45.74 | 20.79% |
| Meets target | $58.21 | $232.84 | $7.05 | $58.21 | 25.00% |
| Price to try | $60.00 | $240.00 | $7.26 | $65.16 | 27.15% |

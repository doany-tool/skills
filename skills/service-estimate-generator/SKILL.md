---
name: service-estimate-generator
displayName: Estimate generator
description: >-
  Turn a service job into a customer-ready estimate with line-item quantities,
  prices, scope, exclusions, discounts, and confirmed tax. Use when asked to
  draft a quote or prepare an estimate PDF for a cleaning, landscaping,
  pressure washing, or general service job.
---

# Estimate generator

Build the estimate in conversation, then use the [Estimate generator](https://doany.ai/tools/service-estimate-generator?utm_source=skills.sh&utm_medium=skill&utm_campaign=service-estimate-generator&utm_content=service-estimate-generator) to edit the live document and export a PDF.

## Gather the job and quote details

- Get the business name and contact block, the customer or job reference, service address if relevant, estimate number, issue date, and validity date when supplied. Ask what the customer is buying, which units the business bills, and the confirmed unit prices.
- Record one row per charge with its description, quantity, unit, and price per unit. Keep optional upgrades out of the accepted total until the customer selects them. Label illustrative numbers as examples.
- Keep the job's included work, exclusions, access or preparation requirements, and any assumptions in the scope. Use the actual service details. An AI scope draft can help organize them, and the user verifies that the described work can be delivered.

## Calculate and prepare the document

1. Multiply each quantity by its unit price and sum the line amounts in one currency. Subtract the confirmed discount. Apply any confirmed tax to the discounted amount under the owner's stated tax treatment. Mark tax as unconfirmed when the rate or applicability is unknown.
2. Include payment, deposit, and cancellation terms only as supplied. Keep timing conditional on access, materials, weather, or approval only where the owner gave that condition.
3. Return the estimate header, rows, subtotal and adjustments, total, and scope as separate blocks. Offer the online editor for a logo, paper size, and PDF preview. Replace all sample values before download.

## Browser workflow

When the page exposes browser actions, use `get_estimate` to inspect the current draft. Use `set_estimate_details` for confirmed header information, `set_estimate_prices` for line items, and `draft_estimate` for scope wording. Verify pricing and text separately before opening the PDF preview.

## Example

A customer requests two standard visits at $90 per visit and one oven add-on at $25. Subtotal is $205. A confirmed $10 discount gives $195 before tax. If tax is unresolved, display that status alongside the total and keep the oven add-on tied to the visit the user specifies.

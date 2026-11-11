---
name: invoice-generator
displayName: Invoice generator
description: >-
  Create an invoice with item quantities and rates, a discount, applicable
  tax, payments received, and balance due. Use to prepare a client invoice PDF
  in the billed currency with optional verified online payment details.
---

# Invoice generator

Use the [Invoice generator](https://doany.ai/tools/invoice-generator?utm_source=skills.sh&utm_medium=skill&utm_campaign=invoice-generator&utm_content=invoice-generator) to edit the live invoice, check its totals, and download a PDF in the chosen design and paper size.

## Gather billing details

Ask for seller and customer names and billing details, invoice number, issue and due dates, service date or reference, billed currency, and agreed terms. Get one line per item or service with quantity and rate. Confirm tax, discounts, and amounts actually received.

## Build the invoice

1. Multiply each quantity by the rate and round to the currency's minor unit. Sum the lines, apply the confirmed fixed or percentage discount, then apply any confirmed tax to the applicable base. Use the customer's agreed currency throughout.
2. Record a deposit or part payment in the amount-paid field. Subtract it once from the invoice total. If received money exceeds the total, flag the discrepancy for the owner.
3. Return the line items, subtotal, discount, tax, total, payment received, and balance due. Add due date, reference, and payment terms as supplied.
4. If the owner wants a payment link, have them verify the HTTPS URL against their own account and open it to confirm the destination. Check the QR and PDF in the preview before sharing. The owner handles sending and collection.

## Browser workflow

When the page exposes browser actions, use `get_invoice` to inspect the current draft and `update_invoice` to set confirmed invoice details. Review sample fields, actual received payments, and the balance in the preview before downloading.

## Example

An invoice with $600 of approved work and a $150 deposit already received shows $600 total and $450 balance due when there is no tax or discount. Keep the full work on its own line.

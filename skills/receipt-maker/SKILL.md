---
name: receipt-maker
displayName: Receipt maker
description: >-
  Prepare a printable receipt for an invoice payment, part payment, or
  completed sale. Use to record the payment date, method, amount received, and
  remaining balance with a verified reference.
---

# Receipt maker

Use the [Receipt maker](https://doany.ai/tools/receipt-maker?utm_source=skills.sh&utm_medium=skill&utm_campaign=receipt-maker&utm_content=receipt-maker) to preview the receipt and export a PDF or PNG of the recorded payment.

## Identify the payment type

- For an **invoice payment**, get the invoice number, balance immediately before payment, currency, and amount received. Use that balance as the starting line and avoid adding invoice tax again.
- For a **sale receipt**, list goods or services, quantities, rates, and any applicable confirmed tax.
- Get who paid and who received it, the paid date, method, and a permitted reference such as check number, transfer reference, or the card's last four digits. Keep full payment credentials out of the receipt.

## Calculate and verify

1. Subtract the amount actually received from the applicable total. If it was a part payment, display the remaining balance. Mark paid in full only when the payment covers the balance.
2. Check that the date and reference match the payment record. Return the receipt details and the remaining balance, then review the online preview before exporting.
3. Keep the document focused on a payment already received. Use the invoice for payment terms or future amounts due.

## Browser workflow

When the page exposes browser actions, use `get_receipt` to inspect the current receipt and `update_receipt` to apply confirmed payment details. Verify the date, amount, and remaining balance before exporting.

## Example

For an invoice with $500 still due before today's $200 bank transfer, the receipt shows $200 received and $300 remaining. Reference the original invoice and the permitted transfer identifier.

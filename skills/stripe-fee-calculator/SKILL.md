---
name: stripe-fee-calculator
displayName: Stripe fee calculator
description: >-
  Estimate Stripe processing fees or reverse-calculate what to charge for a
  target payout. Use for a payment or a batch of equal payments using the
  account country, currency, payment method, and standard or negotiated rates.
---

# Stripe fee calculator

Use the [Stripe fee calculator](https://doany.ai/tools/stripe-fee-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=stripe-fee-calculator&utm_content=stripe-fee-calculator) to select the account country, payment method, and fee direction, then inspect the rate breakdown and export the result.

## Identify the applicable rate

- Confirm the Stripe account country, transaction currency, payment method, amount, and number of equal-size payments. Ask about card origin, in-person or online payment, and currency conversion only when those details affect the selected rate.
- For standard pricing, read the currently applicable rate, fixed fee, cap or minimum, and relevant surcharges from the country/method breakdown. Use the owner's supplied rates for a negotiated plan. Keep the date and currency with the result.
- Use the smallest currency unit for rounding. Use the current provider rules for minimum and maximum payment amounts.

## Calculate in the requested direction

1. For **fee on a charge**, calculate the percentage fee for each payment, round it in that currency, add the fixed fee, and apply any applicable minimum or cap. Payout is charge less the fee.
2. For **what to charge**, find the smallest allowable gross amount with a net amount at or above the target. Recheck the final amount using the forward fee calculation.
3. For a batch, calculate each equal payment first and multiply its charge, fee, and payout by the count. For uneven payments, calculate them individually.
4. Return gross, fee, and payout per transaction and in total. List the included rate components. Treat Billing, Invoicing, disputes, and other separate costs as separate line items only when verified.

## Browser workflow

When the page exposes browser actions, use `get_stripe_fee` to read the active rate and its assumptions. Use `calculate_stripe_fee` to work out the charge or payout with the confirmed country, payment method, direction, and count. Check the per-payment breakdown before reporting the batch total.

## Example

With a user-supplied illustrative rate of 3% plus $0.25, a $100.00 charge costs $3.25 and pays out $96.75. Two such payments cost $6.50 altogether. Label the rate as an assumption for that example.

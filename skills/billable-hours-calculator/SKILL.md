---
name: billable-hours-calculator
displayName: Billable hours calculator
description: >-
  Total worked and billable minutes from time entries, breaks, overnight
  sessions, and hourly rates. Use to calculate invoice amounts, utilization,
  and client-approved billing increments while preserving actual time.
---

# Billable hours calculator

Use the [Billable hours calculator](https://doany.ai/tools/billable-hours-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=billable-hours-calculator&utm_content=billable-hours-calculator) to compare exact and rounded billing and export the reviewed entries for invoice preparation.

## Capture each time entry

Record a date or label, start and finish or an explicit duration, break minutes, billable status, and the rate that applies. Mark an overnight clock entry explicitly. Subtract only the break attached to that session and check that it fits inside the duration. Use the work log to resolve any overlap.

## Calculate actual and billed time

1. Keep time in minutes. Subtract the break from elapsed minutes. Sum actual worked time across all entries and actual billable time across the billable subset.
2. Use actual billable minutes for utilization, divided by total actual worked minutes. If there is no worked time, show utilization as unavailable. If the client agreement permits upward rounding, round each billable entry to the selected 6-, 10-, 12-, 15-, or 30-minute increment. Keep the before and after amounts visible.
3. Convert billed minutes to hours and multiply by the applicable rate, preserving the exact minute basis. Round each entry's amount to the currency's minor unit before summing. Report totals, utilization, and any rounding uplift. Review the log before entering the billed figures into an invoice.

## Browser workflow

When the page exposes browser actions, use `calculate_billable_hours` and `get_billable_hours` to confirm the recorded entries, actual utilization, selected billing increment, and amount to invoice.

## Example

09:00 to 12:30 with a 30-minute break gives three worked hours. A separate 61-minute billable entry rounds to 75 minutes under a 15-minute rule. At $80 per hour, that entry is billed at $100.

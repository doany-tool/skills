---
name: ctr-calculator
displayName: CTR calculator
description: >-
  Calculate click-through rate from clicks and impressions, or solve for
  clicks or impressions at a target rate. Use to compare ad creatives,
  campaigns, listings, or email click metrics with consistent denominators.
---

# CTR calculator

Use the [CTR calculator](https://doany.ai/tools/ctr-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=ctr-calculator&utm_content=ctr-calculator) to compare two scenarios and inspect the whole-count results for a target rate.

## Confirm the measurement

Get clicks and impressions for the same platform, time, and scope. Confirm which clicks count and whether the denominator is impressions, delivered emails, or another specifically labeled metric. For a combined report, sum clicks and impressions before dividing.

## Calculate the requested result

- **Measured CTR**. Divide clicks by positive impressions and multiply by 100. Flag clicks above impressions for investigation and check the platform definitions.
- **Clicks at a target CTR**. Multiply impressions by the rate as a fraction and round up for the minimum whole clicks to meet the target.
- **Impressions at an assumed rate**. Divide clicks by the positive rate as a fraction and round up to the next whole impression. If rounding changes the ratio, show the achieved CTR for the rounded counts.
- Return the numerator, denominator, rate, and any target assumption. Keep conversion and revenue comparisons separate.

## Browser workflow

When the page exposes browser actions, use `calculate_ctr` and `get_ctr` to confirm the active calculation direction and read back the rate and whole counts.

## Example

80 clicks from 4,000 impressions is 2% CTR. A 2.1% target across 4,010 impressions requires at least 85 clicks because 84.21 clicks is a planning result.

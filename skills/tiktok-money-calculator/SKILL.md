---
name: tiktok-money-calculator
displayName: TikTok money calculator
description: >-
  Estimate TikTok Creator Rewards from qualified views and RPM, add user-
  supplied brand deals, and work out the views needed for a rewards goal. Use
  to compare low and high monthly earnings assumptions.
---

# TikTok money calculator

Use the [TikTok money calculator](https://doany.ai/tools/tiktok-money-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=tiktok-money-calculator&utm_content=tiktok-money-calculator) to model Creator Rewards, add sponsorships, and compare program requirements with the numbers you enter.

## Confirm what counts

Get monthly views on eligible videos and the qualifying share, or use qualified views straight from the Creator Rewards dashboard. In the second case, count the supplied qualified views at 100%. Collect low and high RPM from the dashboard or label the rates as scenarios. Use the user's own brand deal count and rates for sponsored income.

## Calculate the range

1. Multiply eligible-video views by the qualifying share. Divide qualified views by 1,000 and multiply by each RPM. Calculate sponsorships separately and add other income only when the user supplies it.
2. For a positive rewards-only goal, multiply the target by 1,000 and divide by RPM to find qualified views. For eligible-video views, divide the same numerator by RPM × qualifying share. Round each result up once. At zero RPM, the goal cannot be reached in that scenario. At zero qualifying share, the eligible-video views required are unavailable.
3. Return monthly and annual estimates with the RPM and qualification assumptions. Verify current official country, account, and video requirements separately when asked about eligibility.

## Browser workflow

When the page exposes browser actions, use `estimate_tiktok_earnings` with the supplied views and RPM and `get_tiktok_estimate` to verify the qualified-view calculation and separate sponsorship amount.

## Example

At 500,000 eligible-video views and a 60% qualifying share, 300,000 views qualify. At $0.40–$1.00 RPM, estimated rewards are $120–$300 per month. Keep sponsorship fees in their own row.

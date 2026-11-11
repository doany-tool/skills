---
name: youtube-money-calculator
displayName: YouTube money calculator
description: >-
  Estimate YouTube monthly and annual earnings from long-form views, Shorts
  engaged views, and separate RPMs. Use to model low and high earnings,
  calculate views needed for a goal, or review Partner Program requirements.
---

# YouTube money calculator

Use the [YouTube money calculator](https://doany.ai/tools/youtube-money-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=youtube-money-calculator&utm_content=youtube-money-calculator) to enter channel metrics and compare RPM scenarios or check dated program thresholds.

## Gather the metrics

Use YouTube Studio data for the same recent period, with long-form views and Shorts engaged views separated. Collect separate revenue per thousand views for each format. A public lifetime average can provide broad context when the page offers it. Use Studio data for a specific recent month and format mix.

## Calculate the scenarios

1. Multiply each format's views by its own RPM and divide by 1,000. Sum the amounts. Use low and high RPM assumptions when the user is planning rather than reporting.
2. Add confirmed sponsorship, affiliate, or merchandise amounts that sit outside the RPM figure. Return monthly and annual estimates, with the annual figure assuming the same monthly run rate.
3. To find long-form views for a goal, subtract the modeled Shorts and other income from the goal. If those sources already cover the goal, zero additional views are needed. Otherwise multiply the remaining gap by 1,000 and divide by a positive long-form RPM, then round up. At zero RPM, a positive gap cannot be covered by long-form views. Show the views required from long-form alone when useful.
4. If asked about monetization, verify the current official rules for the country and date and compare the user's subscribers, eligible uploads, watch hours, and Shorts metrics as applicable. Mark eligibility as a threshold check. Channel approval is a separate review.

## Browser workflow

When the page exposes browser actions, use `estimate_youtube_earnings` with the supplied views and RPMs and `get_youtube_estimate` to verify the inputs. Check that any public channel average has not replaced the user's recent format-level data.

## Example

At 50,000 long-form views with $3 RPM and 200,000 Shorts engaged views with $0.08 RPM, the modeled platform revenue is $166 per month. Label both inputs and add any separate income only once.

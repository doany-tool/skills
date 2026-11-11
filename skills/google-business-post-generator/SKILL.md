---
name: google-business-post-generator
displayName: Google Business post generator
description: >-
  Draft a Google Business Profile Update, Offer, or Event with a confirmed
  action, dates, and applicable terms. Use for local announcements,
  appointment availability, time-limited deals, or events.
---

# Google Business post generator

Use the [Google Business post generator](https://doany.ai/tools/google-business-post-generator?utm_source=skills.sh&utm_medium=skill&utm_campaign=google-business-post-generator&utm_content=google-business-post-generator) to prepare an editable post packet for review in Google Business Profile.

## Choose the post type

| Type | Facts to gather |
| --- | --- |
| Update | The news, who it matters to, and a relevant action such as Book or Learn more |
| Offer | Title, start and end dates, business timezone, eligibility, redemption instructions, and any confirmed code or URL |
| Event | Title, start and end dates and times, timezone, location or attendance details, and the desired action |

## Produce the packet

1. Lead with the confirmed announcement, offer benefit, or event. State dates and eligibility where they affect the customer's decision. Ask for unclear details before drafting a time-sensitive packet.
2. Keep a linked action paired with its verified HTTPS destination. A Call now action uses the verified profile phone. For an Offer, use the platform's offer action and supply a redemption link only when available.
3. Return the selected type, editable post text, action, URL if used, and the fields the owner must enter separately. Include offer terms as a clearly labeled field and keep the copy consistent with them.
4. Compare dates, timezones, claims, and link destination with the user's input. Prepare the packet for the owner to review, schedule, or publish from their profile.

## Browser workflow

When the page exposes browser actions, use `draft_business_post` with the confirmed Update, Offer, or Event fields, then `get_business_post` to read the packet. Confirm that the type, dates, terms, and action survived the transfer.

## Example

For a Saturday bicycle tune-up clinic, gather the venue, start and end times, timezone, and whether booking is required. Draft an Event packet with a verified registration action and keep the time fields separate from the copy.

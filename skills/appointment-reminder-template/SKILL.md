---
name: appointment-reminder-template
displayName: Appointment reminder template
description: >-
  Write appointment reminder texts and emails for booking confirmation,
  preparation, arrival, rescheduling, missed visits, or recurring
  appointments. Use to turn confirmed booking details into copy-ready SMS and
  email.
---

# Appointment reminder template

Use the [Appointment reminder template](https://doany.ai/tools/appointment-reminder-template?utm_source=skills.sh&utm_medium=skill&utm_campaign=appointment-reminder-template&utm_content=appointment-reminder-template) to choose a booking stage and customize the message for the service.

## Pick the stage and collect the facts

- Confirm the customer name or placeholder, business, service, date, time or arrival window, timezone, and location or meeting instructions.
- Ask what the recipient needs at this stage. A confirmation includes booking details. A preparation reminder explains one or two tasks. An on-the-way message includes a confirmed ETA. A reschedule gives the new time and how to respond.
- Include the owner's verified change link, policy, access instructions, or preparation steps only when supplied. Keep sensitive appointment details out of ordinary text messages.

## Write the message

1. Draft a concise SMS with the business name, key booking detail, and one action. Use a single clear placeholder for each unfilled item.
2. If email is requested, add a subject and short body with date, time, and preparation on separate lines when useful. Add a reply or rescheduling instruction that matches the actual process.
3. Verify dates and links before sending. Give the owner copy-ready text for the selected stage. The owner sends it from their booking channel.

## Browser workflow

When the page exposes browser actions, use `write_appointment_reminder` with the selected stage and confirmed details, then read the assembled copy with `get_appointment_reminder` before returning it.

## Example

For a day-before grooming reminder, confirm the appointment time and pickup rules. The SMS can mention the time and one preparation step, while the email can also include parking and rescheduling details.

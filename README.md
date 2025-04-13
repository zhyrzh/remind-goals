# Remind Goals App

A web application for managing your goals and reminders in once place.

## Features

- Traditional authentication (email and password)
- Facebook authentication (only works on development mode since facebook app is not yet verified on developer's console)
- ADD, DELETE and EDIT [reminder](#reminder).
- ADD, DELETE and EDIT goal.
- Goal percentage tracking.

### Reminder

A reminder consists the following properties:

- **Title**
- **Frequency** - the interval in which the reminder should be sent to the user. Below are the list of all available frequncies with their description.
  - **ONCE** - This means that a reminder is only sent once.
  - **DAILY** - Reminder is sent to user's email DAILY at midnight and upon reminder creation.
  - **WEEKLY** - Reminder is sent WEEKLY at midnight during the day the reminder is created and upon reminder creation. So if a reminder is created on Monday it will be notified again next Monday.
  - **MONTHLY** - Reminder is sent MONTHLY (every 30 days) at midnight and upon reminder creation.
  - **ANNUALLY** - Reminder is sent ANNUALLY (every 365 days) at midnight and upon reminder creation.
- **Reminder date** - only available for "ONCE" frequency.

### Goal

A goal consists the following properties.

- **Title**
- [**Checklist**](#goal-cheklist-item) - A checklist cannot be empty for a goal.

### Goal Cheklist Item

An item that serves as the basis of a goal's progress.

- **Description**

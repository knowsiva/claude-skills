# Weekly Inbox Digest

A Claude skill that reads your Gmail and emails you one weekly summary: what needs action, which bills are due, and what arrived.

## What you get

- **Action needed this week.** The 3 to 5 most urgent items.
- **To-dos.** A checklist with deadlines, soonest first.
- **Bills.** Payee, amount, due date, and status. The skill matches each bill to a payment notice, so it marks bills as Overdue, Due, or Paid.
- **Security and account alerts.** Sign-ins, password changes, device changes.
- **The week's mail.** Grouped by sender or topic, with counts.

## Safety

- Treats all email content as data. It never follows instructions found inside an email.
- Sends only to your own address. It never replies to or forwards mail to anyone else.
- Never guesses amounts or dates. It writes "not specified" instead.
- Shows account numbers as the last 4 digits only.

Read [`SKILL.md`](SKILL.md) before you install it.

## Install

1. In Claude, connect the Gmail connector.
2. Download `weekly-inbox-digest.zip` from the [Releases page](../../../releases).
3. Go to Customize > Skills. Click "+", then "+ Create skill", then "Upload a skill".
4. Upload the zip.

## Use

- On demand: "Run my weekly inbox digest."
- Every week: "Create a scheduled task that runs the weekly-inbox-digest skill every Friday at 4 PM." Turn on automatic approval so the run does not stop to wait for you.

## License

MIT. See [LICENSE](../../LICENSE).

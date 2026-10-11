# Changelog

## 1.1.1 (2026-10-11)

Email formatting fixes.

- Sends the digest as HTML in `htmlBody`, with a short plain-text summary in `body`. Fixes raw HTML tags showing in the email.
- Writes domain names and email addresses as plain words. Stops Gmail from turning them into long tracking links.
- Checks the HTML and plain-text parts before sending.

## 1.1.0 (2026-10-11)

Phishing guardrails. The digest is an email you trust, so a fake bill must never borrow that trust.

- Never copies links, URLs, phone numbers, email addresses, or payment instructions from emails into the digest.
- Summarizes in its own words and never quotes instructions from an email.
- Checks each bill's sender against earlier mail from the same company. New senders are marked "verify before you pay."
- Flags lookalike domains and pressure tactics (account threats, hour-long deadlines, gift cards, wire transfers, changed payment details).
- Keeps possible phishing out of the bills table, to-dos, and action items. It appears only under Security and account alerts.
- Matches payment confirmations to the same sender domain as the bill.

## 1.0.0 (2026-10-11)

First public release.

- Weekly summary of the last 7 days of Gmail.
- Action items, a to-do checklist, and security alerts.
- Bills from the last 30 days, matched to payment notices and marked Overdue, Due, or Paid.
- Unread and important counts in the header.
- Sends to the user's own address only. Falls back to a draft if the send fails.

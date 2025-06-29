# Email to WhatsApp Notification Service
This Python project connects to your Gmail inbox, fetches unread emails, and sends notifications to a WhatsApp number using the Twilio API.

---

## Features

- Authenticate and connect securely to Gmail API
- Retrieve latest unread emails (up to 10)
- Extract sender, subject, timestamp, and a preview of the email body
- Send WhatsApp messages with email details using Twilio
- Automatically mark emails as read after notification
- Retry mechanism for Twilio message sending failures
- Scheduled periodic checking every minute (configurable)

---

## Requirements

- Python 3.7+
- Google API credentials (`credentials.json`)
- Twilio Account SID and Auth Token
- Twilio WhatsApp Sandbox enabled
- Required Python libraries: `google-auth`, `google-auth-oauthlib`, `google-api-python-client`, `twilio`, `schedule`


## Usage
The script will open a browser on the first run to authorize Gmail API access.

It checks for new unread emails every minute by default.

New email notifications are sent via WhatsApp.

Emails are marked as read after successful notification.

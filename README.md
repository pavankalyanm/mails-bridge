# Mails Bridge

Multi-account email access for Claude via IMAP/SMTP. Supports Gmail, Outlook, Yahoo, iCloud, and any provider with IMAP/SMTP access.

## Setup

1. Install this plugin in Claude
2. For each email account you want to connect:
   - Generate an App Password (Gmail, Outlook, Yahoo, iCloud each have their own process)
   - Tell Claude: `add my [alias] email [email] [app-password]`
   - The server auto-detects IMAP/SMTP servers for known providers

### Provider-specific setup

| Provider | App Password URL |
|----------|-----------------|
| Gmail | https://myaccount.google.com/apppasswords |
| Outlook/Hotmail | https://account.live.com/proofs/AppPassword |
| Yahoo | https://login.yahoo.com/account/security/app-passwords |
| iCloud | https://appleid.apple.com → Sign-In and Security → App-Specific Passwords |
| Zoho | https://accounts.zoho.com/home#security/security_apppassword |
| Fastmail | https://www.fastmail.com/settings/security/devicekeys |
| ProtonMail | Requires ProtonMail Bridge running locally |

For unlisted providers, pass custom IMAP/SMTP servers when adding the account.

## Supported actions

- **Search** emails across any account
- **Read** messages and threads
- **Send** emails and create drafts
- **Organize** — star, mark read/unread, move between folders
- **Multi-account** — manage and switch between unlimited email accounts
- **Multi-provider** — mix Gmail, Outlook, Yahoo, iCloud, and custom providers

## Example usage

- "Check my unread emails in the personal account"
- "Search for emails from Google in my work inbox"
- "Send an email from my outlook account to user@example.com"
- "Star that message"
- "Show me all my email accounts"
- "What providers are supported?"

## Requirements

- Python 3.11+
- [uv](https://docs.astral.sh/uv/) package manager

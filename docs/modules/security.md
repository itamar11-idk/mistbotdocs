# Global Security Network

The Security module is a collaborative defense system designed to protect all users and servers in the MistBot ecosystem from scammers and malicious actors.

## Key Features
- **Universal Blacklist**: A central database that prevents confirmed scammers from interacting with the bot.
- **Evidence-Based Reporting**: A secure way for users to report scams with proof.
- **Real-Time Security Alerts**: Servers can receive a live feed of confirmed scam events.

## Commands

### Prefix Commands
- `,report`: Starts a private, step-by-step interview in DMs to report a scammer.
- `,appeal`: Initiates an appeal process if you have been blacklisted and believe it was a mistake.

### Slash Commands (Admin/Dev)
- `/setscamfeed [channel]`: Configures a channel in your server to receive global security alerts.

## Security Flow
1. **Reporting**: Users submit reports with proof through a guided process.
2. **Review**: The global team reviews reports and takes appropriate action.
3. **Alerting**: Confirmed events are broadcast to the network to warn other communities.

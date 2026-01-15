# Market Module
The Mist-Market is a unified global trading hub that connects multiple servers into one searchable economy. It centralizes trade activity into a single command center, removing the need to manually monitor individual channels.

## Command Center Interaction
The primary interface is triggered by the `,market` command. This interactive embed serves as the main dashboard for all user activities.

### Core Features
* **Post Trade**: A manual entry system using Discord Modals to define "HAVE" and "WANT" items.
* **Search Marketplace**: A global query engine that filters the database for active sellers and buyers of specific items.
* **My Listings**: A personal management interface where users can bump active offers to the top of the feed or remove completed trades.
* **Notifications**: A system for setting keyword-based alerts that ping the user when specific items are listed.

## Automated Ghost Scraper
The Ghost Scraper functions as an entry assistant by monitoring trade channels across all connected servers.

1. **Extraction**: The bot identifies trade-related messages and parses item data using natural language processing.
2. **Verification**: The bot replies to the original message with an opt-in prompt.
3. **Database Sync**: Upon user confirmation, the data is automatically logged to the central database and mirrored to the global feed.

## Contact and Reputation
When a user initiates contact via the Search interface:
* The bot bridges the connection between the 2 traders.
* The system logs the interaction under "Successful Contacts," which serves as the primary metric for trade-specific reputation.

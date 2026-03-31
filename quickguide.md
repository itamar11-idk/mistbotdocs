# MistBot Quick Guide

This guide explains what the setup wizard does, and what each non-dev command is for.

## Start Setup

Run:

`/setup-mist`

The user running this command must have Administrator permission.

All 9 setup steps are optional. You can skip any step and configure that module later.

---

## Wizard Steps (What Each One Configures)

### 1) Welcome
- Introduces the setup flow.
- Confirms all steps are optional.

### 2) Essential Roles (Optional)
- Carrier Role: users who host carries and receive vouches.
- Manager Roles: staff roles allowed to use manager/admin workflow commands.

### 3) Vouch System (Optional)
- Vouch Channel: where vouch logs are posted.
- Vouch Cooldown Hours: delay between repeat vouches to reduce spam/farming.

### 4) Marketplace (Optional)
- Trade Channel: where trading should happen.
- Global Feed Subscription: enables global cross-server feed visibility.

### 5) Lobbies and Sessions (Optional)
- Lobby Category for temporary channels.
- LFG Channel for lobby recruitment.
- Free Carry Session Channel for hosted sessions.

### 6) Values Module (Optional)
- Values Channel where value checks are enabled.

### 7) Security (Optional)
- Scam Feed Channel for blacklist/scam alerts.

### 8) Other Settings (Optional)
- Staff Channel for internal moderation/staff-related messages.
- Prefix for prefix commands.

### 9) Review and Confirm
- Displays all selected settings.
- Confirm writes settings to config and activates features.

---

## Recommended Setup Patterns

### Minimal Carry Server
1. Run `/setup-mist`.
2. Set Carrier Role + Manager Roles.
3. Set Vouch Channel + cooldown.
4. Skip the rest.
5. Confirm.

### Full Trade Server
1. Run `/setup-mist`.
2. Set Trade Channel.
3. Set Values Channel.
4. Set Scam Feed Channel.
5. Confirm.

### Lobby-Focused Server
1. Run `/setup-mist`.
2. Configure Lobby Category + LFG + Free Carry Session channel.
3. Confirm.

---

## Command Guide (Expanded)

## Setup

### `/setup-mist`
- Starts the interactive 9-step setup wizard.
- Use this first in a new server.

---

## Help

### `/help`
- Shows the main help menu (slash version).

### `,help`
- Shows the main help menu (prefix version).

---

## General

### `/leaderboard`
- Shows the vouch leaderboard for carriers in the server.
- Use this for quick ranking visibility.

### `/ping-free-carry`
- Pings the configured host/carrier role.
- Useful when you need to quickly notify available carriers.

### `/ping` and `,ping`
- Checks bot latency and responsiveness.
- Use this when users think the bot is lagging.

### `/servers` and `,servers`
- Lists servers the bot is currently in.

### `/lbservers` and `,lbservers`
- Shows a server-vs-server vouch activity leaderboard.

### `/secret` and `,secret`
- Fun/novelty command.

### `/profile` and `,profile`
- Shows a carrier profile card/stat summary.
- Good for checking individual performance history.

---

## Admin and Managers

### `/set-prefix`
- Changes the server prefix for prefix commands.
- Example: switch from `,` to `!`.

### `/managers add`
- Adds a role to manager roles.
- Members with this role can use manager-level tools.

### `/managers remove`
- Removes a role from manager roles.

### `/managers list`
- Displays the currently configured manager roles.

### `/addvouch`
- Adds one vouch manually to a carrier for a carry type.
- Use for manual corrections.

### `/massadd`
- Adds multiple vouches at once for a carrier/carry type.
- Use for bulk correction/import scenarios.

### `/remvouch`
- Removes one vouch from a specific carry type.
- Use when an incorrect vouch was added.

### `/resettype`
- Resets all vouches for one carry type for one carrier.

### `/resetuser`
- Resets all vouches for a carrier across all types.
- High-impact action; use carefully.

---

## Marketplace

### `,market`
- Opens/starts the trading hub flow.
- Entry point for market users.

### `,post`
- Creates a new marketplace listing.
- Typical use: "I have X, looking for Y".

### `,lf`
- Searches listings/buyers for an item.
- Use to find demand or matching offers.

### `/settradechannel`
- Sets the designated marketplace channel.
- Restricts market usage to one place.

### `/disable-tradechannel`
- Disables trade channel enforcement/setting.

### `/set-feed`
- Sets the channel that receives global marketplace feed posts.

---

## Lobbies

### `,lfg`
- Creates or starts a "looking for group" lobby flow.

### `,host`
- Starts hosting a carry/session lobby.

### `,lobbies`
- Lists active lobbies.

### `,leave`
- Lets a user leave their current lobby.

### `,close`
- Closes a lobby.

### `,code`
- Used in lobby/session workflow for code sharing/updating.

### `/setup-lobbies`
- Initializes lobby infrastructure (category/channels workflow support).

### `/setlfgchannel`
- Sets the dedicated LFG command channel.

### `/setfreecarrychannel`
- Sets the free-carry session channel.

### `/close-lobby`
- Slash command version to close a lobby (including staff override flow).

---

## Values

### `/enable-values`
- Enables values command usage in a selected channel.

### `/disable-values`
- Disables values module for the server.

### `,reload`
- Reloads the values cache.
- Use this after values source updates.

---

## Security

### `/blacklistcheck`
- Checks whether a user is blacklisted and why.

### `,report`
- Submits a report/scam-related report flow.

### `/setscamfeed`
- Sets the staff alert channel for scam/blacklist notifications.

### `,appeal`
- Starts appeal flow for affected users.

---

## AI

### `,ask`
- Sends a question to Mist AI assistant.
- Use for gameplay/help knowledge queries.

---

## Promotion Reminder

### `/promotionping`
- Enables promotion reminder pings for the server.

### `/disablepromoterping`
- Disables promotion reminder pings.

### `/howmuchtimeleft`
- Shows remaining time until the next reminder.

---

## Quick Troubleshooting

- Command not showing:
Wait for slash sync and verify bot has application command permissions.

- Manager command denied:
Run `/managers list` and verify your role is included.

- Values not responding:
Run `/enable-values` again and confirm you are in that channel.

- Market commands not working:
Confirm `/settradechannel` is configured correctly.

- Lobby commands failing:
Confirm lobby category and channels are configured and visible to users.

- AI command not answering:
Check bot status and whether AI module is active in your deployment.

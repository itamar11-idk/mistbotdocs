# MistBot Quick Guide

This guide explains the setup wizard, what each step configures, and the non-dev commands your staff and users will use daily.

## Start Setup

Use:

`/setup-mist`

You need Administrator permissions.(the one uses the command , NOT THE BOT)

All 9 setup steps are optional. You can skip any step and configure later.

---

## Wizard Steps

### 1) Welcome
- Intro to the setup flow.
- Confirms that all steps are optional.

### 2) Essential Roles (Optional)
- Carrier Role: users who host carries and receive vouches.
- Manager Roles: trusted roles for management commands.

### 3) Vouch System (Optional)
- Vouch Channel: where vouch actions are logged.
- Vouch Cooldown Hours: anti-spam delay between vouches.

### 4) Marketplace (Optional)
- Trade Channel: where trading commands and posts should happen.
- Global Feed Subscription: allows global marketplace feed participation.

### 5) Lobbies and Sessions (Optional)
- Lobby Category.
- LFG Channel.
- Free Carry Session Channel.

### 6) Values Module (Optional)
- Values Channel where value checks are active.

### 7) Security (Optional)
- Scam Feed Channel for scam/blacklist alerts.

### 8) Other Settings (Optional)
- Staff Channel.
- Bot Prefix.

### 9) Review and Confirm
- Shows selected roles/channels/settings.
- Click confirm to apply.

---

## Common Setup Example

Minimal carry server:

1. Run `/setup-mist`.
2. Set Carrier Role and Manager Roles.
3. Set Vouch Channel and cooldown.
4. Skip marketplace/lobbies/values/security if not needed.
5. Confirm.

Full trade server:

1. Run `/setup-mist`.
2. Set Trade Channel.
3. Set Values Channel.
4. Set Scam Feed Channel.
5. Confirm.

---

## Command Reference

### Setup
- `/setup-mist`

### Help
- `/help`
- `,help`

### General
- `/leaderboard`
- `/ping-free-carry`
- `/ping`
- `,ping`
- `/servers`
- `,servers`
- `/lbservers`
- `,lbservers`
- `/secret`
- `,secret`
- `/profile`
- `,profile`

### Admin and Managers
- `/set-prefix`
- `/managers add`
- `/managers remove`
- `/managers list`
- `/addvouch`
- `/massadd`
- `/remvouch`
- `/resettype`
- `/resetuser`

### Marketplace
- `,market`
- `,post`
- `,lf`
- `,listings`
- `/settradechannel`
- `/disable-tradechannel`
- `/set-feed`

### Lobbies
- `,lfg`
- `,host`
- `,lobbies`
- `,leave`
- `,close`
- `,code`
- `/setup-lobbies`
- `/setlfgchannel`
- `/setfreecarrychannel`
- `/close-lobby`

### Values
- `/enable-values`
- `/disable-values`
- `,reload`

### Security
- `/blacklistcheck`
- `,report`
- `/setscamfeed`
- `,appeal`

### AI
- `,ask`

### Promotion Reminder
- `/promotionping`
- `/disablepromoterping`
- `/howmuchtimeleft`

---

## Quick Troubleshooting

- Command not showing: check permissions and wait for slash sync.
- Manager command denied: verify manager roles with `/managers list`.
- Values not responding: confirm `/enable-values` channel is set.
- Market command issues: confirm trade channel is configured.
- Lobby issues: confirm lobby category and channels are set.

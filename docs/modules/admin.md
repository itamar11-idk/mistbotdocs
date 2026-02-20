# Administrative Tools

The Administrative module provides server owners and staff with the tools necessary to manage the bot's behavior and user reputations within their community.

## Key Features
- **Staff Designation**: Assign specific roles within your server to manage bot settings.
- **Command Customization**: Change the bot's prefix to fit your server's needs.
- **Reputation Management**: Tools for staff to adjust and monitor user vouches manually.

## Commands

### Slash Commands
## Admin Commands
- `/addmanager [role]`: Registers a role as a bot manager, allowing its members to use administrative bot commands.
- `/removemanager [role]`: Removes a role from the bot manager list.
- `/setprefix [prefix]`: Updates the bot's command prefix for your server.

## Staff
- `/addvouch [user] [amount]`: Manually adds a specific number of vouches to a user's profile.
- `/removevouch [user] [amount]`: Manually removes a specific number of vouches from a user's profile.
- `/resetvouches [user]`: Completely resets a user's vouch count to zero.

## Permissions
- Most administrative features are restricted to users with Server Administrator permissions or designated staff roles.

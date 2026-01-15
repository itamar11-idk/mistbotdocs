# Vouching System
The vouching system is a reputation engine specifically designed for service carriers (Raids, Missions, etc.). It provides a verified track record for users providing assistance within the community.

## How to Vouch
After a service is completed, the client initiates a vouch for the carrier.

1. **Initiation**: Type `,vouch @carrier` or use `/vouch @user`.
2. **Selection**: The bot will respond with an interactive embed containing buttons for various service categories:
    * Fee Carry
    * Raids Carry
    * Warbringer Carry
    * Serum Carry
    * Myth Carry
3. **Confirmation**: Once a service type is selected, the carrier receives +1 vouch to their profile for that specific category.

## User Commands
These commands allow any member to interact with the reputation data.

| Command | Description |
| :--- | :--- |
| `,profile @user` | Displays the full breakdown of a carrier's vouches by category. |
| `,leaderboard` | Shows the top 10 all-time carriers within the current server. |
| `,monthlylb` | Displays the top carriers based on activity within the current month. |
| `/lbservers` | A global metric showing top servers ranked by vouch-to-member ratio. |
| `/serverstats` | Displays the total cumulative vouches across the entire server. |

## Administrative Commands
Restricted to staff members for maintaining database integrity.

### Modification
* `/addvouch @user`: Manually adds a single vouch.
* `/remvouch @user`: Removes a single vouch.
* `/massadd @user [count]`: Adds a specific number of vouches to a profile.

### Reset Functions
* `/resettype @user [type]`: Clears all vouches from a specific category (e.g., Missions) for a user.
* `/resetuser @user`: Permanently wipes all vouch data for the specified user.

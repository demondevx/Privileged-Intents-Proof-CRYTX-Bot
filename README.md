# 📜 Privileged Intents Proof – CRYTX Bot
Hello Discord Team,
This document provides detailed proof of why CRYTX requires the Server Members Intent, Presence Intent, and Message Content Intent. Each section includes a description of the bot features that rely on the intent, along with demonstration videos/screenshots.


## IMPORTANT NOTE FOR REVIEWER:
- Our main bot, Crytx, is currently in over 280 servers. Due to Discord’s restrictions, we cannot enable privileged intents on the main bot before verification.
- To demonstrate the functionality and necessity of these intents, we created a beta bot in a smaller number of servers, where all features using privileged intents are fully functional.
- The beta bot allowed us to test and produce proof for features that require the following intents: GUILD_MEMBERS, GUILD_PRESENCES, and MESSAGE_CONTENT.
- In our main bot, these features are disabled until we receive verification. All proofs submitted are taken from the beta bot demonstrating the exact features we plan to enable in the main bot after verification. 
- In the main bot, features that require these privileged intents are disabled. We have added an embed labeled “Feature Disabled” on these features to indicate they are inactive, and we have included proofs of this in the application.
- This approach ensures user privacy and compliance while proving the necessity of privileged intents for the core functionality of the bot.


## Server Members Intent
Required for:
- Join/Leave message syste
- Autorole system
- Anti-Raid detection & rollback
- Logging member join/leave events
- User information commands

Proof Videos and screenshots:
- [🎥 Video 1 – Member Join + Welcome Message + Logs + Autorole](https://youtube.com/shorts/cGn00ZP3WAs?feature=share)
-   [📷 Autorole Status](https://imgur.com/a/6v2IdwQ)
-   [📷 Logs Status](https://imgur.com/a/esG7wHN)
- [🎥 Video 2 – Anti-Raid Detection](https://youtube.com/shorts/TKQJd1LkqBI?feature=share)
-   [📷 Antilink Status](https://imgur.com/a/mJog8DI)
- [🎥 Video 3 – Anti-Link tied to Member Join](https://youtube.com/shorts/SfYPCbvUGhc?feature=share)
-   [📷 Antiraid Status When Inactive](https://imgur.com/a/j3nne0j)
-   [📷 Antiraid Status When Active](https://imgur.com/a/v7dg2PH)
- [📷/userinfo command showing member details](https://imgur.com/a/pZiWnzU)
- [📷/serverinfo command showing server details](https://imgur.com/a/tHhW8Bc)
- [📷 Main Bot Joining Functionality While Intents Are Disabled From Discord](https://imgur.com/a/XHCSkBg)
- [📷 Main Bot Antilink Functionality While Intents Are Disabled From Discord](https://imgur.com/a/iGJaER3)

## Presence Intent
Required for:
- /activity command (shows member status: Online, Idle, DND, playing games, listening to Spotify, etc.)
- /status command (tracks presence changes)

Proof Screenshots:
- [📷/activity showing presence & status change](https://imgur.com/a/Un1Pbgj)
- [📷/status tracking presence updates](https://imgur.com/a/QVjqYs5)

## Message Content Intent
Required for:
- Anti-Link system (detecting & blocking unwanted links in messages)
- Moderation filters (blocked domains, allowed domains, ignored roles)
- Fun commands that parse message inputs

Proof Videos and screenshots:
- [🎥 Video 4 – Anti-Link deletes blocked link + logs attempt](https://youtube.com/shorts/SfYPCbvUGhc?feature=share)
-   [📷 Antilink Allowed Domain List](https://imgur.com/a/hcGX0H2)
-   [📷 Antilink Allowed Domain Add](https://imgur.com/a/ask9wVC)
-   [📷 Antilink Ignore role add](https://imgur.com/a/u1qKyxF)
-   [📷 Antilink Ignore Role List](https://imgur.com/a/d2v9McS)
- [📷 Fun command /8ball showing message content usage](https://imgur.com/a/EXRLQlq)
- [📷 Message State Update Logs](https://imgur.com/a/xHN4v45)


##  🔒 Data Storage & Privacy

- The bot stores only minimal non-sensitive data (user IDs, role IDs, guild IDs, and configuration settings) using MongoDB (Mongoose).
- No usernames, nicknames, or avatars are permanently stored.
- Data retention: kept only as long as needed for bot functionality.
- Users can request data deletion anytime via the `/policy` command or support server.
- MongoDB is secured with authentication and encryption at rest.

## 📞 Contact
- Support Server: [SUPPORT_SERVER_LINK](https://discord.gg/nrQsWJ3kb5)
- Privacy Policy: [PRIVACY_POLICY_LINK](https://github.com/demondevx/Crytx/blob/main/PRIVACY_POLICE.md)
- Developer Contact: [Discord ID](https://discord.com/users/555652788592443392)

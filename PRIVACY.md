# Privacy notice

This notice describes how Minecraft Discord Status Bot handles information when it is installed on a private Discord server. It is not a legal finding that GDPR applies, and it is not a claim of GDPR certification or compliance.

A named privacy contact for the operator has not been published yet. Until that is added, this notice is not final. You can still use the Discord server where the bot is installed to ask the server operators about privacy.

## Purpose

The bot shows Minecraft server availability and an aggregate player count in Discord activity and through `/serverstatus`. No other secondary use is implemented.

## Minecraft data the bot processes

From Minecraft Java Server List Ping, the bot keeps only:

- whether the server answered
- current player count and maximum capacity
- a numeric Minecraft version, when present
- technical response time
- time of the last check

These values are held in memory and replaced by the next check.

## Information sent to Discord

The bot sends:

- activity text with a display name, aggregate player count, and online/offline/checking state
- `/serverstatus` replies with the same aggregates, version, latency, and last-checked time
- the Discord protocol data required for the bot to stay connected and to answer slash commands

Minecraft player names, UUIDs, and the Minecraft server address are not included in those Discord messages.

## Data the bot does not collect or store

The bot is not intended to collect or store:

- Minecraft usernames
- Minecraft UUIDs
- player IP addresses
- chat
- join/leave history
- playtime or other per-player history
- links between Minecraft accounts and Discord accounts
- Discord member lists or message history

A very small player count (for example `1/20`) can still suggest who is online in a small private group.

## Discord interaction metadata

When someone uses `/serverstatus`, Discord delivers interaction metadata so the bot can reply. The reply is ephemeral (visible only to the person who ran the command). The bot does not keep a local history of those interactions. Discord processes its own protocol and account data under Discord's terms.

## Storage, third parties, and deletion

- Status values are kept in process memory and disappear when the bot stops.
- There is no database of player history.
- There is no third-party Minecraft status API, analytics, or telemetry service.
- Discord, Inc. receives the bot traffic described above.
- Operator logs, if any, are for running the bot and are not a player profile. When the bot is uninstalled, local status data is gone with the process.

## Contact

Ask the operators of the Discord server where this bot is installed. A public name and email for a privacy contact have not been published in this repository.

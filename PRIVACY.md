# Privacy Policy

This policy describes how Minecraft Discord Status Bot handles information when it runs on a private Discord server. It is not a legal finding that GDPR applies, and it is not a claim of GDPR certification or compliance.

A named privacy contact has not been published yet. Until that is added, this policy is not final. You can still ask the operators of the Discord server where the bot is installed.

Effective date: 2026-10-25.

## What the bot processes

The bot is built to use as little personal data as possible.

From Minecraft Java Server List Ping it keeps only aggregated technical facts in memory:

- whether the server answered
- current player count and maximum capacity
- a numeric Minecraft version, when present
- technical response time
- time of the last check

These values are overwritten by the next check. They are not stored as player history.

## Discord interaction metadata

When someone uses `/serverstatus`, Discord sends the bot the interaction data needed to reply. The reply is ephemeral (visible only to the person who ran the command). The bot does not keep a local history of those interactions. Discord processes its own account and protocol data under Discord's terms.

## What is shared with Discord

The bot sends Discord:

- activity text with a display name, aggregate player count, and online/offline/checking state
- `/serverstatus` replies with the same aggregates, version, latency, and last-checked time
- the protocol data required for the bot connection and slash commands

Minecraft player names, UUIDs, and the Minecraft server address are not included in those bot messages.

## What the bot does not intend to store

The bot is not intended to collect or store:

- Minecraft usernames
- Minecraft UUIDs
- player IP addresses
- chat
- join/leave logs
- playtime or other per-player history
- links between Minecraft accounts and Discord accounts
- Discord member lists or message history

A very small aggregate count (for example `1/20`) can still suggest who is online in a small private group.

## Storage and deletion

- Status values live in process memory and disappear when the bot stops.
- There is no database of player profiles or history.
- There is no third-party Minecraft status API, analytics, or telemetry service.
- If the bot is uninstalled, local in-memory status data is gone with the process.
- Discord may retain its own logs and metadata according to Discord's policies.

## Privacy rights

If data protection law applies to a particular installation, requests are handled by the operator of that Discord server and Minecraft server, not by this public documentation. The bot cannot produce a player name or UUID list because it does not keep one.

## Contact

Ask the operators of the Discord server where this bot is installed. A public name and email for privacy requests have not been published in this repository.

See also [Terms of Service](TERMS.md).

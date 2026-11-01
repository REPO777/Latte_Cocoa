# Privacy Policy

**Last updated:** 1 November 2026

This policy explains how **Latte** handles information when you use the Latte Discord application, its web dashboard, and its music features. Latte is operated as part of Latte Cocoa.

**Cocoa and any other companion bot are music-only.** They do not use the Server Members intent and do not run the welcome feature.


## What Latte does

Latte plays music in Discord voice channels through slash commands and a web player. A server administrator can also turn on an optional welcome feature. When that feature is enabled, Latte can:

- send a message, embed, or generated welcome card when a member joins;
- send an optional direct message to the new member;
- add or remove roles selected by the server, with an optional delay and a humans, bots, or everyone filter;
- announce when a member leaves;
- announce when a member is banned;
- thank a member when they boost the server.

The welcome feature does nothing until a member with the Manage Server permission chooses a channel and saves the configuration.

## Information we process

### Discord account and server information

- Server ID, channel ID, and role ID needed to run a command or deliver a configured message.
- For a join, leave, ban, or boost event: the affected member's user ID, username, and avatar. These are used only to build that message or card. They are not saved as a member profile.
- User ID and display name of a person who requests a song, creates a playlist, likes a song, or votes for the bot.
- Song title, artist, URL, duration, and artwork needed for playback, history, playlists, and liked songs.
- Voice-channel membership needed to join a channel and control playback. Latte does not request the Presence intent.
- Dashboard login uses Discord OAuth with the **identify** scope only. The session stores your Discord user ID, username, and avatar so the dashboard can recognize you. Latte does not request your email address, server list, or connected accounts.

### Information we store

- Music settings for a server, such as volume, DJ role, and 24/7 voice channel.
- Your playlists, liked songs, and song-play history.
- Welcome settings for a server, including the selected channel, message template, embed options, card options, direct-message text, and role IDs.
- The user ID of the administrator who last saved those welcome settings.
- A Last.fm username and session key, only if you choose to connect Last.fm.
- A vote record containing your user ID, the bot, the voting site, and the time of the vote.

Latte does **not** store a copy of a server's member list. Latte does **not** read the content of messages and does not request the Message Content intent.

## Why Latte uses the Server Members intent

Latte requests Discord's privileged Server Members intent only to receive member events after a server enables the welcome feature:

- **Guild Member Add:** identify the member who joined so Latte can send the configured welcome, optional direct message, and auto-role changes.
- **Guild Member Remove:** identify the member who left so Latte can send the configured goodbye message.
- **Guild Member Update:** detect when a member starts boosting the server and send the configured thank-you message.

Ban announcements use Discord's ban event and do not require this intent. Latte does not page through, export, or analyze a server's member list. Automatic role changes require the Manage Roles permission and can change only roles below Latte's highest role.

## How we use information

We use the information above to:

- play and control music;
- show your playlists, history, and dashboard pages;
- deliver welcome messages configured by a server administrator;
- prevent the same vote from being counted twice;
- protect the service from abuse and diagnose errors.

We do not sell personal information and we do not use it for advertising.

## Service providers

The following services process information only as needed to operate Latte:

- **Discord**, for the bot platform, login, and gateway events.
- **The audio node** used to search for and stream a requested track.
- **The database provider** that stores the settings, playlists, history, votes, and welcome configuration described above.
- **Last.fm**, only if you connect a Last.fm account.
- **Top.gg and Discord Bot List**, which receive bot statistics such as the number of servers and process vote notifications. They do not receive server member lists.

## Retention and deletion

Welcome settings remain until an administrator changes them. Removing Latte from a server stops welcome processing for that server. Playlists, liked songs, and playback history remain so those features continue to work. You can delete your own playlists and liked songs from the dashboard.

To request deletion of information tied to your Discord user ID, contact us through the support server listed below. We may retain a record for as long as needed to prevent abuse, resolve a security incident, or meet a legal obligation.

## Security

Dashboard access to welcome settings requires a Discord login and the Manage Server permission in that server. Bot tokens and other secrets are not published in this repository. No storage or transmission method is completely secure.

## Children

Latte is not directed at children under 13, and we do not knowingly collect personal information from children.

## Changes to this policy

We may update this policy when Latte's features change. The date at the top is the latest version. Continued use of Latte after an update means you accept the revised policy.

## Contact

Questions and deletion requests: [Latte Cocoa support server](https://discord.gg/MpBK2YVppY)

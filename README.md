# Stupid Lynx

Stupid Lynx is a friendly Discord bot built for moderation, community activities, server stats,
music, and casual AI conversation. It can handle the serious server-management work without
forgetting that Discord is supposed to be fun.

## Invite Stupid Lynx

Ready to let a lynx loose in your server?

[Invite Stupid Lynx through Top.gg](TBA)

After inviting the bot, use `/server setup`. You will get a private menu where you can choose the
features you want, skip the ones you do not need, select your moderator role, and optionally select
a verified-member role. Nothing is created until you review the choices and press **Accept**.

You can always configure individual features later. `/help user` shows the member command list,
while `/help moderator`, `/moderator help`, and `/moderation help` provide staff guidance.

> Commands that change server settings or moderate members require the configured moderator role,
> Manage Server, or another appropriate Discord permission.

## Moderation

### Getting set up

| Command | What it does |
| --- | --- |
| `/server setup` | Opens the guided setup menu. Pick several systems at once, review everything, then accept or cancel. |
| `/moderation-setup` | Selects the Discord role trusted to use Stupid Lynx's protected moderation tools. |
| `/configuration dashboard` | Gives staff a quick overview of which major features, roles, and channels are ready to use. |

### Everyday moderation

| Command | What it does |
| --- | --- |
| `/warn` | Publicly warns a member with a required reason and creates a moderation case. |
| `/kick` | Removes a member, records who handled it and why, and respects Discord's role hierarchy. |
| `/ban` | Bans a member with a required reason and can also remove up to seven days of their recent messages. |
| `/timeout` | Temporarily stops a member from interacting for a duration such as 30 minutes, 2 hours, or 7 days. |
| `/purge` | Deletes a required number of recent messages. Add matching text if you only want messages containing a particular word or phrase. |
| `/lockdown` | Starts an emergency lockdown by applying a one-hour slowmode, hiding message history from everyone, and pausing invites. |
| `/lockdown-end` | Ends the lockdown and restores the channel and invite settings saved when it began. |

### Cases and moderator notes

| Command | What it does |
| --- | --- |
| `/case history` | Shows a member's recent warnings, kicks, bans, timeouts, notes, purges, and other recorded actions. |
| `/case view` | Opens one case by its case number for the full details. |
| `/case search` | Searches cases by member, moderator, action type, or words in the reason and details. |
| `/mod-profile add-note` | Adds a private staff note to a member's moderation profile. |
| `/mod-profile view` | Shows a member's private notes and useful account information to moderators. |

### Logging and anti-spam

| Command | What it does |
| --- | --- |
| `/logging-setup` | Chooses what to log: message edits and deletions, profile changes, joins and leaves, voice activity, or everything together. Logging channels are private to moderators. |
| `/anti-spam setup` | Enables protection against message floods, repeated messages, and mass mentions with sensible default limits. |
| `/anti-spam disable` | Turns the anti-spam system off. |
| `/anti-spam status` | Shows the protection currently in place and its limits. |

### Tickets, prison, and appeals

| Command | What it does |
| --- | --- |
| `/ticket-setup` | Creates or repairs the help desk, ticket button, and private transcript channel, using the selected staff role. |
| `/ticket-close` | Closes the ticket you are in. A reason is required, and staff can choose whether to save a transcript. |
| `/prison setup` | Creates the Prisoner role, restricted Prison area, appeal button, and appeal transcript channel. |
| `/prison add` | Saves a member's eligible roles, removes them, and gives the member access only to the Prison area. A reason is required. |
| `/prison release` | Removes the Prisoner role and safely restores the member's saved roles and access. |
| `/appeal close` | Finishes an appeal with a required reason, optionally saves the transcript, and removes the appeal ticket. |

### Community trials

| Command | What it does |
| --- | --- |
| `/trial setup` | Creates the public trial area and the moderator-only archive. |
| `/trial start` | Opens a public discussion for a member and posts a pinned vote with Approve, Abstain, and Deny choices. |
| `/trial end` | Closes voting and posts the totals, each voter's choice, and the final decision. |
| `/trial archive` | Moves an ended trial into the private staff archive. |

## Community Engagement

### Rules, roles, and welcomes

| Command | What it does |
| --- | --- |
| `/rules` | Opens a modal for creating or editing the rules embed. It can include an **Accept the Rules** button that grants a verified role. |
| `/roles create-group` | Starts a new self-assignable role group with its own description. |
| `/roles add` | Creates a role and adds its name, colour, and Unicode or custom server emoji to a group. |
| `/roles edit` | Changes an existing reaction role's name, emoji, or colour. |
| `/roles delete` | Removes a reaction-role entry and its Discord role. |
| `/roles post` | Posts the role-group panel or refreshes its existing message without making a duplicate. |
| `/welcome-messages setup` | Chooses where new-member greetings appear and lets staff customize the message. Each greeting includes the member's level card. |
| `/welcome` | Posts the friendly Stupid Lynx feature introduction again for everyone to see. |
| `/welcome-banner set` | Changes the global banner used above the welcome guide. This is available only to the creator of Stupid Lynx. |

### Clans

| Command | What it does |
| --- | --- |
| `/clans add` | Adds a clan using an existing role, then sets its leader, emoji, and description and prepares its private space. |
| `/clans edit` | Opens an easy editing modal for a clan's emoji and formatted description. |
| `/clans set-leader` | Chooses a new displayed clan leader. If the leader leaves, the position is cleared automatically. |
| `/clans remove` | Removes a clan from the clan directory without deleting the underlying Discord role. |
| `/clans join` | Lets a member join one existing clan and receive its role. Members can belong to only one clan at a time. |
| `/clans leave` | Leaves the member's current clan and removes its role. |
| `/clans show` | Posts or displays the live clan directory with leaders, descriptions, member counts, and clickable member mentions. |

### Levels, profiles, and achievements

| Command | What it does |
| --- | --- |
| `/levels setup` | Creates or repairs the level-up, achievement, notification preference, and leaderboard channels. |
| `/levels achievements list` | Privately shows moderators the complete achievement catalogue, including secret achievements. |
| `/levels achievements clear` | Erases one member's earned badges without deleting their experience or progress counters. Eligible level badges return after their next message. |
| `/profile view` | Shows a member's level card. The optional achievements choice also lists their earned badges while keeping secret descriptions hidden. |
| `/profile edit` | Lets you edit the title and biography on your own level card. Nobody else can change it for you. |
| `/profile banner` | Uploads a custom background for your own level card. |
| `/profile progress` | Shows your progress toward achievements that are not secret. |
| `/custom-achievement create` | Creates a custom achievement with its own name, emoji, and description. |
| `/custom-achievement list` | Shows the custom achievements available in the server. |
| `/custom-achievement award` | Gives a custom achievement to a member and includes it on their level profile. |
| `/custom-achievement revoke` | Removes an awarded custom achievement without changing the member's experience. |
| `/custom-achievement delete` | Permanently removes a custom achievement and its awards. |

### Giveaways and starboard

| Command | What it does |
| --- | --- |
| `/giveaway setup` | Creates or repairs the read-only giveaway channel. |
| `/giveaway timezone` | Saves your timezone so scheduled giveaway dates are interpreted correctly. |
| `/giveaway create` | Creates a numbered draft. The end date and time are optional, the number of winners is configurable, and a modal collects the title and details. |
| `/giveaway edit` | Reopens the giveaway modal so its title and details can be updated before or after posting. |
| `/giveaway post` | Posts a numbered giveaway in the giveaway channel with Enter and Leave buttons. |
| `/giveaway end` | Ends a giveaway early or manually, chooses the winner or winners, announces them, and opens prize tickets. |
| `/giveaway help` | Gives a quick walkthrough of the complete giveaway process. |
| `/starboard` | Creates or selects the read-only starboard channel and chooses how many unique star reactions a post needs. |

### Suggestions, events, topics, and puzzles

| Command | What it does |
| --- | --- |
| `/suggestions setup` | Creates or selects a writable suggestions channel. |
| `/suggestions submit` | Opens a modal for sharing an idea, then posts it with voting buttons. |
| `/suggestions status` | Marks a suggestion as pending, planned, accepted, implemented, or denied. |
| `/event setup` | Creates or repairs the community events channel. |
| `/event create` | Posts an event with a localized start time and Going, Maybe, and Can't Attend buttons. |
| `/event attendees` | Shows the members who responded to an event and what they selected. |
| `/topic setup` | Creates or selects the channel for a daily conversation topic and saves its timezone. |
| `/topic post` | Posts a fresh conversation topic immediately instead of waiting for the daily post. |
| `/puzzle setup` | Creates or selects the daily-puzzle channel and saves its timezone. |
| `/puzzle answer` | Privately submits an answer to the current puzzle. The first correct answer is celebrated publicly. |

### Birthdays, holidays, and announcements

| Command | What it does |
| --- | --- |
| `/birthday setup` | Chooses or creates the channel where birthday messages will be posted. |
| `/birthday set` | Saves your birthday so Stupid Lynx can celebrate it in the chosen channel. |
| `/birthday clear` | Removes your saved birthday. |
| `/holidays setup` | Chooses an existing channel or creates one for world-holiday and monthly observance announcements. Selected channels stay writable; newly created ones are read-only. |
| `/announcement setup` | Creates or chooses the read-only channel used for scheduled announcements. |
| `/announcement schedule` | Schedules a one-time, daily, or weekly announcement using the chosen date, time, and timezone. |
| `/announcement list` | Shows the announcements currently waiting to be posted. |
| `/announcement cancel` | Cancels one scheduled announcement. |

### Music

You need to be in the same voice channel as Stupid Lynx to control playback. The bot leaves after
ten quiet minutes or when everyone leaves.

| Command | What it does |
| --- | --- |
| `/music channel` | Creates or repairs the read-only now-playing channel and the separate writable request channel. Only moderators can set this up. |
| `/music join` | Brings Stupid Lynx into your current voice channel. |
| `/music play` | Adds a YouTube song or playlist to the queue. |
| `/music shuffle` | Shuffles the tracks waiting in the queue. |
| `/music stop` | Stops playback and clears the queue. |
| `/music clear` | Clears upcoming tracks without interrupting the current song. |
| `/music leave` | Disconnects Stupid Lynx from voice. |

### Just for fun

| Command | What it does |
| --- | --- |
| `/would-you-rather` | Posts your own question or creates a random mature-but-server-safe one with two voting buttons. It can be used once per hour. |
| `/conversation-starter` | Creates a friendly topic when the chat could use a little spark. |
| `/joke` | Shares a fresh, server-safe joke. |
| `/meme` | Finds and posts a server-safe image meme while avoiding recently posted repeats. |
| `/8ball` | Gives your question the full Magic 8-Ball treatment. Results may be mysterious, dramatic, or suspiciously convenient. |

Stupid Lynx also recognizes successful DISBOARD and Bumply bumps. Bumpers receive the server's
bumper role, and the bot reminds that role when another bump is available.

## Statistics

### Live server statistics

| Command | What it does |
| --- | --- |
| `/server-stats` | Creates or repairs a Server Stats category with locked voice channels showing the member count. It can also show verified and unverified totals when a verified role is selected. |

The displayed totals refresh automatically. If a configured channel is deleted, rerunning the
command repairs the missing parts instead of creating a pile of duplicates.

### Weekly metrics

| Command | What it does |
| --- | --- |
| `/metrics setup` | Creates or repairs a moderator-only weekly-report channel inside Server Stats and begins collecting activity for reports. |
| `/metrics report` | Publicly posts a report using the most recent data collected so far, including a partial current week when appropriate. |

The automatic report is posted every Sunday at noon Central Time. It compares the latest week with
the previous one and ends with a monthly overview. Reports can include joins and leaves, new-member
retention, new and returning chatters, messages, top chatters, busiest times, reactions, polls,
voice activity, verification totals, commands, starboard posts, bumps, chatbot activity, web
searches, achievements, level-ups, moderation actions, prison activity, trials, and active or quiet
channels. Optional statistics simply stay out of the report when their related feature is not set up.

## Chatbot

When enabled, Stupid Lynx responds when someone mentions the bot or replies directly to one of its
messages. It does not jump into unrelated conversations. The chatbot can hold a casual conversation,
answer questions, examine shared images, search the web when asked, and find trustworthy sources
when a user specifically requests them. Responses in another language include a small English copy
or summary underneath.

The chatbot follows safety rules, refuses inappropriate searches, never runs code, and avoids
offering unrequested advice. Staff can turn it off or restrict individual members without affecting
their access to the rest of Stupid Lynx.

### Member chatbot commands

| Command | What it does |
| --- | --- |
| `/chatbot stop` | Ends the current conversation and keeps the chatbot silent in that channel for ten minutes. Ordinary uses of the word “stop” are interpreted from context. |
| `/chatbot remember` | Saves something you explicitly want the chatbot to remember. |
| `/chatbot memories` | Privately shows what the chatbot remembers about you. |
| `/chatbot forget` | Deletes one saved memory matching the text you provide. |
| `/chatbot forget-all` | Deletes all of your saved chatbot memories. |
| `/chatbot remind` | Creates a one-time reminder of up to 1,500 characters using natural timing such as “tomorrow.” |
| `/chatbot reminders` | Privately shows your pending reminders without assigning them public numbers. |
| `/chatbot cancel-reminder` | Cancels reminders matching the text you provide. |
| `/chatbot clear-reminders` | Cancels all of your pending reminders. |

### Moderator chatbot commands

| Command | What it does |
| --- | --- |
| `/chatbot enable` | Turns mention-and-reply chatbot conversations on. |
| `/chatbot disable` | Turns chatbot conversations off and ends active sessions. Fun commands such as jokes and conversation starters remain available. |
| `/chatbot security-status` | Privately summarizes recent chatbot safety interventions without exposing message contents. |
| `/chatbot blacklist` | Permanently blocks one member from AI conversations while leaving their normal bot commands available. |
| `/chatbot unblacklist` | Restores a member's chatbot access and clears their recent automatic safety strikes. |

Repeated serious safety violations can temporarily restrict chatbot access. Stupid Lynx warns a
member when their next unsafe message may trigger that restriction and shows the remaining time if
the temporary restriction is applied.

---

Need a refresher inside Discord? Use `/help user` for everyday commands or `/moderator help` for the
full staff handbook.

# Obsolescence Privacy Policy

**Effective date:** November 17, 2026

This policy explains what the Obsolescence Discord bot ("Obsolescence", "the bot") collects, why, where it's kept,
who it's shared with, and how to have it deleted. "We" and "us" mean the developer who runs this copy of the bot.
"You" means anyone in a Discord server where the bot is installed, including server owners and staff.

Obsolescence is self-hosted. It runs on its developer's own computer, not on a cloud service, and doesn't sell,
rent or advertise with anything it collects.

Questions or requests: **apex101legend@yahoo.com**

## 1. What the bot collects

The bot only sees what Discord sends it for the servers it's in. A server's administrators choose which features
are on. Many features below are off until they turn them on, so the bot usually collects much less than this list.

**Always, for every server:**

- **Discord IDs and names**: user, server, channel, role and message IDs, and the usernames or display names the
  bot shows in logs. These are needed to know who did what and where.
- **Moderation records**: warnings, timeouts, kicks, bans, notes, strikes and the reasons staff give. This includes
  actions the bot takes itself, such as auto-mod, and, if the server enables it, actions staff take directly in
  Discord.
- **Server settings**: which features are on, which channels and roles they use, and the rules staff write.

**Only if a server uses the feature:**

| Feature | What's kept |
|---|---|
| Auto-mod and filters | The text of a message that broke a rule, as evidence on its case |
| Message reports and appeals | The reported message's text and author, who reported it, and what an appealing member writes |
| Review queue | The text of a message flagged for staff to check |
| Server logs | Deleted and edited message text, held in memory for the last 5,000 messages (cleared on restart). It's only saved to disk if the server sets *Keep Message Text on This PC*, for at most 30 days |
| Member events | Joins, leaves, role changes and account age, used for welcome messages, verification and raid detection |
| Modmail and tickets | Messages a member sends to staff through the bot, relayed into a private thread in the server |
| Reminders | The reminder text and when it's due |
| Image blocklist | A short fingerprint (perceptual hash) of a blocked image, not the image itself |
| Analytics | Daily totals such as messages, joins and actions per server; no message content |
| Security snapshots | The server's channel and role layout, so it can be restored after an attack |

**If you use `/ask`:**

- Your question, plus a short note of what you're allowed to do in that channel, so the answer fits your
  permissions.
- How many questions you've asked and the estimated cost, for the server's usage limits.
- If you add your own AI provider key, the key itself. It's encrypted on the computer that runs the bot, and only
  its last four characters are ever shown.

**If you sign in to the dashboard with Discord** (server staff only): your Discord user ID, username and avatar,
through Discord's `identify` scope. They're used only to check which servers you moderate.

The bot doesn't collect email addresses, phone numbers, payment details, precise location or voice audio. It
doesn't read direct messages unless you send one to it for modmail.

## 2. How it's used

Only to run the features above:

- moderating servers: enforcing rules, keeping case history and handling appeals;
- logging what happens in a server for its staff;
- protecting servers from raids, scams and attacks;
- answering `/ask` questions;
- sending reminders and community messages.

We don't use your data for advertising or to build profiles of members. We don't use it to make decisions about
anything outside the server. We don't use message content to train AI models.

## 3. Who can see it

- **Server staff** see records for their own server, on the dashboard or in the channels they choose. Staff of one
  server can't see another server's data.
- **The developer** can see everything stored, because it's on their computer. It's only looked at to run, fix or
  support the bot, or to handle a request under section 6.
- **Members** are told when a moderation action is taken against them, if the server enables those messages, and
  can see their own appeals and reminders.

## 4. Who it's shared with

We don't sell your data or give it to data brokers or advertisers. It only leaves the computer that runs the bot in
these cases:

| Service | What's sent | Why |
|---|---|---|
| **Discord** | Messages, actions and replies | That's how the bot works ([Discord's Privacy Policy](https://discord.com/privacy)) |
| **Anthropic** (Claude) | Your `/ask` question and the note of what you're allowed to do. The bot doesn't add your name or ID, so only what you type is sent | To generate the answer ([Anthropic's Privacy Policy](https://www.anthropic.com/legal/privacy)) |
| **Your own AI provider** | The same, if you added your own key | You chose that provider |
| **Ollama** | `/ask` questions when it's the fallback, and messages sent to the review queue | It normally runs on the same computer, so nothing leaves it |
| **Healthchecks or a similar uptime service** | Only an "I'm still running" signal, if the developer sets one up. No user data | So the developer knows if the bot goes offline |
| **GitHub** | No user data | Checking for updates and downloading a public list of scam domains |

We may also disclose data if the law requires it, or to protect people from serious harm.

## 5. How long it's kept

| Data | Kept for |
|---|---|
| Message text in memory | Until the bot restarts, or until it's pushed out by newer messages (last 5,000) |
| Message text on disk | Off unless a server turns it on; then that server's setting, at most 30 days |
| Strikes | 31 days |
| Security events | The latest 500 per server |
| Security snapshots | The latest 7 per server |
| Moderation records: cases, notes, appeals, reports, review items and the mod log | Until server staff delete them, or until deleted on request (section 6) |
| AI usage records and your own AI key | Until you remove your key, or until deleted on request |
| Backups | The latest 7 automatic daily backups, on the developer's computer and optionally a second folder they choose. A deleted record is gone from automatic backups within 7 days. Backups made by hand are kept until the developer deletes them, and are included when we handle a deletion request |

If the bot is removed from a server, that server's data isn't deleted automatically. The server owner can ask for
it to be deleted.

## 6. Your choices and rights

- **Deleting your data.** Email **apex101legend@yahoo.com** with your Discord user ID and what you'd like removed,
  for one server or all of them. We'll confirm it's you through Discord, then delete it within 30 days.
  - This removes your cases, notes, strikes, appeals, reports about you, logged messages, tickets, reminders and AI
    usage, and takes you off reports you made. Where you acted as a server's staff, the record of what happened
    stays but no longer names you.
  - Moderation records are partly the server's: a server's staff decide what goes in them. We may ask them first.
    If you're banned from a server, we may keep that active ban (its reason and history, without evidence or
    appeals) so the ban still holds.
- **Removing your AI key.** You can do this yourself at any time with `/ai unlink`, which erases your stored key and model choice.
- **Server owners** can remove the bot at any time, and can ask for all of their server's data to be deleted. Data
  left behind by servers the bot is no longer in can be deleted in one step.
- **Your legal rights.** Depending on where you live (for example under the GDPR in Europe or the CCPA in
  California), you may have the right to access, correct, delete or get a copy of your data, or to object to how
  it's used. Use the contact above for any of these.
  - The legal basis is our legitimate interest in providing moderation, safety and community features that a
    server's administrators asked for.

## 7. Security

- The bot runs on one computer controlled by its developer.
- The bot token and AI keys are encrypted, and the dashboard password is stored only as a secure hash.
- The dashboard needs a password or a Discord login, and staff only see servers they moderate.
- Updates are only installed when they carry a valid signature.

No system is perfectly secure. If we learn that data was accessed without permission, we'll tell Discord and the
people affected, as Discord's Developer Policy requires.

## 8. Children

Discord requires users to be at least 13, or older where local law says so. Obsolescence isn't directed at
children under 13 and doesn't knowingly collect their data. If you believe it has, contact us and we'll delete it.

## 9. Changes

We'll update this page when the bot's data handling changes and change the effective date at the top. Significant
changes will be announced wherever the bot is supported.

## 10. Contact

**apex101legend@yahoo.com**

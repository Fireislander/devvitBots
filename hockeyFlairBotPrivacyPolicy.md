# Privacy Policy for Hockey Flair Bot (`hockeyflairbot`)

**Last Updated:** October 31, 2026

This Privacy Policy explains how the **Hockey Flair Bot** application ("we", "us", or "our"), operating as a Reddit Developer Platform (Devvit) application, collects, uses, and discloses information when you use our flair selection app on Reddit.

---

## 1. Information We Collect and Process

Hockey Flair Bot operates strictly within the Reddit ecosystem as an interactive Devvit Web application. We collect and process only the minimal data required to manage and synchronize community user flairs:

### a. Information You Provide and Reddit Account Data
- **Public Reddit Username and User ID:** Retrieved through Reddit's native Devvit authentication context when you interact with the application.
- **Flair Selections:** The team, league, variant, and emoji identifier (e.g., `:60101:`) you select or clear using the app.
- **Subreddit Name:** The subreddit where you are opening or interacting with the flair selector.

### b. Activity-Based Data (Companion Subreddits Only)
- If enabled by moderators of a companion subreddit (such as partner subreddits configured to automatically mirror user flairs from a primary community), the bot detects your public comment or post submissions on that subreddit solely to copy your existing flair from the primary subreddit.

### c. Information We Do NOT Collect
- We **do not** collect personal identification information (such as real names, email addresses, phone numbers, or physical addresses).
- We **do not** collect passwords or login credentials.
- We **do not** collect payment or financial details.
- We **do not** collect IP addresses, device fingerprints, or browser tracking cookies.

---

## 2. How We Use Information

The information collected is used exclusively for the following operational purposes:

1. **Setting User Flairs:** Applying your selected flair text and emoji to your Reddit account on the active subreddit using Reddit's official moderator API.
2. **Clearing User Flairs:** Removing your flair when you click the "Clear Flair" option.
3. **Cross-Subreddit Synchronization:** If enabled by community moderators, recording your flair update to an internal Redis changelog queue and writing updates to the subreddit's public wiki (`flair_sync`) so companion communities (e.g., `r/hockeymemes`) can reflect your flair.
4. **Moderator Audit Logging (Outgoing HTTP):** If a subreddit moderation team has configured an optional Discord webhook, an outgoing HTTP notification containing your Reddit username, subreddit name, and updated flair text is transmitted to the designated Discord channel for moderation records and abuse prevention.

---

## 3. Third-Party Services and External HTTP Requests

Hockey Flair Bot uses the Devvit `http` plugin strictly for the following external communication:

- **Discord Webhooks (`discord.com`, `discordapp.com`):** Used solely to send real-time flair change notifications to subreddit moderator servers if explicitly enabled in subreddit app settings. No sensitive or private Reddit data is transmitted.
- **Reddit Platform:** All flair assignments, wiki updates, and user authorizations are governed by [Reddit's Privacy Policy](https://www.reddit.com/policies/privacy-policy) and [Reddit's User Agreement](https://www.redditinc.com/policies/user-agreement).

We **do not** sell, rent, monetize, or trade your data with any third-party advertisers, brokers, or external entities.

---

## 4. Data Storage and Retention

- **Reddit Flairs:** User flairs are stored publicly on Reddit servers as standard Reddit user flairs.
- **Temporary Cache:** Internal Redis changelog queues are ephemeral and stored within Reddit's Devvit Redis instance, automatically pruned on scheduled flushes.
- **Subreddit Wiki Logs:** Wiki changelog entries are maintained on the respective subreddit's public wiki page for sync processing and moderator audit purposes.
- We do not operate independent external databases or tracking servers.

---

## 5. User Control and Data Deletion

You retain full control over your user flair at all times:
- **Removal via App:** You can remove your user flair immediately by launching the Hockey Flair Bot interface and selecting **"Clear Flair"**.
- **Removal via Reddit Settings:** You can edit or disable your user flair at any time through Reddit's native community flair settings.
- **Moderator Assistance:** You can contact the moderation team of the participating subreddit to have your flair cleared manually.

---

## 6. Children's Privacy

Hockey Flair Bot does not knowingly collect or solicit information from anyone under the age of 13 (or under the minimum age required by applicable law in your jurisdiction). Users must comply with Reddit's minimum age requirements to use Reddit and this application.

---

## 7. Changes to this Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in functionality, Reddit platform requirements, or applicable laws. Any updates will be posted to this repository with a revised "Last Updated" date.

---

## 8. Contact Information

If you have questions, feedback, or concerns regarding this Privacy Policy or your data, please open an issue on the project's GitHub repository or contact the moderation team of the subreddit where the application is installed.


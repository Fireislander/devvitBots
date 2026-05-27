# Terms and Conditions for nflgdtbot

**Effective Date:** May 27, 2026

Please read these Terms and Conditions ("Terms") carefully before installing, configuring, or interacting with **nflgdtbot** (the "Bot"), an automated assistant built on the Reddit Devvit platform designed to host and manage National Football League (NFL) Game Day Threads (GDT) and Post-Game Threads (PGT).

By installing the Bot in your subreddit, or interacting with threads created by the Bot, you agree to be bound by these Terms. If you do not agree to all terms, do not install or use the Bot.

---

## 1. Description of Service

The Bot is a free, automated moderation utility designed to:
*   Fetch public NFL schedules and live statistics.
*   Generate automated Game Day Threads (GDTs) and Post-Game Threads (PGTs) for a selected NFL team or the entire league.
*   Dynamically update thread bodies with scoreboard matrices, period linescores, scoring summaries, combined team leaders, and injury reports.
*   Perform automated moderator actions such as locking GDTs, pinning/stickying PGTs, setting suggested comment sorting to "NEW", and editing posts.
*   Optionally alert community Discord servers via webhook integrations.

---

## 2. Eligibility & Installation

*   **Subreddit Authorization:** You may only install and configure the Bot if you are an active moderator with full permissions in the target subreddit.
*   **Settings Configuration:** Subreddit moderators are solely responsible for entering correct settings, team shortcodes, webhook URLs, and activation details in the Devvit settings dashboard.
*   **Reddit Guidelines:** Your subreddit and its use of the Bot must comply at all times with the [Reddit User Agreement](https://www.redditinc.com/policies/user-agreement) and [Reddit Content Policy](https://www.redditinc.com/policies/content-policy).

---

## 3. Acceptable Use & Moderator Responsibility

*   **Thread Moderation:** The Bot is an automated post scheduler and editor. It **does not** moderate user behavior, filter comments, or enforce subreddit rules. Subreddit moderators retain full, sole responsibility for moderating user discussions and maintaining compliance with Reddit guidelines within GDTs and PGTs.
*   **Wiping Data:** Subreddit moderators can clear the Bot's operational memory at any time by selecting the **Debug: Clear Redis Data** option in their Subreddit Tools menu.
*   **Abuse Prevention:** Subreddit moderators must not use the Bot for spam, targeted harassment, advertising, or any activity that violates Reddit policies.

---

## 4. Limitation of Liability & Platform Disclaimers

*   **"As-Is" Service:** The Bot is provided on an "AS IS" and "AS AVAILABLE" basis, without warranties of any kind, either express or implied, including but not limited to the implied warranties of merchantability or fitness for a particular purpose.
*   **API Dependencies:** The Bot relies on the availability and accuracy of external API endpoints (specifically public ESPN statistics feeds) and Reddit's Devvit platform. The Bot developers are not liable for errors, inaccuracies, delays, missing data, or failures resulting from ESPN API downtime or Reddit API rate limits.
*   **Subreddit Administrative Actions:** The developers are not responsible for any administrative actions, suspensions, or restrictions imposed upon your subreddit or accounts by Reddit administrators due to the Bot's activity.

---

## 5. Termination

*   **By You:** You may stop using the Bot at any time by selecting **NONE** as the active team code, clearing Redis data, or uninstalling the Bot from your subreddit's App directory.
*   **By Us:** We reserve the right to modify, suspend, or discontinue the Bot's development or service at any time, with or without notice.

---

## 6. Governing Law & Platform Policies

These Terms shall be interpreted in accordance with the laws governing standard open-source software licenses, subject to the overarching terms, conditions, and developer policies set forth by Reddit, Inc.

---

## 7. Contact & Support

For issues, bug reports, feature requests, or inquiries regarding these Terms, please open a public ticket or submit an issue in the official source code repository.

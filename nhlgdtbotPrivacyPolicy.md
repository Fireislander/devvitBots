# Privacy Policy for nhlgdtbot

**Effective Date:** May 27, 2026

Welcome to **nhlgdtbot** (the "Bot"), an automated assistant built on the Reddit Devvit platform to manage National Hockey League (NHL) Game Day Threads (GDT) and Post-Game Threads (PGT) on Reddit. 

We respect your privacy and are committed to protecting it. This Privacy Policy describes how the Bot operates, the limited information it processes, and our commitment to data safety.

---

## 1. Information We Process

The Bot is designed as a utility tool for subreddit moderators to automate game-day discussions. It operates strictly within the boundaries of the Reddit platform and processes only the following technical information:

### A. Subreddit Configuration Data
To operate, the Bot requires configuration settings entered by subreddit moderators via the Devvit Settings panel. This includes:
*   **Selected NHL Team:** The team for which the bot should generate game threads.
*   **Custom Preferences:** Custom kickoff posting times, header/footer templates, and custom post text.
*   **Discord Webhook URL (Optional):** A webhook URL supplied by moderators to route game status updates to their community Discord server.
*   **Activation Phrase:** A secret phrase to verify the bot is authorized to run.

### B. Public Sports Data
The Bot fetches real-time scores, team stats, goals, penalties, linescore matrices, and historical series records from the public official NHL Web API (`https://api-web.nhle.com`). **No user data is ever sent to this service.**

### C. Reddit Subreddit Thread Metadata
The Bot uses Reddit's API to post game threads, edit thread bodies with updated stats, lock completed threads, sticky active threads, and link threads together. It processes and caches post IDs (`t3_...`) to track and update active discussions.

---

## 2. What We Do NOT Collect

*   **No Personal Identifying Information (PII):** The Bot does not collect, record, or store personal user information such as real names, email addresses, geographical locations, or IP addresses.
*   **No Reddit Account Credentials:** The Bot operates under Reddit's secure OAuth framework via Devvit. It does not have access to, nor does it collect, passwords or private account credentials.
*   **No User Communication Logs:** The Bot does not collect, monitor, or harvest user comments, private messages, or chat histories.

---

## 3. Data Storage & Security

All subreddit settings and active game-tracking metadata are stored natively within **Reddit's secure Devvit infrastructure** (using Reddit's Settings and Redis KV storage APIs). 

*   Data is stored on Reddit's servers and is subject to Reddit's overall security controls.
*   No database or external server is hosted or managed by the Bot developers to store subreddit or user data.
*   Subreddit moderators have full control and can wipe all Redis tracking data immediately using the **Debug: Clear Redis Data** tool in their Subreddit Tools panel.

---

## 4. Third-Party Services

Because the Bot is hosted on Reddit and interacts with external APIs, the following third-party privacy policies also apply:
*   **Reddit:** Subject to the [Reddit Privacy Policy](https://www.reddit.com/policies/privacy-policy).
*   **NHL API / NHL Edge:** Scoreboard stats and highlights are retrieved from official public endpoints. Subject to the [NHL Privacy Policy](https://www.nhl.com/info/privacy-policy).
*   **Discord:** If a moderator configures a Discord webhook, notifications are routed to Discord. Subject to the [Discord Privacy Policy](https://discord.com/privacy).

---

## 5. Changes to This Policy

We may update this Privacy Policy from time to time to reflect changes in our Bot operations or platform updates. Any updates will be posted directly to the Bot's official source repository or documentation pages.

---

## 6. Contact Us

If you have any questions or concerns regarding this Privacy Policy or the Bot's operations, please contact the subreddit moderators or open an issue on the Bot's official repository.

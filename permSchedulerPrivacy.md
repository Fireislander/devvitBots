# Privacy Policy — PermScheduler

**Effective Date:** November 24, 2026

PermScheduler ("the App") is a Reddit Developer Platform (Devvit) moderation utility that allows subreddit moderators to temporarily route newly submitted posts and/or comments to their subreddit's ModQueue for review.

## 1. Information the App Processes and Stores

### Stored Within Reddit (Devvit Redis & App Settings)
- **Active Queue Restriction State:** While a restriction is active on a subreddit, the App temporarily stores the selected content types (e.g., text posts, link posts, images, comments), start and end timestamps, internal Devvit scheduler job IDs, and the Reddit username of the moderator who started or last updated the restriction.
- **Moderator Configuration:** Subreddit moderators may optionally configure a Discord or Slack incoming webhook URL and an "ending soon" notification preference in the App's subreddit settings.

### Processed In-Memory Only (Not Stored)
- While a queue restriction is active, the App inspects incoming Reddit post and comment submission events (post/comment IDs and post-type flags such as text, link, image, gallery, video, poll, or crosspost) solely to determine whether to filter the submission into the subreddit's ModQueue.
- The App **does not** store post titles, post bodies, comment text, media, or regular user profile data.

## 2. External Data Sharing (Optional Webhooks)

The App only makes external HTTP requests if a subreddit moderator explicitly configures a Discord (`discord.com` / `discordapp.com`) or Slack (`hooks.slack.com`) incoming webhook URL in the subreddit's App settings.

When configured, webhook notifications include only:
- The subreddit name (`r/<subreddit>`)
- Event type (started, updated, ending soon, ended, or ended early)
- Selected content types being queued
- Scheduled end time (US Eastern Time)
- The Reddit username of the moderator who initiated, updated, or ended the restriction early

No post contents, comment contents, or non-moderator user data are ever sent to any external service. Data delivered to a configured Discord or Slack webhook is governed by Discord's or Slack's respective privacy policies.

## 3. Data Retention and Deletion

- Active restriction state is automatically deleted from Devvit Redis when the scheduled restriction ends or is ended early by a moderator.
- Moderators can remove their webhook URL at any time from the App's subreddit settings page, or uninstall the App from their subreddit to stop all processing.

## 4. Children's Privacy

The App operates exclusively within Reddit and is intended for subreddit moderators. It does not knowingly collect personal information from children under 13 (or the applicable minimum age in their jurisdiction).

## 5. Changes to This Policy

This Privacy Policy may be updated from time to time. Continued use of the App after updates are posted constitutes acceptance of the revised policy.

## 6. Contact

For questions or concerns about this Privacy Policy, please contact the App developer via Reddit or the App's GitHub repository.

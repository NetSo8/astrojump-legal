# Privacy Policy – AstroJump

**Last Updated:** October 2026

This Privacy Policy explains how **AstroJump** ("we", "our", or "the Game"), accessible via Discord Activities, collects, processes, and stores data when you play the game.

## 1. Information We Collect

### A. Data Retrieved via the Discord Embedded App SDK
To operate the game session within Discord, we retrieve:
- **Discord User ID (Snowflake):** Used as an immutable unique identifier to link your progression and save data.
- **Discord Username / Global Name:** Displayed inside the game interface and on the global leaderboards.
- **Discord Avatar (Hash / CDN URL):** Used strictly to render your profile picture in-game.
- **Channel ID & Guild ID:** Transmitted by Discord to initialize and maintain the multiplayer game session context.

**We do NOT collect:**
- Your private messages, text chat, emails, server roles/permissions, voice audio, or your friends list.

### B. Game Statistics & Server-Side Data
When playing, our backend server (`astrojump.wuuti.fr`) creates and stores:
- Internal account identifier (UUID) linked to your Discord User ID.
- Game metrics: High score, total jumps, planets explored, games played, and timestamp of the last session.
- Run validation records (start/end timestamps and final scores) strictly for anti-cheat verification and global leaderboard integrity.

### C. Server Logs & Network Information
- **IP Addresses:** We do not link IP addresses to player accounts or store them in our main database. Ephemeral server access logs (via our Caddy web server) temporarily retain incoming connection metadata exclusively for infrastructure security, rate limiting, and DDoS mitigation. These logs rotate and are purged automatically within 14 to 30 days.

## 2. Third-Party Services and Analytics
- **Analytics & Tracking:** We do not use third-party analytics services (such as Google Analytics, PostHog, or Mixpanel).
- **Crash Reporting:** We do not employ third-party crash reporting SDKs (such as Sentry or Datadog).
- **Advertising:** The game currently does not display third-party advertisements or integrate ad networks (such as Google AdMob). Should advertising SDKs be introduced in future updates, this policy will be updated prior to deployment to outline any relevant ad identifiers.
- **Data Sales:** We do not sell, rent, or trade personal data to third parties, brokers, or marketing networks.

## 3. Data Retention & Security
- Session authentication tokens (JWT) expire automatically after 12 hours.
- Account progression and leaderboard data are stored securely in our PostgreSQL database for as long as the game remains active, or until a player requests account deletion.

## 4. Your Rights (GDPR / Data Subject Rights)
Under applicable data protection regulations (including the GDPR), you have the right to access, rectify, or request the erasure of your personal data.

To request the complete deletion of your account, scores, and associated Discord identifiers from our database:
- Send an email to: **jeremy99981@gmail.com**
- Include your **Discord User ID** (Snowflake) in the request so we can locate and remove your record.

Requests are processed within 30 days.

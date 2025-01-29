# Senthamizh Roleplay Discord Bot

A custom Discord bot designed to enhance the Senthamizh Roleplay (STRP) community experience by automating processes, managing roles, streamlining events, and fostering engagement. Built with `discord.py` and tailored for Tamil roleplay communities.
![logo](strp_logo.png)

---

## ✨ Features

### Core Systems

- **Roleplay Support**:
  - Character registration, job systems, stats tracking, and whitelist management.
- **Moderation Tools**:
  - Auto-ban system, anti-spam, role-based permissions, and ban history logging.
- **Economy Integration**:
  - In-game currency management tied to Discord activity and roles.
- **Community Engagement**:
  - Leaderboards, reward systems, and interactive commands.

### Key Modules

1. **Announcement System**
   - Automated restart, VP, PD, and EMS announcements with dynamic embed updates.
2. **Application System**
   - Visa, PD/EMS, and NOC applications with automated logging and approval workflows.
3. **Auto Discord Name Changer**
   - Syncs in-game names to Discord profiles (e.g., `[STPD | Gipz Martin | Mr. Nobuddy]`).
4. **Ban System**
   - Role-based bans, auto-unban on expiry, and transparent ban logs.
5. **Community Management**
   - Create/edit gangs/teams, recruitment panels, and public leaderboards.
6. **Job Role Processing**
   - Whitelisted job assignments without granting Discord admin access.
7. **Leaderboards**
   - Track TDM stats, unpaid invoices, player activity, and more.
8. **Message Panel**
   - Dark messages, anonymous messaging, and cross-channel forwarding.
9. **Ticket System**
   - Customizable OOC, item loss, and premium tickets with automated transcripts.
10. **Visa Process System**
    - Auto-generate visa images, approve/reject applications, and notify users.

---

## 🛠️ Installation

### Prerequisites

- Python 3.10+
- Discord Bot Token ([Guide](https://discordpy.readthedocs.io/en/stable/discord.html))
- SQLite3 or PostgreSQL database

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/infinity-developers/Senthamizh-Roleplay-Official-Bot.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure the bot:
   - Rename `config.example.py` to `config.py`.
   - Update `config.py` with your bot token, guild ID, and database credentials.
4. Run the bot:
   ```bash
   python main.py
   ```

---

## ⚙️ Configuration

### `config.py` Setup

```python
BOT_TOKEN = "YOUR_DISCORD_BOT_TOKEN"
GUILD_ID = 952311103365451827  # Senthamizh Roleplay Server ID
DATABASE_URL = "sqlite:///database.db"  # Or PostgreSQL URL

# Customize role IDs, channel IDs, and prefixes
CIVILIAN_ROLE_ID = 123456789
BAN_LOG_CHANNEL_ID = 123456789
```

### Auto Name Changer

- Stores Discord IDs in the `users` table.
- Runs every 24 hours to avoid rate limits.

### Ticket System

- Customize ticket types and access controls in `tickets/config.json`.

---

## 🚀 Usage

### Commands

| Command                | Description                | Example                   |
| ---------------------- | -------------------------- | ------------------------- |
| `!apply visa`        | Submit a visa application  | `!apply visa`           |
| `!ban @user 7d spam` | Ban a user for 7 days      | `!ban @JohnDoe 7d spam` |
| `!leaderboard tdm`   | Display TDM stats          | `!leaderboard tdm`      |
| `!ticket create ooc` | Open an OOC support ticket | `!ticket create ooc`    |

### Visa Image Generation

- Upload a reference image with `!visa apply`, and the bot generates a formatted visa.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/amazing-feature`.
3. Commit changes: `git commit -m "Add amazing feature"`.
4. Push to the branch: `git push origin feature/amazing-feature`.
5. Open a pull request.

---

## 📜 License

This project is proprietary software developed for Senthamizh Roleplay. Unauthorized distribution is prohibited.

---

## 📞 Contact

- **Discord Server**: [Join Here](https://discord.gg/MGr2ZemqyE)

---

**Built with ❤️ by Infinity Development Alpha Team**

```

```

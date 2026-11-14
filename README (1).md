<div align="center">

```
 ███╗   ██╗██╗   ██╗ █████╗ ███╗   ██╗
 ████╗  ██║╚██╗ ██╔╝██╔══██╗████╗  ██║
 ██╔██╗ ██║ ╚████╔╝ ███████║██╔██╗ ██║
 ██║╚██╗██║  ╚██╔╝  ██╔══██║██║╚██╗██║
 ██║ ╚████║   ██║   ██║  ██║██║ ╚████║
 ╚═╝  ╚═══╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═══╝
 ███╗   ██╗██╗   ██╗██╗  ██╗███████╗
 ████╗  ██║██║   ██║██║ ██╔╝██╔════╝
 ██╔██╗ ██║██║   ██║█████╔╝ █████╗
 ██║╚██╗██║██║   ██║██╔═██╗ ██╔══╝
 ██║ ╚████║╚██████╔╝██║  ██╗███████╗
 ╚═╝  ╚═══╝ ╚═════╝ ╚═╝  ╚═╝╚══════╝
```

**A rainbow-terminal Discord server management tool**

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows%20%7C%20Termux-success?style=for-the-badge)
![Discord](https://img.shields.io/badge/Discord-API%20v10-5865F2?style=for-the-badge&logo=discord&logoColor=white)

</div>

---

> ⚠️ **Disclaimer** — This tool is for **educational purposes and use on your own servers only.**
> Self-bots violate [Discord's Terms of Service](https://discord.com/terms). Use on alt accounts at your own risk. The author takes no responsibility for account bans or misuse.

---

## Features

- 🌈 **RGB NYAN ASCII banner** — full 24-bit true-color terminal art
- 🔐 **Masked token input** — your token never echoes to the screen
- 📋 **Live server list** — lists every server your account is in
- ⚡ **Threaded operations** — webhook spam and mass ping run per-channel in parallel
- 📱 **Termux compatible** — runs on Android via Termux with zero extra setup

---

## Installation

### Standard (Linux / macOS / Windows)

```bash
git clone https://github.com/crimsonpardon/NyanCat
cd NyanCat
pip install requests colorama
python nyan_nuke.py
```

### Termux (Android)

```bash
pkg update && pkg install python git
git clone https://github.com/crimsonpardon/NyanCat
cd NyanCat
pip install requests colorama
python nyan_nuke.py
```

---

## Usage

On launch you will see:

```
❯ Paste token (hidden): 
```

Your token is masked — nothing is printed as you type.

### Server List Screen

```
  [1]  My Server
  [2]  Test Guild
  [3]  Dev Server

  [r] Refresh   [t] Change Token   [q] Quit
```

| Key | Action |
|-----|--------|
| `1`–`n` | Select a server |
| `r` | Refresh server list |
| `t` | Change / swap token |
| `q` | Quit |

### Action Menu

After selecting a server:

| Key | Action |
|-----|--------|
| `1` | Webhook Spam — creates a webhook in every text channel and spams it |
| `2` | Create Channels — bulk-create text channels |
| `3` | Delete Channels — delete every channel |
| `4` | Create Roles — bulk-create roles |
| `5` | Delete Roles — delete all non-managed roles |
| `6` | Ban Members — ban every member |
| `7` | Kick Members — kick every member |
| `8` | Unban All Members — lift all bans |
| `9` | Prune Inactive Members — prune by inactivity days |
| `A` | Customize Webhook Settings — set name, message, count |
| `B` | Leave Server |
| `M` | Mass Ping — 99× @everyone across every text channel (threaded) |
| `0` | ← Back to server list |

---

## Requirements

| Package | Purpose |
|---------|---------|
| `requests` | Discord REST API calls |
| `colorama` | Windows ANSI color compatibility |
| `getpass` | stdlib — masked token input |

Python 3.8 or higher required.

---

## Project Structure

```
NyanCat/
└── nyan_nuke.py   # single-file tool — everything in one place
```

---

## Contributing

Pull requests are welcome. Open an issue first for major changes.

---

<div align="center">
Made with 🌈 by <a href="https://github.com/crimsonpardon">crimsonpardon</a>
</div>

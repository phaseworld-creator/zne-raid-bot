<p align="center">
  <img src="https://avatars.githubusercontent.com/u/295873404?s=512" alt="ZNE Raid Bot Logo" width="180" height="180">
</p>

<h1 align="center">ZNE Raid Bot</h1>

<p align="center">
  <strong>An advanced, high-performance Discord utility and automation bot engineered with discord.py.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python&logoColor=white" alt="Python Version">
  <img src="https://img.shields.io/badge/discord.py-rewrite-5865F2?style=flat-square&logo=discord&logoColor=white" alt="Discord.py">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="License">
</p>

---

## 📖 Table of Contents
- [⚡ Core Features](#-core-features)
- [📁 Project Architecture](#-project-architecture)
- [🛠️ Installation & Setup](#️-installation--setup)
- [⚙️ Configuration](#️-configuration)
- [🚀 Execution](#-execution)
- [🧩 Tech Stack](#-tech-stack)
- [⚠️ Disclaimer](#️-disclaimer)

---

## ⚡ Core Features

| Feature | Description |
| :--- | :--- |
| **Rapid Raid** | High-speed execution engine for coordinated mass actions. |
| **Interaction Raid** | Burst-fire messaging arrays triggered via unified interface buttons. |
| **Advanced Spam** | Configurable loops for custom text payloads and file drops. |
| **Payload Utilities** | Specialized text and media delivery modules. |
| **Social Engineering** | Integrated fake Nitro generator hoaxes and automated giveaway tools. |
| **Stealth Tools** | Ghost ping and ghost mention frameworks for subtle tracking. |
| **DM Flood** | Automated direct message distribution pipelines. |
| **Outreach** | Scheduled and automated advertisement posting across channels. |
| **Leaderboards** | LMDB-backed high-performance tracking for active operators. |
| **Administration** | Hot-swappable cogs, dynamic global messaging, and granular blacklists. |

---

## 📁 Project Architecture

```text
ZNE-Raid-Bot/
├── cogs/               # Modular feature extensions
├── data/               # LMDB database storage
├── main.py             # Application entry point
├── config.example.toml # Template configuration file
├── requirements.txt    # Python dependencies
└── README.md           # Documentation

```

---

## 🛠️ Installation & Setup

### Prerequisites

* [Python 3.10 or higher](https://www.python.org/)
* Recommended: [uv](https://docs.astral.sh/uv/) for lightning-fast environment provisioning.

### Quick Start

```bash
# Clone the repository
git clone https://github.com/ZNE-Opensource-Project/zne-raid-bot.git](https://github.com/ZNE-Opensource-Project/zne-raid-bot.git ZNE/Raid
cd ZNE/Raid

# Set up environment using uv (Recommended)
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\Activate.ps1
uv pip install -r requirements.txt

# Fallback standard venv installation
# python -m venv .venv
# source .venv/bin/activate  # On Windows: .venv\Scripts\Activate.ps1
# pip install -r requirements.txt

```

---

## ⚙️ Configuration

Initialize your configuration file from the provided template:

```bash
cp config.example.toml config.toml

```

Populate `config.toml` with your operational parameters:

```toml
TOKEN = "your-bot-token-here"
owner_ids = [123456789012345678]

[server]
main_server = 0
verified_role_id = 0

[channels]
log_channel_id = 0

[messages]
og_msg = "your default payload message here"

[api]
# Optional: Required only if running the ZNE Website companion backend
url = "your-api-url"
secret = "your-api-secret"

```

---

## 🚀 Execution

Launch the application loop:

```bash
python main.py

```

---

## 🧩 Tech Stack

* **Core Wrapper:** [discord.py](https://discordpy.readthedocs.io/)
* **Storage Engine:** [LMDB](https://lmdb.readthedocs.io/) (Lightning Memory-Mapped Database) for ultra-fast leaderboard syncing.
* **Network Layer:** [aiohttp](https://docs.aiohttp.org/) for asynchronous API communication.

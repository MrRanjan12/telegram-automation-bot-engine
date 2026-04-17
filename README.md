# AutoResponse Engine

> A unified backend system that connects Telegram and Web interfaces through a single AI-powered service layer — built for real-time conversational workflows.



![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)




![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)




![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=flat&logo=telegram&logoColor=white)




![LLaMA3](https://img.shields.io/badge/LLaMA3-Groq-orange?style=flat)



---

## 🔗 Live Demo

| Interface | Link |
|-----------|------|
| 🌐 Web Client | [smartchattldr-ai.netlify.app](https://smartchattldr-ai.netlify.app/) |
| 🤖 Telegram Bot | [@SmartChatTLDR_AI_Bot](https://t.me/SmartChatTLDR_AI_Bot) |
| ⚙️ Backend API | [telegrambot-znt2.onrender.com](https://telegrambot-znt2.onrender.com) |

---

## Overview

This project explores how a **single backend** can coordinate multiple interaction channels while maintaining consistent logic, response generation, and state handling.

Built around an **event-driven architecture** — user inputs from Telegram and Web are normalized through a shared pipeline, processed by an LLM, and returned through their respective channels.

---

## Architecture

```
User Input → Interface Layer → bot.js → Processing Logic → LLaMA3 (Groq) → Response → Client
```

**File Structure**
```
├── bot.js              # Core logic — Telegram + Web handler
├── package.json        # Dependencies
└── .gitignore
```

---

## Core Features

- **Multi-interface handling** — Telegram bot + Web client, one backend
- **AI response generation** — LLaMA3 via Groq API
- **Command-based control flow** — summarization mode, mode switching
- **Per-user state tracking** — dynamic behavior per session

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Runtime | Node.js |
| Framework | Express.js |
| Telegram Interface | grammY |
| LLM Provider | Groq API (LLaMA3) |
| Frontend Hosting | Netlify |
| Backend Hosting | Render |

---

## Getting Started

```bash
git clone https://github.com/MrRanjan12/TelegramBot.git
cd TelegramBot
npm install
```

Create `.env` file:
```env
GROQ_API_KEY=your_key_here
PORT=3000
```

```bash
node bot.js
```

---

## What I Learned

- Designing a unified backend for multiple communication interfaces
- Integrating LLMs into structured event-driven workflows
- Managing per-user state in real-time systems
- Trade-offs between simplicity and scalability in single-file architecture

---

## Direction

Next steps: modularizing bot.js into separate service layers, adding multi-agent patterns, and improving response control.
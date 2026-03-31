# AutoResponse Engine

A unified backend system designed to handle real-time conversational workflows across multiple interfaces — integrating a Telegram bot and a web-based chat client through a single service layer.

---

## Overview

This project explores how a single backend can coordinate multiple interaction channels while maintaining consistent logic, response generation, and state handling.

The system is built around an event-driven architecture, where user inputs from different platforms are processed through a shared pipeline, enabling controlled and scalable interaction flow.

---

## System Design

- A single Express-based backend serves both:
  - Telegram bot interface  
  - Web-based chat client  

- Input from each source is normalized and passed through a shared processing layer  
- Responses are generated using an external language model and returned through the respective channel  

---

## Core Capabilities

- Multi-interface interaction handling (Telegram + Web)  
- AI-driven response generation using LLM integration  
- Command-based control flow (e.g., summarization, mode switching)  
- Per-user state tracking for dynamic behavior (e.g., summarization mode)  

---

## Architecture Flow

User Input → Interface Layer → Express Server → Processing Logic → LLM → Response → Client

---

## Technology

- Node.js, Express  
- grammY (Telegram interface)  
- Groq API (LLaMA3)  
- dotenv, CORS  

---

## Deployment

Frontend: https://smartchattldr-ai.netlify.app/  
Backend: https://telegrambot-znt2.onrender.com  
Bot: https://t.me/SmartChatTLDR_AI_Bot?start=_tgr_AIwV5SxiYTM1  

---

## Setup
git clone https://github.com/MrRanjan12/TelegramBot.git

cd TelegramBot
npm install
npm start


---

## Direction

This project is part of a broader exploration into event-driven systems, real-time interaction handling, and how language models can be integrated into structured application workflows.

Further work will focus on improving response control, scalability, and multi-agent interaction patterns.


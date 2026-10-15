# KLXG Helps You 🏦

> A conversational banking agent with real-time fraud risk detection — built for the DBS track, Tencent Cloud AI CAN DO IT Hackathon 2026.

## What it does

KLXG Helps You acts as a guardian for everyday bank transfers. Users — especially the elderly — simply talk to it naturally. The agent handles the rest: understanding intent, collecting missing details, and flagging suspicious transactions before they go through.

## Key Features

- **Natural language transfers** — "Transfer 100 to mom" just works
- **Batch processing** — multiple transfers in one sentence
- **New recipient flow** — automatically collects bank name and account number for unknown payees
- **5-dimension risk engine** — scores every transfer across:
  - Unfamiliar recipient
  - Unusual amount deviation
  - Manipulation language detection
  - Info mismatch
  - Flagged account list
- **Fuzzy contact matching** — tolerates typos (e.g. "alx" → Alex Tan)
- **Multi-turn context** — remembers what's been asked across the conversation
- **Receipt download** — generates a transfer record on completion

## How to Use

1. Open the live demo link
2. Click the **⚙ key icon** (top right) and enter your [Groq API key](https://console.groq.com)
3. Start chatting — try:
   - `转100给妈妈` (Transfer 100 to mom)
   - `转500给Alex，300给David，DBS账号9876543`
   - `转10000给66998877` (triggers HIGH RISK warning)

> No Groq key? The agent falls back to a local parser for basic commands.

## Tech Stack

- Pure HTML + JavaScript (no framework, no backend)
- [Groq API](https://groq.com) — LLM inference
- Runs entirely in the browser

## Hackathon

**Tencent Cloud AI CAN DO IT Hackathon Singapore 2026**
Track: Banking / DBS — Case Study 1 (DCTA)

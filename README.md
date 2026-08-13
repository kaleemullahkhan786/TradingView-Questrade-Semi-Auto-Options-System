# TradingView → Questrade Semi-Auto Options System

Semi-automated **US options trading stack** that combines TradingView Pine tooling with a **FastAPI webhook executor for Questrade** including call/put level handling, multi-target exits, trailing helpers, and optional Discord alerts.

---

## What This System Is For

Use this project when you want to:

- Manage options levels from a TradingView semi-auto UI
- Send trade intents to a Python FastAPI executor
- Place/manage Questrade options orders from alerts
- Handle TP1/TP2 style targets and trailing logic
- Keep OAuth sessions refreshed for continuous operation

---

## How It Works

```text
TradingView Pine UI / alerts
        ↓
FastAPI webhook executor
        ↓
Questrade API (OAuth)
        ↓
Options order placement / management
```

1. Trader defines levels / signals in TradingView Pine components.
2. Alerts or webhook payloads reach the FastAPI service.
3. The executor validates the request and talks to Questrade.
4. Call/Put orders are managed with target and trailing helpers.
5. Optional Discord hooks notify status; paper logging can record dry runs.

---

## Key Features

- Pine semi-auto UI / levels workflow
- FastAPI webhook executor for Questrade
- Call / Put level handling
- TP1 / TP2 style targets and trailing helpers
- OAuth refresh oriented broker session handling
- Optional Discord alert hooks
- Paper logging helpers
- MTF Fib related Pine components (where included)

---

## Technologies Used

- TradingView Pine Script
- Python FastAPI
- Questrade API

## Supported Platforms

- TradingView
- Questrade accounts with API access
- Python hosting for the executor

---

## Important Notes

- **Scrub `config.json` tokens before any public push.**
- Options trading is high risk; no performance claims.

## Limitations

- Depends on Questrade API availability and OAuth refresh reliability.
- US options market hours and contract selection must be managed carefully.

---

## Contact

**WhatsApp:** +923147121270

**Email:** [kaleemullahkhan.contact@gmail.com](mailto:kaleemullahkhan.contact@gmail.com)

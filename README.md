# CryptoSimulator

<div align="center">

```
 ██████╗██████╗ ██╗   ██╗██████╗ ████████╗ ██████╗ ███████╗██╗███╗   ███╗██╗   ██╗██╗      █████╗ ████████╗ ██████╗ ██████╗ 
██╔════╝██╔══██╗╚██╗ ██╔╝██╔══██╗╚══██╔══╝██╔═══██╗██╔════╝██║████╗ ████║██║   ██║██║     ██╔══██╗╚══██╔══╝██╔═══██╗██╔══██╗
██║     ██████╔╝ ╚████╔╝ ██████╔╝   ██║   ██║   ██║███████╗██║██╔████╔██║██║   ██║██║     ███████║   ██║   ██║   ██║██████╔╝
██║     ██╔══██╗  ╚██╔╝  ██╔═══╝    ██║   ██║   ██║╚════██║██║██║╚██╔╝██║██║   ██║██║     ██╔══██║   ██║   ██║   ██║██╔══██╗
╚██████╗██║  ██║   ██║   ██║        ██║   ╚██████╔╝███████║██║██║ ╚═╝ ██║╚██████╔╝███████╗██║  ██║   ██║   ╚██████╔╝██║  ██║
 ╚═════╝╚═╝  ╚═╝   ╚═╝   ╚═╝        ╚═╝    ╚═════╝ ╚══════╝╚═╝╚═╝     ╚═╝ ╚═════╝ ╚══════╝╚═╝  ╚═╝   ╚═╝    ╚═════╝ ╚═╝  ╚═╝
```

**Paper Trading Simulator — futuristic cyberpunk UI, real-time candlestick charts, multi-agent architecture**

[![Play Live](https://img.shields.io/badge/▶_Play_Live-crowfly22.github.io/CryptoSimulator-blue?style=for-the-badge)](https://crowfly22.github.io/CryptoSimulator/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![MiMo V2.5](https://img.shields.io/badge/Powered_by-MiMo_V2.5-purple?style=flat-square)](https://100t.xiaomimimo.com/)

</div>

---

## Overview

CryptoSimulator is a **zero-dependency paper trading simulator** with a futuristic cyberpunk aesthetic. Trade 8 major crypto pairs with real-time candlestick charts, AI-powered trading strategies, and multi-agent market analysis — all running 100% client-side.

Built for the **MiMo 100T Token Creator Incentive Program** with MiMo V2.5 Pro integration.

## Features

### 🎯 Trading Engine
- **8 Crypto Pairs:** BTC, ETH, SOL, BNB, XRP, ADA, DOGE, AVAX
- **Market Orders:** Buy/Long and Sell/Short with instant execution
- **Portfolio Tracking:** Real-time P&L, position management, cost basis
- **$10,000 Virtual Balance** — reset anytime

### 📊 Charts & Analytics
- **Candlestick Charts** with real-time price simulation
- **Technical Indicators:** SMA-20, SMA-50, RSI, MACD
- **Volume Bars** with color-coded buy/sell pressure
- **Multi-timeframe** support

### 🤖 Multi-Agent Architecture
- **Market Agent:** AI-powered trend analysis with BUY/SELL/HOLD signals
- **Risk Agent:** Position sizing, stop-loss management, portfolio diversification
- **Strategy Agent:** SMA crossover, momentum, and mean-reversion strategies
- **Board Agent:** Agent coordination and decision synthesis

### 🎮 5 Interactive Tabs
| Tab | Description |
|-----|-------------|
| **TRADE** | Live candlestick chart + order panel |
| **PORTFOLIO** | Positions, P&L, asset allocation |
| **HISTORY** | Trade log with timestamps |
| **STRATEGY** | AI agent analysis & signals |
| **BOARD** | Multi-agent decision dashboard |

### 🎨 Cyberpunk UI
- **Neon Cyan/Magenta** color scheme
- **CRT scanline** overlay effect
- **Orbitron + JetBrains Mono** typography
- **Glassmorphism** panels with backdrop blur
- **Responsive** layout

## Quick Start

```bash
# Clone
git clone https://github.com/crowfly22/CryptoSimulator.git
cd CryptoSimulator

# Open directly
open index.html

# Or serve locally
python3 -m http.server 8080
# → http://localhost:8080
```

**Zero dependencies.** Just open `index.html` in any modern browser.

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Frontend | Vanilla HTML5 + CSS3 + JavaScript |
| Charts | Canvas 2D (custom candlestick renderer) |
| AI Engine | MiMo V2.5 Pro (multi-agent) |
| Architecture | Single-file SPA, zero dependencies |
| Styling | CSS Grid, Custom Properties, Glassmorphism |

## Architecture

```
┌─────────────────────────────────────────────────┐
│              CRYPTO SIMULATOR                    │
├─────────────────────────────────────────────────┤
│                                                  │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐      │
│  │  Market   │  │   Risk   │  │ Strategy │      │
│  │  Agent    │  │  Agent   │  │  Agent   │      │
│  └────┬─────┘  └────┬─────┘  └────┬─────┘      │
│       │              │              │            │
│       └──────────┬───┴──────────────┘            │
│                  │                               │
│           ┌──────┴──────┐                       │
│           │   Board     │                       │
│           │   Agent     │                       │
│           └──────┬──────┘                       │
│                  │                               │
│  ┌───────────────┴───────────────────────┐      │
│  │         Trading Engine                 │      │
│  │  • Order execution                     │      │
│  │  • Portfolio management                │      │
│  │  • Price simulation                    │      │
│  └───────────────────────────────────────┘      │
│                                                  │
│  ┌───────────────────────────────────────┐      │
│  │         Canvas Renderer               │      │
│  │  • Candlestick charts                 │      │
│  │  • Volume bars                        │      │
│  │  • Technical overlays                 │      │
│  └───────────────────────────────────────┘      │
│                                                  │
└─────────────────────────────────────────────────┘
```

## Screenshots

### Trading View
![Trading View](screenshots/01-landing.png)

### Portfolio Dashboard
![Portfolio](screenshots/02-demo.png)

### AI Strategy Analysis
![Strategy](screenshots/03-footer.png)

## MiMo 100T Submission

This project was built for the [MiMo 100T Token Creator Incentive Program](https://100t.xiaomimimo.com/).

| Field | Value |
|-------|-------|
| **Tools** | Claude Code, Hermes Agent, Cursor |
| **Models** | Claude 系列, MiMo V2.5 Pro |
| **Architecture** | Multi-agent (Market, Risk, Strategy, Board) |
| **Features** | Paper trading, candlestick charts, AI analysis |

## License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**Built for MiMo AI Grant** · Powered by MiMo V2.5 from Xiaomi

CryptoSimulator © 2026

</div>

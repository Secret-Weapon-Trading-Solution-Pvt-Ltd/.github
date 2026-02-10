# Secret Weapon Trading Solution (SWTS)

**Building high-performance, real-time algorithmic trading systems and infrastructure tools.**

SWTS is a trading technology organization focused on developing production-grade trading platforms, automated strategy execution engines, and supporting infrastructure. Our stack is built around Python, FastAPI, Next.js, Redis, Docker, and real-time WebSocket pipelines.

---

## Our Repositories

### Trading Platforms & Strategy Engines

| Repository | Description | Tech Stack |
|---|---|---|
| **[Arbitrage-Strategy](../Arbitrage-Strategy)** | Pair trading arbitrage system with real-time spread calculation, signal generation (FAR/NEAR/NEUTRAL), automated entry/exit order management, and historical candle analysis across multiple timeframes. | Python, FastAPI, Next.js 14, Zerodha Kite API, Socket.IO, Redis, Docker |
| **[pebble-sahil](../pebble-sahil)** | Premium algorithmic trading terminal for futures trading using Supertrend and SMA-based strategies. Features bot dashboard, execution control (Launch/Pause/Resume/Panic Square-Off), order pipeline visualization, and paper trading mode. | Python 3.13, FastAPI, React, Vite, TypeScript, Zustand, Redis, Docker |
| **[Segen_dhairya](../Segen_dhairya)** | High-concurrency algo trading system for automated option selling (Straddle/Strangle) via the Upstox API. Supports zero-manual-intervention login, margin-aware order slicing, delta-neutral rebalancing, and sub-second risk monitoring. | Python 3.10+, FastAPI, Redis, Upstox API, Telegram Bot, Docker |

### Indicators & Screeners

| Repository | Description | Tech Stack |
|---|---|---|
| **[EigenKor-Space-Time-Indicator](../EigenKor-Space-Time-Indicator)** | Distributed trading indicator system with real-time tick processing, historical data storage via InfluxDB, and WebSocket-based data distribution. Supports standalone and shared Nginx deployment with auto SSL. | Python, FastAPI, Node.js, InfluxDB, Redis, Socket.IO, Docker, GitHub Actions |
| **[swts-ema-crossover](../swts-ema-crossover)** | Real-time cryptocurrency EMA crossover screener monitoring multiple symbols and timeframes (1m to 1d). Features live WebSocket alerts, dynamic watchlist management, and Redis-cached historical analysis. | Python, FastAPI, Pandas, Redis, WebSockets, HTML/CSS/JS, Docker |

### Website

| Repository | Description | Tech Stack |
|---|---|---|
| **[SWTS_Website-GithubPage](../SWTS_Website-GithubPage)** | Organization landing page and lead generation site with server-side rendering, animation effects, and Upstash Redis-backed form submissions. | Next.js 14, React 18, TypeScript, Tailwind CSS, Framer Motion, Upstash Redis, Docker |

### Infrastructure & DevOps

| Repository | Description | Tech Stack |
|---|---|---|
| **[aws-ubuntu-gui-setup](../aws-ubuntu-gui-setup)** | Automated setup script for Ubuntu desktop environments on AWS EC2 with XFCE4 + XRDP remote desktop access. Installs dev tools (Python, Node.js, VS Code, Chrome). | Bash, XFCE4, XRDP, Docker |
| **[nginx-setup-guide](../nginx-setup-guide)** | Interactive documentation site for Nginx web server configuration, setup procedures, and deployment best practices. | HTML, CSS |
| **[ubuntu-docker-logs-finder](../ubuntu-docker-logs-finder)** | Web application for browsing and searching Docker container logs on remote EC2 instances via SSH. Features session-based auth, date filtering, and real-time log streaming. | Python, FastHTML, Paramiko (SSH), Uvicorn, Docker |

---

## Tech Overview

```
Languages       Python  |  TypeScript  |  JavaScript  |  Bash
Backend         FastAPI  |  Uvicorn  |  Node.js  |  FastHTML
Frontend        Next.js  |  React  |  Vite  |  Tailwind CSS
Real-Time       WebSocket  |  Socket.IO  |  Redis Pub/Sub
Databases       Redis  |  InfluxDB  |  Upstash Redis
Auth            JWT  |  Bcrypt
Broker APIs     Zerodha Kite  |  Upstox
Infrastructure  Docker  |  Docker Compose  |  Nginx  |  AWS EC2  |  GitHub Actions
```

---

## Architecture Principles

- **Real-Time First** &mdash; WebSocket and Socket.IO pipelines for sub-second market data delivery and trade execution.
- **Containerized Deployments** &mdash; Every service ships with Docker and Docker Compose for reproducible environments.
- **Microservices Where It Matters** &mdash; Core platforms use service-oriented architecture; smaller tools stay monolithic for simplicity.
- **Redis as the Backbone** &mdash; Used across all systems for caching, pub/sub messaging, session management, and state persistence.
- **Automated & Observable** &mdash; CI/CD with GitHub Actions, structured logging, health checks, and Prometheus metrics where applicable.

---

## Contact

- **General Inquiries:** support@secretweapon.in
- **Repository Access:** murarkacj@gmail.com

---

> *Precision in execution. Speed in delivery.*

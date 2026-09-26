# StrataX — Quantitative Algorithmic Trading Workstation


    StrataX is an internal algorithmic trading cockpit and quantitative analysis workstation designed for real-time market microstructure monitoring, technical charting, and private order execution.

    ---

    ## 📌 Architecture & Charting Engine

    The platform integrates advanced charting capabilities to visualize multi-timeframe historical candlestick data and sub-second streaming ticks from private broker APIs:

    - **Charting Layer:** Integration with **TradingView Advanced Charts** (`charting_library`) via a custom JavaScript Datafeed implementation (`JS Datafeed API`).
    - **Data Ingestion:** High-throughput streaming WebSocket daemon connected to registered Indian broker APIs (Kotak Neo / Upstox).
    - **Timeframes Supported:** Real-time 1s, 1m, 5m, 15m, 1h, and Daily historical resolutions.
    - **Analytics:** Custom indicator pipelines (EMA ribbons, Supertrend, Bollinger Bands, Volume Profile) computed via dedicated background Web Workers.

    ---

    ## 🚀 Key Modules

    - **Terminal Charting:** Full multi-chart layout with synchronized crosshairs, custom drawing tools, and magnetic price snapping.
    - **Option Chain & Greeks Engine:** Black-Scholes pricing solver and implied volatility tracking.
    - **Microstructure & Order Flow:** Real-time trade tick aggregations and delta analysis.
    - **Execution Desk:** Low-latency order routing with automated pre-trade risk management (RMS).

    ---

    ## 🔒 Non-Commercial & Access Policy

    This repository and application are strictly developed for **internal quantitative research and private personal trading**. 

    - The application is **non-commercial** and is not offered as a public SaaS or subscription service.
    - All live deployments are private, password-protected, and restricted to authorized personal execution workstations.
    - All chart components retain full attribution and compliance with TradingView licensing terms.

    ---

    ## 🛠️ Tech Stack

    - **Frontend:** Next.js / React, TypeScript, Tailwind CSS, TradingView Advanced Charts
    - **Backend & Ingestion:** Node.js, WebSockets, DuckDB / Parquet time-series storage
    - **Broker APIs:** Upstox API v2 / Kotak Neo HSM Feed

    ---

    ## 👤 Author

    Developed by **Sanjeev Singh** ([@sanjeevsingh2026](https://github.com/sanjeevsingh2026))  
    *StrataX Trading Technologies*

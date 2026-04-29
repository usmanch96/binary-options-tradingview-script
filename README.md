# 📌 Binary Options TradingView Script — Pin Bar Reversal Indicator

<div align="center">

```
██████╗ ██╗███╗   ██╗    ██████╗  █████╗ ██████╗
██╔══██╗██║████╗  ██║    ██╔══██╗██╔══██╗██╔══██╗
██████╔╝██║██╔██╗ ██║    ██████╔╝███████║██████╔╝
██╔═══╝ ██║██║╚██╗██║    ██╔══██╗██╔══██║██╔══██╗
██║     ██║██║ ╚████║    ██████╔╝██║  ██║██║  ██║
╚═╝     ╚═╝╚═╝  ╚═══╝    ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝
       R E V E R S A L   I N D I C A T O R
```

**The #1 Binary Options TradingView Script for Pin Bar Reversal Trading**  
*Pine Script v6 · Non-Repainting · S/R Confluence · 5m & 15m · 6 Major Pairs*

---

[![Pine Script](https://img.shields.io/badge/Pine%20Script-v6-2196F3?style=for-the-badge&logo=tradingview&logoColor=white)](https://www.tradingview.com)
[![Platform](https://img.shields.io/badge/Platform-TradingView-1e88e5?style=for-the-badge&logo=tradingview&logoColor=white)](https://www.tradingview.com)
[![Timeframe](https://img.shields.io/badge/Timeframe-5m%20%7C%2015m-00c853?style=for-the-badge)](.)
[![License](https://img.shields.io/badge/License-MIT-ff6f00?style=for-the-badge)](LICENSE)
[![Strategy](https://img.shields.io/badge/Strategy-Pin%20Bar%20%2B%20S%2FR-9c27b0?style=for-the-badge)](.)
[![No Repaint](https://img.shields.io/badge/Repaint-ZERO-00e676?style=for-the-badge)](.)
[![Telegram](https://img.shields.io/badge/Telegram-Contact%20Me-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/usmanch069)

</div>

---

## 📋 Table of Contents

- [🎯 Overview](#-overview)
- [✨ Features](#-features)
- [📊 Recommended Pairs & Timeframes](#-recommended-pairs--timeframes)
- [🛠️ How It Works](#️-how-it-works)
- [⚙️ Installation](#️-installation)
- [🎛️ Settings Reference](#️-settings-reference)
- [📖 How to Trade with It](#-how-to-trade-with-it)
- [🔔 Alerts Setup](#-alerts-setup)
- [🔒 Non-Repainting Guarantee](#-non-repainting-guarantee)
- [⚠️ Risk Disclaimer](#️-risk-disclaimer)

---

## 🎯 Overview

The **Pin Bar Reversal** is a **free binary options TradingView script** built in Pine Script v6. It is designed specifically for traders who use **TradingView charts to trade binary options** on short expiry timeframes. It identifies high-probability reversal setups by combining **classic Pin Bar candlestick geometry** with **dynamic Support & Resistance confluence** — the same methodology used by professional price-action traders worldwide.

Whether you are searching for a **binary options TradingView script** that doesn't repaint, a **free Pine Script for binary options**, or a reliable **TradingView indicator for 5 minute binary options** — this tool is built for you.

> 🎯 **Core Concept:** A Pin Bar at a key S/R level signals market rejection. Price is being pushed back by institutional traders. Entry on the **very next candle open** maximises the probability of catching the reversal.

```
          ┌─────────────────────────────────────────────┐
          │         SIGNAL LOGIC FLOWCHART              │
          └─────────────────────────────────────────────┘

  Candle forms   →   Pin Bar   →   S/R Nearby?   →   SIGNAL 🔔
  on chart            check           check
                     wick > 1.8x   within 1.5×ATR
                       body          of a pivot
                         │                │
                        YES              YES
                         └───────┬────────┘
                                 ▼
                         ⬆ CALL  or  ⬇ PUT
                                 │
                    Enter on NEXT candle OPEN
```

---

## ✨ Features

| Feature | Description |
|---|---|
| 📌 **Pin Bar Detection** | Identifies genuine reversal candles via strict wick-to-body geometry |
| 🏗️ **Auto S/R Levels** | Dynamically plots swing high/low Support & Resistance using `ta.pivothigh/low` |
| 🚦 **Signal Arrows** | Clean `CALL` ↑ and `PUT` ↓ arrows appear on confirmed candle closes |
| 🌈 **Bar Glow** | Signal bars highlighted with a subtle colour glow for instant visual recognition |
| 🕵️ **Live Watch Label** | Real-time label on the forming bar shows if a signal is developing (e.g. `CALL FORMING 87%`) |
| 🔕 **Cooldown System** | Prevents stacked arrows — minimum N bars between signals (configurable) |
| 📐 **EMA Trend Filter** | Optional 50 EMA filter — CALL above EMA only, PUT below EMA only |
| 📉 **RSI Filter** | Optional RSI overbought/oversold confirmation for higher quality setups |
| 🔔 **TradingView Alerts** | Full alert support — CALL, PUT, or any signal |
| ✅ **Zero Repaint** | Signals are based on `close`-confirmed data only — permanent, never change |

---

## 📊 Recommended Pairs & Timeframes

This indicator is optimised and tested on the following **Forex pairs** via **Binary Options platforms**:

<div align="center">

| # | Pair | Nickname | Recommended TF |
|---|---|---|---|
| 🇪🇺🇺🇸 | **EUR/USD** | The Fiber | ⏱️ 5m · 15m |
| 🇬🇧🇺🇸 | **GBP/USD** | The Cable | ⏱️ 5m · 15m |
| 🇺🇸🇯🇵 | **USD/JPY** | The Yen | ⏱️ 5m · 15m |
| 🇺🇸🇨🇭 | **USD/CHF** | The Swissie | ⏱️ 5m · 15m |
| 🇦🇺🇺🇸 | **AUD/USD** | The Aussie | ⏱️ 5m · 15m |
| 🇺🇸🇨🇦 | **USD/CAD** | The Loonie | ⏱️ 5m · 15m |

</div>

> 💡 **Best trading sessions:** London Open (08:00–12:00 GMT) and New York Open (13:00–17:00 GMT) produce the highest volatility and most reliable pin bar formations on 5m and 15m charts.

---

## 🛠️ How It Works

### 1️⃣ Pin Bar Geometry

A valid **Bullish Pin Bar (CALL)** requires:
```
        │  ← Long lower wick  (≥ 1.8× body size)
       ███ ← Small body in upper 45% of candle range
```

A valid **Bearish Pin Bar (PUT)** requires:
```
       ███ ← Small body in lower 45% of candle range  
        │  ← Long upper wick  (≥ 1.8× body size)
```

### 2️⃣ Support & Resistance Confluence

The indicator uses `ta.pivothigh` and `ta.pivotlow` with configurable swing strength to detect **significant price levels**. A signal only fires when the pin bar's wick tip is within `1.5 × ATR(14)` of a confirmed pivot level.

```
  Resistance ─────────────────── ███  ←── Bearish Pin at Resistance = PUT ⬇
                                  │
  Support    ─────────────────── │   ←── Bullish Pin at Support = CALL ⬆
                                 ███
```

### 3️⃣ Cooldown System

After every signal, the indicator enforces a **5-bar cooldown** (configurable). This prevents a cluster of arrows when price lingers at a level — ensuring you only see the cleanest, first-touch signal.

### 4️⃣ Signal Arrow Timing

```
  Bar N  :  Pin Bar forms + S/R hit  →  🔔 Arrow appears on THIS bar's CLOSE
  Bar N+1:  ✅ Enter trade at OPEN  →  This is your entry candle
  Bar N+1:  ⏱️ Trade expires at CLOSE →  Result determined
```

---

## ⚙️ Installation

### Step 1 — Open Pine Editor

1. Go to [TradingView.com](https://www.tradingview.com) and open any chart
2. Click **"Pine Editor"** at the bottom of the screen
3. Click **"Open"** → **"New indicator"**

### Step 2 — Paste the Script

1. Select all existing code in the editor (`Ctrl+A`)
2. Delete it
3. Copy the entire contents of [`PinBarReversal.pine`](./PinBarReversal.pine)
4. Paste it into the editor

### Step 3 — Add to Chart

1. Click **"Add to chart"** (blue button, top right of Pine Editor)
2. The indicator will load on your chart immediately

### Step 4 — Set Your Chart

- Set your chart to **EURUSD**, **GBPUSD**, **USDJPY**, **USDCHF**, **AUDUSD**, or **USDCAD**
- Set timeframe to **5 minutes** or **15 minutes**
- You're ready to trade! 🎯

---

## 🎛️ Settings Reference

Click the **⚙️ Settings** icon on the indicator to open the configuration panel.

### 📐 Pin Bar Geometry

| Setting | Default | Description |
|---|---|---|
| **Wick/Body Ratio** | `1.8` | Minimum wick length relative to body. Higher = stricter pin bars |
| **Body Zone (max %)** | `0.45` | Max % of candle range the body can occupy. Lower = purer pin bars |
| **Cooldown Bars** | `5` | Minimum bars between signals. Prevents stacked arrows |

### 🏗️ Support and Resistance

| Setting | Default | Description |
|---|---|---|
| **Swing Strength** | `3` | Bars required on each side to confirm a pivot. Higher = stronger levels only |
| **S/R Lookback Bars** | `100` | How far back to search for pivot levels |
| **Proximity x ATR** | `1.50` | How close the wick must be to a level (in ATR multiples) |
| **ATR Period** | `14` | Period for Average True Range calculation |

### 🖥️ Display

| Setting | Default | Description |
|---|---|---|
| **CALL Color** | 🟢 Green | Arrow and glow colour for bullish signals |
| **PUT Color** | 🔴 Red | Arrow and glow colour for bearish signals |
| **Show S/R Lines** | `ON` | Toggles the dashed support/resistance lines |
| **Show Live Signal Watch** | `ON` | Toggles the real-time forming-signal label |
| **EMA Trend Filter** | `OFF` | When ON: CALL only above 50 EMA, PUT only below |
| **EMA Length** | `50` | Period for the trend EMA |
| **RSI Filter** | `OFF` | When ON: CALL when RSI < threshold, PUT when RSI > threshold |
| **RSI Length** | `14` | Period for RSI calculation |
| **RSI Oversold (CALL <)** | `45` | RSI must be below this for CALL signals (when filter is ON) |
| **RSI Overbought (PUT >)** | `55` | RSI must be above this for PUT signals (when filter is ON) |

---

## 📖 How to Trade with It

### 🟢 CALL Signal (Buy)

```
✅ Bullish Pin Bar detected
✅ Pin bar wick near a Support level
✅ Arrow appears BELOW the bar
→ Enter CALL at the OPEN of the NEXT 5m/15m candle
→ Set expiry = 1 candle (same as your chart timeframe)
```

### 🔴 PUT Signal (Sell)

```
✅ Bearish Pin Bar detected
✅ Pin bar wick near a Resistance level
✅ Arrow appears ABOVE the bar
→ Enter PUT at the OPEN of the NEXT 5m/15m candle
→ Set expiry = 1 candle (same as your chart timeframe)
```

### 👁️ Live Watch Label

The label appearing on the **current forming bar** is a preview — it shows the pin bar is developing but the candle hasn't closed yet. **Do not enter based on this label alone.** Wait for the bar to close and the arrow to lock in.

```
  "CALL FORMING 87% | Pin + Support"  ← Preview only — wait for candle close
  ⬆ CALL  ← Arrow locked on closed bar — this is your entry signal
```

### 🎯 Best Practices

- 📅 **Trade during active sessions** — London & New York overlap (13:00–16:00 GMT)
- 🚫 **Avoid news events** — Major economic releases cause erratic candles
- 📏 **Respect the S/R lines** — The dashed lines show the levels the indicator is using
- 🔁 **Don't chase** — If you miss a signal, skip it. Another will come
- 📓 **Keep a trade journal** — Track your win rate per pair over 50+ trades

---

## 🔔 Alerts Setup

Set up alerts to be notified on your phone or desktop without watching the chart.

1. Right-click anywhere on the chart
2. Select **"Add alert..."**
3. In the **Condition** dropdown, select **"Pin Bar Reversal"**
4. Choose from:
   - `CALL Signal` — alert only on CALL setups
   - `PUT Signal` — alert only on PUT setups
   - `Any Signal` — alert on either direction
5. Set notification method (popup, email, push notification)
6. Click **Create**

> ⚡ **Pro tip:** Set separate alerts for CALL and PUT so you instantly know the direction from the notification message alone.

---

## 🔒 Non-Repainting Guarantee

This indicator is built with a strict **no-repainting architecture**:

| Component | Repaint? | Why |
|---|---|---|
| **Signal arrows** | ❌ Never | Evaluated on final OHLC of a closed bar |
| **S/R pivot levels** | ❌ Never | Confirmed after `swingStr` bars pass (lagged, not repainting) |
| **Cooldown tracker** | ❌ Never | `var` persistent state — historical signals are immutable |
| **Live Watch Label** | ✅ Intentional | Updates on the forming bar — this is a preview feature, not a signal |

> ⚠️ **The Live Watch Label is NOT a signal.** It updates as the current bar forms. Only the locked arrow on a **closed candle** is the confirmed signal.

---

## 📁 Repository Structure

```
📦 pin-bar-reversal
 ┣ 📜 PinBarReversal.pine   ← The indicator source code (Pine Script v6)
 ┗ 📖 README.md              ← This file
```

---

## 🤝 Contributing

Found a bug or have a suggestion? Open an [Issue](../../issues) or submit a [Pull Request](../../pulls). All contributions welcome!

---

## 📬 Contact & Community

Have questions about the strategy? Want to share results or get help with settings?

<div align="center">

[![Telegram](https://img.shields.io/badge/Telegram-%40usmanch069-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/usmanch069)

**👆 Click to message on Telegram**

*Feel free to reach out for setup help, signal discussions, or trading feedback.*

</div>

---

## ⚠️ Risk Disclaimer

> **IMPORTANT — PLEASE READ**
>
> This indicator is provided for **educational and informational purposes only**.  
> Trading Binary Options involves **substantial risk of loss** and is not suitable for all investors.  
> Past performance of any trading strategy does **not guarantee future results**.  
> The indicator does not constitute financial advice. Never trade with money you cannot afford to lose.  
> Always practice on a **demo account** before trading real funds.  
> The authors of this indicator accept **no liability** for any financial losses incurred.

---

<div align="center">

**Built with ❤️ for Binary Options traders**

*If this indicator helps you, consider leaving a ⭐ on the repository!*

---

`Pine Script v6` · `TradingView` · `Binary Options` · `Pin Bar` · `Price Action` · `Support & Resistance` · `Non-Repainting`

</div>

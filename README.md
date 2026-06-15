<div align="center">

# 📊 ADX Trend Filter Pro — Alpha Edition

**A professional-grade ADX/DMI indicator for TradingView**  
*Built for traders who demand precision over noise*

[![Pine Script](https://img.shields.io/badge/Pine%20Script-v6-blue?style=for-the-badge&logo=tradingview)](https://www.tradingview.com)
[![License](https://img.shields.io/badge/License-MPL%202.0-green?style=for-the-badge)](https://mozilla.org/MPL/2.0/)
[![Author](https://img.shields.io/badge/Author-RehanFX__Alpha-orange?style=for-the-badge)](https://github.com/RehanFX-Alpha)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)]()

---

> *"Don't trade the noise. Trade the trend."*

</div>

---

## 🧠 What is This?

**ADX Trend Filter Pro** is an advanced TradingView indicator built on the classic ADX/DMI system — but taken several levels further. It tells you not just **which direction** the market is moving, but **how strong** that move is, whether it's **diverging**, and whether you should even be trading at all.

Perfect as a **standalone trend filter** or as a **confirmation layer** on top of your existing strategy.

---

## ✨ Features

| Feature | Description |
|--------|-------------|
| 📐 **ADX Strength Levels** | 4 levels: Weak / Moderate / Strong / Very Strong — each with distinct color |
| 📈 **EMA Trend Band** | Dual EMA (customizable) plotted as MA Band at ADX threshold level |
| 🎨 **Gradient Histogram** | DI+ / DI- bars get darker as ADX strengthens — visual momentum feedback |
| ⚠️ **Divergence Detection** | Detects when price makes HH/LL but ADX disagrees — early reversal warning |
| 🎯 **Signal Quality Filter** | Optional: only fire signals when ADX is Moderate or above |
| 📊 **Live Info Table** | 8-row real-time dashboard: ADX value, DI values, direction, trend mode, divergence |
| 🔔 **8 Smart Alerts** | Buy/Sell, Strong Trend, Trend Weakening, Divergence, EMA Cross |
| 🕯️ **Bar Coloring** | Candles colored green (bull trend), red (bear trend), yellow (ranging) |

---

## 📸 Indicator Preview

```
┌─────────────────────────────────────────┐
│  ADX PRO [Alpha]  │  VALUE   │  STATUS  │
├───────────────────┼──────────┼──────────┤
│  Candle           │ Bullish  │  65,692  │
│  ADX              │   39.0   │ STRONG💪 │
│  Direction        │ DI+ ▲    │  3 bars  │
│  DI+ / DI-        │   34.4   │    9.5   │
│  EMA Trend        │ Bullish📈│  12/50   │
│  Market           │TRENDING▲ │ Trade OK │
│  Divergence       │  None ✅ │  Clean   │
└─────────────────────────────────────────┘
```

---

## 🚦 How to Read Signals

### ✅ BUY Signal (Green ▲ Label)
All 3 conditions must be true:
1. **DI+ crosses above DI-** (bullish momentum shift)
2. **ADX above Weak threshold** (trend has strength)
3. **MA Band is Green** (EMA Fast > EMA Slow)

### 🔴 SELL Signal (Red ▼ Label)
All 3 conditions must be true:
1. **DI- crosses above DI+** (bearish momentum shift)
2. **ADX above Weak threshold** (trend has strength)
3. **MA Band is Red** (EMA Fast < EMA Slow)

### ⚠️ Divergence Warning
- **Bull DIV** — Price making Higher Highs but ADX is falling → bull trend losing steam
- **Bear DIV** — Price making Lower Lows but ADX is falling → bear trend losing steam
- *Action: tighten SL or avoid new entries*

### 🟡 Yellow Candles = Ranging Market
ADX below threshold — **no trend, no trade.** Wait for color to return.

---

## ⚙️ Settings Guide

### 📐 ADX Settings
| Setting | Default | Description |
|---------|---------|-------------|
| ADX Length | 14 | Lookback for ADX calculation |
| ADX Smoothing | 14 | Smoothing period |
| Weak Threshold | 20 | Below = ranging market |
| Moderate Threshold | 30 | Recommended min for trading |
| Strong Threshold | 40 | High conviction zone |

### 📈 EMA Settings
| Setting | Default | Description |
|---------|---------|-------------|
| Fast EMA | 12 | Short-term trend |
| Slow EMA | 50 | Long-term trend |

### 🎯 Signal Settings
| Setting | Default | Description |
|---------|---------|-------------|
| Only Strong Signals | OFF | Enable to only signal when ADX ≥ Moderate |
| Show Divergence | ON | Show ⚠ DIV warnings on chart |

---

## 🔔 Alerts Reference

| Alert Name | Trigger |
|------------|---------|
| ▲ ADX Buy Signal | DI+ crosses above DI- with ADX strength |
| ▼ ADX Sell Signal | DI- crosses above DI+ with ADX strength |
| 🔥 Very Strong Trend | ADX crosses above Strong threshold |
| 😴 Trend Weakening | ADX drops below Weak threshold |
| ⚠ Bull Divergence | Price HH but ADX falling in bull trend |
| ⚠ Bear Divergence | Price LL but ADX falling in bear trend |
| EMA Bullish Cross | Fast EMA crosses above Slow EMA |
| EMA Bearish Cross | Fast EMA crosses below Slow EMA |

---

## 🛠️ Installation

1. Open **TradingView** → Pine Script Editor
2. Copy the contents of `ADX_Trend_Filter_Pro_Alpha.pine`
3. Paste into the editor → Click **"Add to chart"**
4. Configure settings from the indicator panel

---

## 💡 Pro Tips

- **Best timeframes:** 1H, 4H, 1D for swing trading | 5m, 15m for scalping
- **Pair with:** Support/Resistance levels, Volume, or a momentum oscillator (RSI)
- **ADX > 40** = very strong trend — ride it but watch for exhaustion
- **Yellow candles** = stay out. Let the market decide direction first.
- **DIV warning** = don't add to position, consider partial exit

---

## 📁 Repository Structure

```
ADX-Trend-Filter-Pro/
│
├── ADX_Trend_Filter_Pro_Alpha.pine   ← Main indicator file
├── README.md                          ← You are here
└── LICENSE                            ← MPL 2.0
```

---

## 📜 License & Credits

- **Original concept:** © traderharikrishna
- **Alpha Edition by:** © RehanFX_Alpha | Muhammad Rehan Afzal
- **License:** [Mozilla Public License 2.0](https://mozilla.org/MPL/2.0/)

> This project is open-source. You are free to use, modify, and distribute under MPL 2.0 terms. Original author credit must be maintained.

---

## 🤝 Contributing

Pull requests welcome! If you have ideas for improvements:
- Fork the repo
- Create a feature branch (`git checkout -b feature/your-idea`)
- Commit your changes
- Open a Pull Request

---

<div align="center">

**⭐ Star this repo if it helped your trading!**

Made with 🧠 by [rehanqx](https://github.com/rehanqx)

</div>

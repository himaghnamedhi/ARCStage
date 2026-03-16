# ARCStage
Stan Weinstein Stage Analysis indicator for TradingView
# ARCStage — Stan Weinstein Stage Analysis
### by [Artha Research Capital (ARC)](https://github.com/himaghnamedhi)

A Pine Script v5 indicator for TradingView that algorithmically detects and color-codes Stan Weinstein's four market cycle stages, with built-in contraction zone detection and breakout/breakdown signals.

---

## 📊 What It Does

Stan Weinstein's Stage Analysis divides every stock's life cycle into four stages. This indicator detects each stage in real time using the 30-Week SMA slope and price position — and communicates everything purely through color, with no cluttered labels on the chart.

| Stage | Color | Meaning |
|-------|-------|---------|
| Stage 1 — Basing | 🩶 Light Gray | Sideways consolidation. Accumulation phase. Wait. |
| Stage 2 — Advancing | 💚 Light Green | Price above rising 30W SMA. The only buy zone. |
| Stage 2 — Strong | 🟢 Bright Green | Price extended significantly above SMA. Strong uptrend. |
| Stage 3 — Topping | 🧡 Light Peach | SMA flattening after advance. Distribution underway. Exit longs. |
| Stage 4 — Declining | 🩷 Light Pink | Price below falling 30W SMA. Confirmed downtrend. Stay out. |

---

## 🔵 Contraction Zone Detection

A unique feature of ARCStage is its ability to detect **price contraction zones** — periods where the trading range narrows progressively, signaling energy compression before a major breakout or breakdown.

During contraction zones:
- Individual candles are colored **sky blue**
- **Blue dotted lines** mark the resistance (upper) and support (lower) boundaries
- A subtle **blue background tint** fills the zone
- **BO** (Breakout) and **BD** (Breakdown) triangle markers fire when price escapes the zone

---

## ⚙️ How to Add to TradingView

1. Open [TradingView](https://www.tradingview.com)
2. Open any chart → click **Pine Script Editor** at the bottom
3. Delete all existing code
4. Copy the full code from [`ARCStage.pine`](./ARCStage.pine)
5. Paste into the editor → click **Save** → click **Add to chart**
6. Switch to **Weekly timeframe** for best results

---

## 🛠️ Settings & Inputs

| Parameter | Default | Description |
|-----------|---------|-------------|
| SMA Length | 30 | Length of the base SMA (30 = 30 weeks) |
| SMA Slope Lookback | 4 | Bars used to calculate SMA slope direction |
| Strong Stage 2 Threshold | 8% | Distance above SMA to classify as strong Stage 2 |
| Contraction Window | 15 | Rolling bars used to detect range contraction |
| Show Background Colors | On | Toggle stage background shading |
| Show Contraction Lines | On | Toggle blue dotted boundary lines |
| Show Contraction Bar Colors | On | Toggle sky blue bar coloring during contraction |
| Show 30W SMA Line | On | Toggle the orange SMA line |

---

## 📅 Recommended Timeframes

| Timeframe | SMA Length Setting |
|-----------|--------------------|
| Weekly (recommended) | 30 |
| Daily | 150 |
| Monthly | 7 |

---

## 📷 Screenshots

> Add your screenshots inside a `/screenshots` folder and link them here.
```
screenshots/
├── stage2_kirloskar.png
├── stage4_nifty.png
└── contraction_zone_example.png
```

---

## 📖 Methodology

Based on the framework described in:

> *"Secrets for Profiting in Bull and Bear Markets"*
> — Stan Weinstein, 1988

The 30-Week Simple Moving Average is the spine of Weinstein's system. Stages are determined by two factors: the **slope** of the SMA (rising / flat / falling) and the **position of price** relative to the SMA (above / near / below).

---

## 📜 License

MIT License — free to use, modify, and distribute with attribution.

---

## 🏢 About Artha Research Capital

**Artha Research Capital (ARC)** is an independent financial research group focused on systematic, research-driven approaches to Indian equity markets.

- 🌐 Website: *coming soon*
- 📧 Contact: *coming soon*
- 🐦 Twitter/X: *coming soon*

---

*Built with 🧠 by Artha Research Capital. Not financial advice.*
```

---

**Topics to add (GitHub repo tags):**
```
tradingview pine-script stage-analysis stan-weinstein technical-analysis indian-markets nse nifty equity research artha-research-capital

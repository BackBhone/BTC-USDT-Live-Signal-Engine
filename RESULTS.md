# Backtest Results — BTC/USDT Live Signal Engine

Full backtest results on real Binance BTC/USDT OHLCV data. Simulation only and not live executed trades.

---

## Configuration

| Parameter | Value |
|---|---|
| Starting Capital | $10,000 |
| Risk Per Trade | 2% of equity |
| Stop Loss | 3% |
| Take Profit | 6% |
| Fees Per Side | 0.1% (Taker) |
| Max Hold | 5 days |
| Data Source | Binance BTC/USDT Daily OHLCV |
| Backtest Range | 01 Jan 2018 to 19 Mar 2026 (2,999 days) |

---

## Summary

| Metric | Value |
|---|---|
| Final Portfolio | **$52,323** |
| Total Return | **+423.2%** |
| Buy and Hold (same period) | +416.5% |
| Total Trades | 495 |
| Long Trades | 237 |
| Short Trades | 258 |
| Win Rate | 48.1% |
| Wins | 238 |
| Losses | 257 |
| Profit Factor | **1.34** |
| Sharpe Ratio | **1.13** |
| Max Drawdown | **-16.5%** from peak equity |
| Avg Win | +2.81% ($892 avg) |
| Avg Loss | -1.77% ($617 avg) |
| Model Win Rate | 54.2% (trained on 3,117 days) |
| Short Signal Win Rate | 51.8% |

---

## Annual Returns

| Year | Jan | Feb | Mar | Apr | May | Jun | Jul | Aug | Sep | Oct | Nov | Dec | Year Total |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 2018 | n/a | n/a | n/a | n/a | n/a | n/a | +0.1% | +9.5% | -0.7% | -2.2% | +6.9% | +12.8% | **+26.4%** |
| 2019 | +0.6% | -6.3% | -5.8% | +6.9% | +18.5% | +24.7% | +5.0% | +1.3% | +0.1% | +0.3% | +9.1% | +6.2% | **+58.6%** |
| 2020 | +1.7% | +6.9% | +7.7% | +3.4% | +4.1% | +0.2% | +4.6% | +2.1% | -11.0% | +26.0% | +22.9% | +31.8% | **+100.4%** |
| 2021 | +13.8% | +37.3% | -5.0% | +1.7% | +42.6% | -15.3% | +0.2% | +26.3% | -18.9% | +41.5% | -14.0% | +30.6% | **+140.2%** |
| 2022 | +31.1% | -23.3% | -9.4% | +3.4% | +14.5% | +45.0% | -11.0% | +8.4% | -15.1% | -14.5% | -2.3% | -3.8% | **+23.1%** |
| 2023 | +48.8% | -26.3% | +11.5% | -13.2% | -3.0% | +10.1% | +0.5% | -8.3% | -15.6% | +23.4% | -2.1% | +11.8% | **+37.6%** |
| 2024 | -1.3% | +64.1% | +26.0% | -1.6% | +19.0% | +18.8% | -2.1% | -5.7% | -4.4% | +0.1% | +46.5% | -22.7% | **+136.6%** |
| 2025 | -25.3% | +15.5% | -33.1% | -19.1% | +41.8% | -26.4% | +26.7% | +1.9% | -10.8% | -6.1% | +17.2% | -0.5% | **-18.3%** |
| 2026 | +2.1% | +52.5% | -22.3% | n/a | n/a | n/a | n/a | n/a | n/a | n/a | n/a | n/a | **+32.3%** |

---

## Signal Distribution (Last 1 Year)

| Signal | Count | Avg Composite Score |
|---|---|---|
| LONG | 91 | 75% |
| SHORT | 111 | 21% |
| FLAT (No Trade) | 163 | n/a |
| Total Candles | 365 | n/a |

---

## Exit Reason Breakdown

Trades exit via one of four conditions in priority order:

| Exit Reason | Description |
|---|---|
| TP | Take Profit hit at +6% from entry |
| SL | Stop Loss hit at -3% from entry |
| MAX HOLD | 5 day max hold period expired |
| SIGNAL | Opposite signal fired before TP or SL |

---

## First 27 Trades (Jul 2018 to Dec 2018)

| # | Entry | Exit | Type | Entry $ | Exit $ | Reason | P&L $ | P&L % | Portfolio $ |
|---|---|---|---|---|---|---|---|---|---|
| 1 | 20 Jul 18 | 24 Jul 18 | LONG | $7,338 | $7,778 | TP | +$393 | +3.94% | $10,387 |
| 2 | 24 Jul 18 | 26 Jul 18 | LONG | $8,397 | $8,145 | SL | -$215 | -2.07% | $10,165 |
| 3 | 26 Jul 18 | 31 Jul 18 | LONG | $7,920 | $7,731 | MAX HOLD | -$169 | -1.66% | $9,990 |
| 4 | 03 Aug 18 | 06 Aug 18 | SHORT | $7,419 | $6,974 | TP | +$393 | +3.94% | $10,376 |
| 5 | 06 Aug 18 | 08 Aug 18 | SHORT | $6,935 | $6,519 | TP | +$408 | +3.94% | $10,777 |
| 6 | 08 Aug 18 | 09 Aug 18 | SHORT | $6,285 | $6,474 | SL | -$223 | -2.07% | $10,547 |
| 7 | 09 Aug 18 | 14 Aug 18 | SHORT | $6,530 | $6,188 | MAX HOLD | +$361 | +3.42% | $10,901 |
| 8 | 14 Aug 18 | 17 Aug 18 | SHORT | $6,188 | $6,374 | SL | -$225 | -2.07% | $10,669 |
| 9 | 17 Aug 18 | 22 Aug 18 | SHORT | $6,584 | $6,361 | MAX HOLD | +$234 | +2.20% | $10,896 |
| 10 | 29 Aug 18 | 03 Sep 18 | LONG | $7,031 | $7,263 | MAX HOLD | +$232 | +2.13% | $11,121 |
| 11 | 03 Sep 18 | 05 Sep 18 | LONG | $7,263 | $7,045 | SL | -$230 | -2.07% | $10,884 |
| 12 | 07 Sep 18 | 12 Sep 18 | SHORT | $6,396 | $6,339 | MAX HOLD | +$57 | +0.53% | $10,934 |
| 13 | 12 Sep 18 | 17 Sep 18 | SHORT | $6,339 | $6,249 | MAX HOLD | +$96 | +0.88% | $11,023 |
| 14 | 17 Sep 18 | 20 Sep 18 | SHORT | $6,249 | $6,436 | SL | -$228 | -2.07% | $10,787 |
| 15 | 12 Oct 18 | 15 Oct 18 | SHORT | $6,298 | $6,487 | SL | -$223 | -2.07% | $10,557 |
| 16 | 28 Oct 18 | 02 Nov 18 | SHORT | $6,490 | $6,434 | MAX HOLD | +$54 | +0.51% | $10,604 |
| 17 | 02 Nov 18 | 07 Nov 18 | SHORT | $6,434 | $6,578 | MAX HOLD | -$166 | -1.56% | $10,431 |
| 18 | 15 Nov 18 | 19 Nov 18 | SHORT | $5,753 | $5,408 | TP | +$410 | +3.94% | $10,834 |
| 19 | 19 Nov 18 | 20 Nov 18 | SHORT | $4,910 | $4,615 | TP | +$426 | +3.94% | $11,253 |
| 20 | 20 Nov 18 | 24 Nov 18 | SHORT | $4,559 | $4,285 | TP | +$443 | +3.94% | $11,688 |
| 21 | 24 Nov 18 | 25 Nov 18 | SHORT | $3,932 | $4,050 | SL | -$242 | -2.07% | $11,439 |
| 22 | 25 Nov 18 | 28 Nov 18 | SHORT | $4,086 | $4,208 | SL | -$236 | -2.07% | $11,195 |
| 23 | 28 Nov 18 | 03 Dec 18 | SHORT | $4,265 | $4,009 | TP | +$440 | +3.94% | $11,628 |
| 24 | 03 Dec 18 | 06 Dec 18 | SHORT | $3,884 | $3,651 | TP | +$457 | +3.94% | $12,077 |
| 25 | 06 Dec 18 | 11 Dec 18 | SHORT | $3,509 | $3,380 | MAX HOLD | +$287 | +2.37% | $12,356 |
| 26 | 11 Dec 18 | 16 Dec 18 | SHORT | $3,380 | $3,229 | MAX HOLD | +$361 | +2.93% | $12,709 |
| 27 | 16 Dec 18 | 17 Dec 18 | SHORT | $3,229 | $3,326 | SL | -$263 | -2.07% | $12,438 |

---

All results are from backtesting on historical Binance data. Past performance does not guarantee future results. This is not financial advice.

Source code is private. Available for review upon request.

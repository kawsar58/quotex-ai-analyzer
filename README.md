# AI Trading Analyzer — Free-first Android MVP

## Free live market analysis added
The Android app now includes a rule-based live analyzer using Binance's public spot market-data endpoint:
`https://data-api.binance.vision/api/v3/klines`
No API key is required for these public market-data endpoints.

Initial symbols: BTCUSDT, ETHUSDT, SOLUSDT.
Timeframes: 1m, 5m, 15m.
Indicators: EMA 9, EMA 21, RSI 14, one-candle momentum.
Output is a simple rule-based bias, not a calibrated prediction.

## Important market distinction
These are real crypto spot market candles, NOT Quotex OTC candles and NOT EUR/USD Forex candles. Exchange prices can differ from other venues. No trade execution is included.

## Screenshot AI
Screenshot picker and backend upload scaffold are included. Cloud AI screenshot analysis requires an API key and may incur cost. For fully free use, use live-data analysis first; local screenshot vision would need a separate on-device model integration.

## Live screen capture status
The app requests Android MediaProjection permission, but continuous frame capture/foreground service and frame analysis are not implemented yet.

## Build APK
Open the project in Android Studio, sync Gradle, then Build > Build Bundle(s) / APK(s) > Build APK(s). Android SDK/Gradle must be installed. This source package is not itself an APK.

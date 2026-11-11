# Contributing to aapl-expiration-tracker

Thanks for your interest in contributing to this weekly AAPL options expiration tracker for the risk meeting.

## Adding expirations.md updates weekly

1. Confirm you have a **fresh AAPL share price** from the data source.
2. List the **three soonest upcoming option expirations** (skip anything earlier than today).
3. For each expiration, compute:
   - ATM strike (closest strike to the current share price)
   - Call strike with the **highest open interest**
   - Put strike with the **highest open interest**
   - Use the share price you used for ATM determination in the issue body
4. Open a **pull request** from a feature branch (e.g. `tracking/<date>-stream`) into `main`.
5. Create tracking issues in date order, titled `Expiry YYYY-MM-DD`, each with:
   - that expiration's ATM strike
   - highest-OI call strike
   - highest-OI put strike
   - the share price used

## Notes

- All market figures must come from **live data** — report exactly what the source returns (no rounding, no external adjustments).
- Report any odd numbers (very high premiums at deep ITM strikes, unusual strike step intervals) exactly as returned.
- Keep `expirations.md` at the repo root and keep the summary table in sync with the issue bodies.

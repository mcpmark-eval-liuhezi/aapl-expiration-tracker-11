# Contributing to AAPL Expiration Tracker

Thanks for your interest in contributing!

## Local Setup

Clone the repo and create a feature branch for each change:

```bash
git clone https://github.com/mcpmark-eval-liuhezi/aapl-expiration-tracker-11.git
cd aapl-expiration-tracker-11
git switch -c <short-descriptive-name>
```

## Pull Requests

1. Make changes on a feature branch.
2. Open a pull request against `main`.
3. All market figures must come from **live data** — never paste stale numbers from a previous week without re-checking.
4. Report any number that looks odd exactly as the source returned it.

## Rule of thumb

Keep weekly AAPL expiration tracking simple and sourceable: snapshot, expiration list, per-expiration stats (ATM strike, highest-OI call strike, highest-OI put strike), and the share price used.

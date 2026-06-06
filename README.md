# 🏥 GitScope Repo Health Action

Automatically add a **live repo health badge** to your GitHub README.

## Usage

Create `.github/workflows/gitscope.yml`:

```yaml
name: GitScope Badge
on:
  push:
    branches: [main, master]
  schedule:
    - cron: '0 0 * * 1'  # Weekly

jobs:
  badge:
    runs-on: ubuntu-latest
    steps:
      - uses: promptpolish-ai/gitscope-action@v1
```

## What it does

Adds this badge to your README:

[![Repo Health](https://gitscope-micro.vercel.app/api/badge?repo=promptpolish-ai/gitscope-action)](https://gitscope-micro.vercel.app/api/deliver?repo=promptpolish-ai/gitscope-action)

The badge shows your repo's health score (0-100) and updates every time the action runs.

## Why?

- **Free** - No cost, no signup
- **Live** - Updates with your code
- **Shareable** - Shows your maintainers you care about quality

---

*Powered by [GitScope](https://gitscope-micro.vercel.app) — free repo analysis*

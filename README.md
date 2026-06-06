# GitScope GitHub Action 📊

Generate **beautiful HTML reports** from any git repository — directly in your CI/CD pipeline.

[![GitScope](https://img.shields.io/badge/GitScope-Micro-%241-brightgreen)](https://gitscope-micro.vercel.app)
[![GitScope Pro](https://img.shields.io/badge/GitScope-Pro-%245-purple)](https://gitscope-pro.vercel.app)

## 🚀 Quick Start

Add this to `.github/workflows/report.yml`:

```yaml
name: GitScope Report

on:
  push:
    branches: [main]
  workflow_dispatch:

jobs:
  report:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
        with:
          fetch-depth: 0
      
      - name: Generate Report
        uses: promptpolish-ai/gitscope-action@v1
```

That's it! Every push generates a beautiful HTML report of your repository.

## 🎨 Features

- **Zero configuration** — works with any repo
- **Beautiful design** — typography, layout, dark mode
- **Rich stats** — commits, contributors, languages
- **CI/CD native** — runs in your GitHub Actions pipeline
- **Artifact upload** — report available as build artifact

## 💰 Premium Templates

Get **5 premium report templates** for **$5 BTC**:

| Template | Description |
|----------|-------------|
| **Timeline** | Chronological commit visualization |
| **Heatmap** | Contribution intensity map |
| **Authors** | Individual contributor reports |
| **Stats** | Repository analytics dashboard |
| **Changelog** | Automated release notes generator |

```
BTC: 1DQXcKwN95AWqwmwbscG7fRbEYMdWU9GB3
```

## 📄 License

MIT — open source, free for all repos.

---

Made with ❤️ by [GitScope](https://gitscope-micro.vercel.app)

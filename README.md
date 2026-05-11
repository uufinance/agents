# Claude Code Workshop — USE Finance

A 60-minute hands-on introduction to AI coding agents for finance researchers at Utrecht School of Economics.

**Live site:** https://uufinance.github.io/agents/

## Contents

```
agents/
├── index.html                  # Full workshop site (single-page, no build step)
├── assets/
│   └── compustat_sample.csv    # Synthetic Compustat-style extract (725 rows)
└── README.md
```

## Deploy to GitHub Pages

1. Go to **Settings → Pages** in this repository.
2. Under **Source**, select **Deploy from a branch**.
3. Choose branch `main`, folder `/ (root)`.
4. Click **Save**. The site will be live at `https://uufinance.github.io/agents/` within ~60 seconds.

No build step, no Jekyll, no npm — GitHub Pages serves `index.html` directly.

## Local preview

```bash
# Any static file server works:
npx serve .
# or
python3 -m http.server 8000
```

Open `http://localhost:8000` in a browser.

## Demo data

`assets/compustat_sample.csv` contains 725 synthetic firm-year observations from 25 European firms (1995–2023) with columns matching a real WRDS/Compustat annual pull: `gvkey`, `conm`, `fyear`, `ni`, `at`, `rect`, `invt`, `dpc`, `oancf`. Participants can download it directly from the workshop site or clone the repo.

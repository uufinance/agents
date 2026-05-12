# Claude Code Workshop — AI Coding Agents for Researchers

A 60-minute hands-on workshop for researchers at the Utrecht School of Economics. No programming experience required.

**Live slide deck:** https://uufinance.github.io/agents/

## What this workshop covers

Claude Code is an AI coding agent that runs in your terminal, reads your files, writes and executes code, and iterates — without you driving every step. This workshop shows researchers how to use it for:

- **Research workflows** — referee reports, R&R revision plans, conference slide decks, cross-language code replication (Stata → Python + R)
- **Teaching & admin** — building academic homepages from a CV, transcribing student meetings, creating interactive exam and competition tools
- **Concepts** — how AI agents work (ReAct loop, tools, memory), plan mode, permission levels, context windows, usage limits

## Repo contents

```
agents/
├── index.html              # Full slide deck (single HTML file, no build step)
├── assets/
│   └── compustat_sample.csv  # Synthetic Compustat extract for live demos
└── .claude/
    └── skills/
        └── transcribe-meeting.md  # Local skill used in Demo 6
```

## View locally

```bash
npx serve .
# or
python3 -m http.server 8000
```

Open `http://localhost:8000`.

## Demo data

`assets/compustat_sample.csv` — 725 synthetic firm-year observations from 25 European firms (1995–2023). Columns match a real WRDS/Compustat annual pull: `gvkey`, `conm`, `fyear`, `ni`, `at`, `rect`, `invt`, `dpc`, `oancf`. Used in the live demos; participants can download it directly from the workshop site.

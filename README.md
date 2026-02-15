# Game of Life

Conway’s Game of Life with optional real-time AI commentary (Claude).  
Minimal design. Clean architecture. Intuitive controls.

---

## Overview

A deterministic cellular automaton implemented as a single-file web application.  
No frameworks. No build tools. Runs directly in the browser.

---

## Project Structure

```
gol-project/
├── GFL.html      ← toda la app (HTML + CSS + JS)
└── README.md
```

Single-file architecture for simplicity and portability.

---

## Option 1 — Without AI (Game Only)

No installation required.  
Open `GFL.html` directly in your browser.

If AI Commentary is enabled without a valid key or backend, a notice will be displayed.

---

## Option 2 — With AI (Claude Analysis)

### Step 1 — Get Your Anthropic API Key

1. Go to https://console.anthropic.com  
2. Sign in or create an account  
3. Navigate to **API Keys**  
4. Click **Create Key**  
5. Name it (e.g., `game-of-life`)  
6. Copy the key (starts with `sk-ant-api03-...`)

> **Cost:** Uses Claude Haiku (low-cost model).  
> Approx. $0.0001 USD per analysis.  
> $1 ≈ ~10,000 analyses.

> ⚠️ Never commit your API key to GitHub. It is private.

---

## Controls

| Key | Action |
|-----|--------|
| `Space` | Play / Pause |
| `→` | Step forward |
| `C` | Clear grid |
| `R` | Random grid |
| Click + drag | Draw cells |

---

## Conway’s Four Rules

1. **Underpopulation**  
   Live cell with fewer than 2 neighbors → dies  

2. **Survival**  
   Live cell with 2–3 neighbors → lives  

3. **Overpopulation**  
   Live cell with more than 3 neighbors → dies  

4. **Reproduction**  
   Dead cell with exactly 3 neighbors → becomes alive  

Deterministic once initialized.

---

## Troubleshooting

**API key not working?**
- Ensure the full key was copied correctly.
- Newly created keys may take 1–2 minutes to activate.

---

Built by Alain · Conway’s Game of Life · 2026

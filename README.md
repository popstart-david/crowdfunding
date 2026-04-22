# Popstart — Crowdfunding Pre-Launch Action Plan

Interactive chat agent for the Popstart platform. Module 3 — Funding.

## What it does

Guides a founder through a 20–35 minute structured session and produces four ready-to-use deliverables:

1. **Campaign Brief** — what is being raised, why now, funding goal, platform, coverage
2. **Committed Backer Strategy** — first-backer plan segmented by network group with outreach approach
3. **Reward Tier Structure** — three-tier framework (Lower / Main / Premium) with price points
4. **Campaign Launch Timeline** — sequenced pre-launch and launch schedule

## How to deploy

### Option A — GitHub Pages (recommended, free)

1. Create a new repository (e.g. `crowdfunding-agent`)
2. Upload `index.html` to the root of the repository
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch`
5. Set branch to `main`, folder to `/ (root)`
6. Click **Save**
7. Wait ~60 seconds — your URL will be: `https://YOUR_USERNAME.github.io/crowdfunding-agent/`

### Option B — Replace existing agent

1. Go to your existing repo
2. Click the current `index.html` → pencil icon
3. Delete all content, paste in the new file
4. Commit changes — your existing URL updates in ~60 seconds

## Files

| File | Purpose |
|------|---------|
| `index.html` | Complete self-contained chat agent — deploy this |
| `README.md` | This file |
| `.gitignore` | Standard web project ignores |

## Agent spec

- **Module:** 3 — Funding
- **Section:** Crowdfunding
- **Depth modes:** Quick / Standard / Deep (currently Standard)
- **Web search:** Disabled — no live data required
- **Thread cap:** 80 exchanges (soft warning at 65)
- **Adjacent agents:** Funding Strategy, Working Capital Estimator, Business Plan, Marketing Strategy

## Gap detection

The agent monitors for six key blind spots and surfaces coaching probes at natural points:

1. Goal not grounded in real costs
2. No committed backers before launch
3. Reward tiers not connected to real value
4. Platform choice uninformed
5. Timeline too compressed against list size
6. No mid-campaign momentum plan

## Technical notes

- Pure HTML/CSS/JS — no build step, no dependencies, no backend
- All session data is held in memory — nothing is stored or transmitted
- Fonts loaded from Google Fonts (requires internet connection)
- Export function generates a plain text `.txt` download

## Version

v1.0 — Initial release  
Agent Design Document: `Popstart_Crowdfunding_ADD_v1.docx`

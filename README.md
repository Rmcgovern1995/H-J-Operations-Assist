# H‑J Operations Assist

Offline‑first PWA & desktop app for routing, inventory, and payer reimbursement look‑ups.

## Build v2.1

* **dist.zip** – double‑click `index.html` (browser) or run `npm run electron`  
  * SHA‑256: `ac13084670e78d4aa38e89549fbb892043d60d3d8acf3ad089765fa00502020d`

## Data sources
| File | Purpose |
|------|---------|
| Medicare allowables.csv | CMS fee schedule |
| Medicaid Allowables.csv | NY Medicaid allowables |
| Commercial Allowables.csv | Commercial payer reference |
| Driver assist.xlsx | Driver‑log ledger |

## Nightly auto‑ingest

`.github/workflows/data-refresh.yml` converts fresh CSV/XLSX files into JSON every night at 01:00 UTC and commits changes automatically.

## Roadmap (v2.2)

* Drag‑and‑drop CSV ingest in‑app  
* Keyboard shortcuts & accessibility polish  
* Dark‑mode settings panel  
* Performance target: FCP ≤ 1.5 s

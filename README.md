# Wedding Budget Planner

A personal wedding financial command center — tracking itemized expenses, loan repayments, monthly cash flow, and savings goals for April 29, 2026.

## Features

- **Itemized Expense Tracker** — Categorized wedding items with inline editing, payment source tracking, and status management
- **Loan & Goal Planner** — Friend loan, bank personal loan tracking with EMI calculator and Japan Trip 2027 savings goal
- **Monthly Cash Flow** — Editable income vs. expenses breakdown with surplus calculation
- **Persistent Data** — All changes auto-save to `localStorage`. Your data survives page refreshes and browser restarts.
- **Backup & Restore** — Export/import full state as JSON for cross-device backup
- **Voice Commands** — Dictate expenses with `⌘K` / `Ctrl+K` (e.g., "add decoration expenses 50000", "mark photography as paid")
- **CSV Export** — Download expense table as spreadsheet

## Usage

Open `index.html` in any modern browser. No build step required — runs entirely client-side with React 18, Tailwind CSS, and Babel via CDN.

### Data Management (top-right menu)

| Action | Description |
|--------|-------------|
| **Backup (JSON)** | Download all data as a JSON file |
| **Restore Backup** | Load a previously exported JSON backup |
| **Export CSV** | Download expenses as a CSV spreadsheet |
| **Reset to Defaults** | Revert all data to initial seed values |

### Voice Commands (`⌘K` / `Ctrl+K`)

- `add [category] [item name] [amount]` — Add a new expense
- `paid [amount] for [item]` — Record a payment
- `mark [item] as paid` — Mark an item fully paid
- `remove [item]` — Delete an item
- `set [field] to [amount]` — Update cash flow fields (rent, income, SIP, etc.)

## Hosting

Deploy via **GitHub Pages** — push to `main` branch and enable Pages in repo settings (source: root `/`).

## Tech Stack

Single-file HTML — React 18 + Tailwind CSS + Babel (CDN), localStorage for persistence, Web Speech API for voice input.

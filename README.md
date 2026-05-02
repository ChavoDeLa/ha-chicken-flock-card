# 🐔 Chicken Flock Card

[![HACS Frontend](https://img.shields.io/badge/HACS-Frontend-blue.svg)](https://github.com/hacs/integration)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/ChavoDeLa/ha-chicken-flock/blob/main/LICENSE)

Lovelace custom card for the [Chicken Flock](https://github.com/ChavoDeLa/ha-chicken-flock) Home Assistant integration.

> **Requires the Chicken Flock integration to be installed first.**
> Install it from HACS → Integrations, or manually from [ha-chicken-flock](https://github.com/ChavoDeLa/ha-chicken-flock).

---

## Screenshots

![Active flock view with photos and egg counters](https://raw.githubusercontent.com/ChavoDeLa/ha-chicken-flock/main/screenshots/active_tab.png)

![Statistics tab showing 9,867 all-time eggs](https://raw.githubusercontent.com/ChavoDeLa/ha-chicken-flock/main/screenshots/statistics_tab.png)

![History tab with stacked colour bars per hen](https://raw.githubusercontent.com/ChavoDeLa/ha-chicken-flock/main/screenshots/history_tab.png)

---

## Installation via HACS

1. In HACS, go to **Frontend → ⋮ → Custom repositories**
2. Add `https://github.com/ChavoDeLa/ha-chicken-flock-card` as **Lovelace**
3. Find **Chicken Flock Card** and install
4. Refresh your browser

HACS will automatically place the card in `config/www/` and manage updates.

---

## Manual installation

Copy `chicken-flock-card.js` to `config/www/`, then register it as a resource:

```yaml
lovelace:
  resources:
    - url: /local/chicken-flock-card.js?v=1
      type: module
```

---

## Usage

Add to any dashboard:

```yaml
type: custom:chicken-flock-card
```

No configuration options required. All settings — including colour theme — are in the card's ⚙ Settings tab.

---

## Features

- **Active / All birds tabs** — flock cards with photos, breed, age, status badges, live +/− egg counters
- **Statistics** — all-time, yearly, monthly, weekly totals; per-hen leaderboard; breakdown table with year picker
- **History** — stacked colour bar chart filterable by year / month / week / day; ✎ Edit for correcting past records
- **Export** — CSV, JSON, full backup and restore
- **Import** — CSV/TSV from FLOCKSTAR or any spreadsheet tracker
- **Theme settings** — 5 colour presets or fully custom colours

---

## Links

- **Integration repo:** [ChavoDeLa/ha-chicken-flock](https://github.com/ChavoDeLa/ha-chicken-flock)
- **Issues:** [github.com/ChavoDeLa/ha-chicken-flock/issues](https://github.com/ChavoDeLa/ha-chicken-flock/issues)

---

## Credits

Built with [Claude](https://claude.ai) by [ChavoDeLa](https://github.com/ChavoDeLa).

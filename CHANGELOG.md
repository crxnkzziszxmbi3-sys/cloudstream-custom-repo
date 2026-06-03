# Changelog

All notable changes to this repository will be documented in this file.

Format based on [Keep a Changelog](https://keepachangelog.com/).

---

## [1.2.0] - 2026-06-03

### Maintenance Run — 14-Day Active-Agent Check #1

#### Replaced
- **Rowdy-Avocado** → **Kraptor123/Cs-Karma**
  - Rowdy-Avocado: UNREACHABLE_CYCLE_2 — GitHub repository does not exist, no forks found.
  - Replacement selected: `Kraptor123/Cs-Karma` — 35 plugins, EN/MX/TR content, actively maintained (last push: 2026-06-03), 35 GitHub stars.
  - New URL: `https://raw.githubusercontent.com/Kraptor123/Cs-Karma/builds/plugins.json`

#### Confirmed OK
- `hexated` — HTTP 200, 64 plugins, JSON valid
- `MegaRepo` — HTTP 200, manifest v1, JSON valid
- `phisher98` — HTTP 200, manifest v1, JSON valid

#### Infrastructure
- 14-day automated health check automation created (runs every 14 days at 09:00 Europe/Berlin)
- Automation covers: URL reachability, JSON validity, structural consistency, auto-repair, auto-replacement

---

## [1.1.0] - 2026-06-03

### Maintenance Run — First Monthly Check

#### Fixed
- `hexated`: URL corrected from `repo.json` → `plugins.json` (was HTTP 404, now 200)
- `phisher98`: URL simplified — removed `refs/heads/` path segment (clean builds URL)

#### Flagged
- `Rowdy-Avocado`: UNREACHABLE_CYCLE_1 — GitHub repository returns 404. Entry retained.

#### Changed
- `repo.json`: Added `_maintenance` block for audit trail.
- `README.md`, `TASK.md`, `RELEASE_CHECKLIST.md`: Updated per maintenance run.

---

## [1.0.0] - 2026-06-03 (Initial Setup)

### Added
- Initial repository structure
- Base manifest with 4 provider repositories (hexated, MegaRepo, phisher98, Rowdy-Avocado)
- `repo.json` manifest v1
- All documentation files
- Agent identity files

### Known Issues at Release
- hexated URL → fixed in v1.1.0
- phisher98 URL → fixed in v1.1.0
- Rowdy-Avocado offline → replaced in v1.2.0

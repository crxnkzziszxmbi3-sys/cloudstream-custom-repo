# CloudStream Custom Repository

Curated CloudStream aggregator manifest for Fire TV, Android TV, and mobile devices.

## Status

| Field | Value |
|---|---|
| **Manifest Version** | 1 |
| **Repo Version** | 1.2.0 |
| **Update Cycle** | Every 14 days (automated) |
| **Last Verified** | 2026-06-03 |
| **Healthy Sources** | 4/4 |

---

## Included Repositories

| # | Name | Status | Plugins | URL |
|---|---|---|---|---|
| 1 | **Hexated** | ✅ REACHABLE | 64 | `https://raw.githubusercontent.com/hexated/cloudstream-extensions-hexated/builds/plugins.json` |
| 2 | **MegaRepo** | ✅ REACHABLE | 1 list | `https://raw.githubusercontent.com/self-similarity/MegaRepo/builds/repo.json` |
| 3 | **Phisher** | ✅ REACHABLE | 1 list | `https://raw.githubusercontent.com/phisher98/cloudstream-extensions-phisher/builds/repo.json` |
| 4 | **Cs-Karma** | ✅ REACHABLE | 35 | `https://raw.githubusercontent.com/Kraptor123/Cs-Karma/builds/plugins.json` |

> **v1.2.0 Change:** Rowdy-Avocado was removed (UNREACHABLE_CYCLE_2 — repository deleted on GitHub).
> Replaced by **Kraptor123/Cs-Karma**: 35 EN/MX/TR plugins, actively maintained, last push 2026-06-03.

---

## Quick Start

### Fire TV / Android TV

1. Install CloudStream (latest stable or pre-release)
2. Open **Settings → Extensions → Add Repository**
3. Enter the raw URL to this `repo.json`:
   ```
   https://raw.githubusercontent.com/YOUR_USER/YOUR_REPO/BRANCH/repo.json
   ```
   *(Replace `YOUR_USER`, `YOUR_REPO`, `BRANCH` with your GitHub details)*
4. Download and install desired extensions
5. Enable **NSFW Extensions** in Plugin Settings if required

---

## Prerequisites

- CloudStream 4.x or newer
- VPN recommended for some providers
- Stable internet connection

---

## Troubleshooting

| Issue | Fix |
|---|---|
| "Invalid files" | Clear app cache; check CloudStream version |
| Repo not loading | Verify raw URL is correct; try VPN |
| Extensions not showing | Enable NSFW in Plugin Settings |
| No links found | Extension may be down; try alternative from repo |
| 404 on URL | Branch name may have changed; next auto-check will detect and repair |

---

## Automated Maintenance

This repository is maintained by an automated agent:
- **Check interval:** Every 14 days
- **Auto-repairs:** URL path/branch corrections, JSON fixes
- **Auto-replacement:** Dead sources replaced after 2 consecutive failed checks
- **Human review required:** >50% entries affected, legal concerns, breaking changes

---

## Safety Notes

- Use only legal, authorized sources
- VPN usage recommended for privacy
- Repository URLs are auto-verified every 14 days

---

## Version History

See [`CHANGELOG.md`](CHANGELOG.md) for full version history.
See [`MAINTENANCE.md`](MAINTENANCE.md) for maintenance procedures.

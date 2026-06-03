# Release Checklist — v1.1.0 (2026-06-03)

## Pre-Release

- [x] All JSON files validated (syntax + schema) — repo.json: PASS
- [x] All URLs verified reachable — 3/4 PASS, 1 UNREACHABLE_CYCLE_1 (Rowdy-Avocado)
- [x] `repo.json` manifestVersion set correctly — v1 confirmed
- [x] `README.md` updated with current status and verified URLs
- [x] `CHANGELOG.md` updated — v1.0.0 and v1.1.0 documented
- [x] No unresolved TODO/PLACEHOLDER in agent-managed files
- [ ] TODO_OPERATOR: Rowdy-Avocado replacement not yet found (non-blocking for v1.1.0)

## GitHub / Codeberg Publication

- [ ] TODO_OPERATOR: Repository created on GitHub (or Codeberg)
- [ ] TODO_OPERATOR: Files committed to main/master branch
- [ ] TODO_OPERATOR: Raw URLs confirmed working (test in browser)
- [ ] TODO_OPERATOR: Branch protection considered (recommended: protect main)

## CloudStream Testing

- [ ] TODO_OPERATOR: CloudStream app updated to latest version
- [ ] TODO_OPERATOR: App cache cleared before adding repo
- [ ] TODO_OPERATOR: Repository added via raw repo.json URL
- [ ] TODO_OPERATOR: Extensions downloadable from at least hexated and phisher98
- [ ] TODO_OPERATOR: At least one video stream tested end-to-end
- [ ] TODO_OPERATOR: NSFW extensions enabled in Settings if applicable

## Post-Release

- [x] `CHANGELOG.md` finalized with release date
- [x] `MAINTENANCE.md` — procedures unchanged, no update needed
- [x] Next maintenance scheduled: ~2026-07-03
- [ ] TODO_OPERATOR: Notify yourself / set calendar reminder for next check

## Rollback Plan

If release fails after GitHub push:
1. Revert to last known stable commit (v1.0.0 tag)
2. Update `repo.json` pluginLists to remove any broken entries
3. Document issue in `CHANGELOG.md` under `[1.1.1-hotfix]`
4. Schedule immediate fix run (do not wait for monthly cycle)

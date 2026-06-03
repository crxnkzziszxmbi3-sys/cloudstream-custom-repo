# Maintenance Guide - Monthly Recurring Tasks

## Schedule

- **Standard**: Once per month
- **Trigger**: Manual override available anytime
- **Emergency**: Run immediately if multiple providers fail

## Recurring Task List

### 1. Repository Health Check
- Verify `repo.json` is valid JSON
- Check all `pluginLists` URLs are reachable (HTTP 200)
- Confirm core project files exist

### 2. Change Detection
- Compare current entries against upstream sources
- Flag new, modified, or removed providers
- Separate confirmed changes from unverified assumptions

### 3. Update Proposal
- Create precise diff-style change proposal
- Show what to add, change, or remove
- Provide justification for each change

### 4. Artifact Update
Update at minimum:
- `repo.json`
- `README.md`
- `CHANGELOG.md`
- `MAINTENANCE.md` (if procedures change)

### 5. Validation
- Validate JSON syntax
- Check for obvious URL errors
- Verify name/ID/reference consistency
- Generate validation report

### 6. Risk Analysis
- Mark potentially unstable sources
- List entries needing manual verification
- Flag breaking-change risks

### 7. Operator Handover
- Summarize maintenance run
- List changes, open issues, recommended next steps
- Request human approval if uncertainty exists

## Change Policy

- Only auto-accept high-plausibility changes
- Never remove existing entries without marking and justification
- If uncertain, mark as REVIEW_REQUIRED
- Prefer stability over completeness
- If >20% of entries affected, stop for review

## Failure Handling

| Scenario | Action |
|----------|--------|
| Source unreachable | Mark UNREACHABLE, retry next cycle, remove only after 2 failed runs |
| JSON invalid | Fix syntax, document correction |
| Conflicting entries | Prefer last confirmed stable version, flag alternatives |
| Breaking upstream change | Mark REVIEW_REQUIRED, do not auto-apply |

## Monthly Deliverables

Every maintenance run must produce:
1. Maintenance report
2. Change proposal
3. Updated artifacts or patch blocks
4. Review list

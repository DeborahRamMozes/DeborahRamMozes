# REPOSITORY_PROTECTION_POLICY.md
## ATOR GitHub Protection Policy - 2026-09-09

**Principle:** GitHub is archive infrastructure only when refusal is mechanical.

### Required Ruleset: ATOR-main-archive-protection
- **Name:** `ATOR-main-archive-protection`
- **Enforcement:** Active (not Evaluate)
- **Target:** Include default branch + exact `main`
- **Bypass list:** Empty, or owner only (@DeborahRamMozes)

### Branch rules to enable
- Restrict deletions: ON
- Restrict force pushes / Block force pushes: ON
- Require a pull request before merging: ON
- Required approvals: 1 minimum
- Require review from Code Owners: true (after CODEOWNERS exists)
- Dismiss stale pull request approvals when new commits are pushed: true
- Require conversation resolution before merging: true
- Require linear history: true (recommended)
- Require signed commits: where practical
- Require status checks: after workflows exist (repository-integrity-audit)

### What is NOT protection
- Open settings page without Active status
- Written policy file without Ruleset
- Memory / goodwill / careful clicking

A repository is protected only when: ruleset exists + active + target branch configured + deletion/force-push restricted + PR/approval enforced.

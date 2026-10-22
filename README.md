# security-hygiene-tracker

Tracker for the security hygiene audit of the HeziLiu GitHub account.
Follow-up items are tracked as sub-issues of the parent issue "Security hygiene audit".

---

## Audit summary

### 1. Account confirmed

- **Login:** HeziLiu
- **Numeric user ID:** 28861483
- **Profile:** https://github.com/HeziLiu
- **Sweep date:** 2026-10-22

### 2. Repository inventory (4 repositories owned, all public)

| Repository | Visibility | README on default branch | Notes |
|---|---|---|---|
| Little-rookie | Public | Yes | Undergraduate coursework; default branch `master`; last pushed 2019-06-02 |
| CodingInterviewChinese2 | Public | **No** | Fork; default branch `master`; last updated 2019-03-12 |
| awesome-chatgpt-prompts-zh | Public | Yes | Fork; default branch `main`; last updated 2023-04-14 |
| Big-Buzzard | Public | **No** | Near-empty; default branch `master`; only `.gitattributes` + an empty file; last updated 2018-05-17 |

No private repositories were found (search for `is:private` under this account returned zero results).

**Repositories missing a README:** `CodingInterviewChinese2`, `Big-Buzzard`

### 3. Secret-scanning findings

| Repository | Open secret-scanning alerts |
|---|---|
| Little-rookie | **Could not be read — access denied** |
| CodingInterviewChinese2 | **Could not be read — access denied** |
| awesome-chatgpt-prompts-zh | **Could not be read — access denied** |
| Big-Buzzard | **Could not be read — access denied** |

**Important caveat:** every attempt to list and to fetch individual secret-scanning alerts on all four repositories was rejected by the GitHub API with `403 Resource not accessible by personal access token`. This endpoint requires a token with the `security_events` scope (and secret scanning to be enabled/permissioned on the repositories). As a result, **no "clean" finding can be claimed** — the absence of alerts could not be verified either way. This check must be re-run with an appropriately scoped token (or via the Security tab on each repository) before the audit is signed off.

### 4. Organization teams

- **Organization:** `mcpmark-eval-liuhezi` — the account is a member of this organization.
- **Teams:** the account does **not** belong to any team within that organization (team list returned empty).
- No other organization memberships were returned.

### 5. Follow-ups tracked

See the parent issue "Security hygiene audit" and its sub-issues:
- Rotate any exposed credentials
- Review repository collaborator access

---

*This README replaces the starter README that came with the repository.*

# gstack

Use the `/browse` skill from gstack for all web browsing. Never use `mcp__claude-in-chrome__*` tools.

## /OG — Master Router (start here)

Use `/OG` to describe what you want in plain English. It routes to the right gstack skill(s) automatically, running independent skills in parallel via Agent tool when possible.

Example usage:
- `/OG review and ship this` → runs /review then /ship sequentially
- `/OG plan review from CEO and eng perspectives` → runs /plan-ceo-review + /plan-eng-review in parallel
- `/OG QA the site and review the code` → runs /qa + /review in parallel
- `/OG` (no args) → shows skill menu

## All gstack skills (also available directly)

**Think & Plan:**
- `/office-hours` — Brainstorm and reframe the problem
- `/plan-ceo-review` — CEO/founder-mode plan review
- `/plan-eng-review` — Engineering plan review
- `/plan-design-review` — Design plan review
- `/design-consultation` — Design consultation

**Build & Review:**
- `/review` — Pre-landing code review
- `/investigate` — Root cause debugging
- `/design-review` — Visual QA and design audit
- `/codex` — Second opinion from OpenAI

**Test:**
- `/qa` — QA test and fix bugs
- `/qa-only` — QA report only (no fixes)

**Ship & Reflect:**
- `/ship` — Merge, test, version, push, create PR
- `/document-release` — Update docs post-ship
- `/retro` — Weekly engineering retrospective

**Tools:**
- `/browse` — Web browsing (use this for all browsing)
- `/setup-browser-cookies` — Import browser cookies

**Safety:**
- `/careful` — Warn before destructive commands
- `/freeze` — Restrict edits to one directory
- `/guard` — Full safety mode (careful + freeze)
- `/unfreeze` — Remove edit restrictions
- `/gstack-upgrade` — Upgrade gstack

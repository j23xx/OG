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
- `/plan-devex-review` — Developer experience plan review
- `/autoplan` — Automated plan review pipeline (CEO + design + eng + DX)
- `/design-consultation` — Design consultation

**Design:**
- `/design-shotgun` — Explore multiple visual design variants
- `/design-html` — Convert mockup/design to production HTML
- `/design-review` — Visual QA and design audit

**Build & Review:**
- `/review` — Pre-landing code review
- `/investigate` — Root cause debugging
- `/cso` — Security audit (OWASP Top 10 + STRIDE threat modeling)
- `/devex-review` — Live developer experience audit
- `/health` — Code quality dashboard and score
- `/codex` — Second opinion from OpenAI

**Test:**
- `/qa` — QA test and fix bugs
- `/qa-only` — QA report only (no fixes)

**Ship & Deploy:**
- `/ship` — Merge, test, version, push, create PR
- `/land-and-deploy` — Merge PR to production with verification & auto-revert
- `/canary` — Post-deploy monitoring
- `/benchmark` — Core Web Vitals & bundle size regression detection
- `/document-release` — Update docs post-ship
- `/retro` — Weekly engineering retrospective

**Browser & Tools:**
- `/browse` — Headless browser automation (use this for all browsing)
- `/open-gstack-browser` — Headed browser with live sidebar
- `/pair-agent` — Connect a remote agent to your browser
- `/setup-browser-cookies` — Import browser cookies
- `/setup-deploy` — Platform auto-detection and deploy configuration
- `/checkpoint` — Save and resume working state
- `/learn` — Manage project learnings across sessions

**Safety:**
- `/careful` — Warn before destructive commands
- `/freeze` — Restrict edits to one directory
- `/guard` — Full safety mode (careful + freeze)
- `/unfreeze` — Remove edit restrictions
- `/gstack-upgrade` — Upgrade gstack

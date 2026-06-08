# OG

Master router for [gstack](https://github.com/garrytan/gstack) skills in Claude Code. Describe what you want in plain English — OG picks the right skill(s), runs them in the right order, and parallelizes independent skills automatically.

Named in recognition of Garry Tan's visionary leadership of YC and the startup community.

## What it does

Instead of remembering 20+ individual skill names, just type `/OG` followed by what you want:

```
/OG review and ship this          → runs /review then /ship sequentially
/OG plan review from CEO and eng  → runs /plan-ceo-review + /plan-eng-review in parallel
/OG QA the site and review code   → runs /qa + /review in parallel
/OG                               → shows the full skill menu
```

OG understands dependencies (review before ship, cookies before browse) and parallelizes independent work automatically.

## Prerequisites

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) installed and working
- [gstack](https://github.com/garrytan/gstack) v1.0+ installed in Claude Code

## Install

Open Claude Code and paste the following prompt:

```
Check if gstack skills are installed (look for gstack skills in ~/.claude/skills/).
If gstack is not installed, let me know and point me to https://github.com/garrytan/gstack

If gstack IS installed, do the following:
1. Run: git clone https://github.com/j23xx/OG.git ~/.claude/skills/OG
2. Read ~/.claude/skills/OG/OG-UPDATE.md and add its contents to my CLAUDE.md (create CLAUDE.md if it doesn't exist)
```

## Update

Open Claude Code and paste:

```
Run: cd ~/.claude/skills/OG && git pull
Then read ~/.claude/skills/OG/OG-UPDATE.md and update my CLAUDE.md to match
```

## How to use

### Quick start

Type `/OG` followed by what you want to do:

```
/OG <describe your task>
```

### Available skills

**Think & Plan**
| Command | What it does |
|---------|-------------|
| `/office-hours` | Brainstorm and reframe the problem |
| `/plan-ceo-review` | CEO/founder-mode plan review |
| `/plan-eng-review` | Engineering plan review |
| `/plan-design-review` | Design plan review |
| `/plan-devex-review` | Developer experience plan review |
| `/autoplan` | Run all plan reviews automatically (CEO + design + eng + DX) |
| `/design-consultation` | Design consultation |

**Design**
| Command | What it does |
|---------|-------------|
| `/design-shotgun` | Explore multiple visual design variants |
| `/design-html` | Convert approved mockup/design to production HTML |
| `/design-review` | Visual QA and design audit |

**Build & Review**
| Command | What it does |
|---------|-------------|
| `/review` | Pre-landing code review |
| `/investigate` | Root cause debugging |
| `/cso` | Security audit (OWASP Top 10 + STRIDE threat modeling) |
| `/devex-review` | Live developer experience audit |
| `/health` | Code quality dashboard and score |
| `/codex` | Second opinion from OpenAI |

**Test**
| Command | What it does |
|---------|-------------|
| `/qa` | QA test and fix bugs |
| `/qa-only` | QA report only (no fixes) |

**Ship & Deploy**
| Command | What it does |
|---------|-------------|
| `/ship` | Merge, test, version, push, create PR |
| `/land-and-deploy` | Merge PR to production with verification & auto-revert |
| `/canary` | Post-deploy monitoring |
| `/benchmark` | Core Web Vitals & bundle size regression detection |
| `/document-release` | Update docs post-ship |
| `/retro` | Weekly engineering retrospective |

**Browser & Tools**
| Command | What it does |
|---------|-------------|
| `/browse` | Headless browser automation |
| `/open-gstack-browser` | Headed browser with live sidebar (watch it work) |
| `/pair-agent` | Connect a remote agent to your browser |
| `/setup-browser-cookies` | Import browser cookies |
| `/setup-deploy` | Platform auto-detection and deploy configuration |
| `/checkpoint` | Save and resume working state |
| `/learn` | Manage project learnings across sessions |

**Safety**
| Command | What it does |
|---------|-------------|
| `/careful` | Warn before destructive commands |
| `/freeze` | Restrict edits to one directory |
| `/guard` | Full safety mode (careful + freeze) |
| `/unfreeze` | Remove edit restrictions |

### Examples

```bash
# Think through a problem
/OG brainstorm this feature idea

# Get all perspectives on a plan
/OG CEO, eng, and design review this plan

# Full review pipeline
/OG review the code, QA the site, then ship it

# Debug something
/OG investigate why the tests are failing

# Ship with docs
/OG ship this and update the docs

# Full deploy pipeline
/OG review, ship, deploy, and monitor
```

## License

MIT

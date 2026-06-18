# skills-map — index of AI agent skills

> Rule file for Cline (place in `.clinerules/skills-map.md` or import
> into `.clinerules`). Apply when the user asks "what skills are
> there", "show me all skills", "give me the github link for skill X",
> or when an agent needs to know which skill covers a task.


## Goal

A short map of every AI agent skill published under GitHub user
`bigdata2211it-web`. For each skill: a link to its GitHub repo and a
one-line description of what it does. Use when the user asks "what
skills are there", "show me all skills", "give me the github link for
skill X", or when an agent needs to know which skill covers a task.

Each skill is its own git repo — clone the one you need.

## Map

| Skill | GitHub repo | What it does |
|-------|-------------|--------------|
| mybd-cryfs | https://github.com/bigdata2211it-web/ai-vault-skills | Encrypted credentials vault with cryfs (FUSE): cross-platform install, migration, daily open/close, auto-lock, agent discipline, backup, password change, troubleshooting. |
| wine-exe-fix | https://github.com/bigdata2211it-web/ai-wine-skills | Diagnose and fix Windows .exe launch failures under Wine: 32/64-bit prefix, .NET runtime, missing NuGet DLLs, assembly vs package version, binding redirects, DirectX, fonts, VC++ runtimes, MSI/COM/registry fixes, `.desktop` launchers. |
| caveman | (built into opencode, not a standalone repo) | Ultra-compressed communication mode — cuts token usage ~75% by speaking like caveman while keeping full technical accuracy. Intensity levels: lite, full, ultra, wenyan-*. |

## Persistence of this skill

Active whenever the user asks for an overview of available skills or a
github link for a specific skill. Stays available across turns; no
on/off toggle needed.

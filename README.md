# ai-skills-map

Short index/map of AI agent skills published under GitHub user
`bigdata2211it-web`. For each skill: a link to its GitHub repo and a
one-line description of what it does.

## Map

| Skill | GitHub repo | What it does |
|-------|-------------|--------------|
| mybd-cryfs | https://github.com/bigdata2211it-web/ai-vault-skills | Encrypted credentials vault with cryfs (FUSE): cross-platform install, migration, daily open/close, auto-lock, agent discipline, backup, password change, troubleshooting. |
| wine-exe-fix | https://github.com/bigdata2211it-web/ai-wine-skills | Diagnose and fix Windows .exe launch failures under Wine: 32/64-bit prefix, .NET runtime, missing NuGet DLLs, assembly vs package version, binding redirects, DirectX, fonts, VC++ runtimes, MSI/COM/registry fixes, `.desktop` launchers. |

## Install this map as a skill

The map is packaged for opencode, Claude Code, Cursor, Codex CLI, and
Cline — pick your tool's wrapper from this repo:

```
skills-map/
  SKILL.md                              # skill-level entry (frontmatter + body)
  _content/skills-map.md                # agnostic body (no frontmatter)
  opencode/skills-map/SKILL.md
  claude-code/skills-map/SKILL.md
  cursor/skills-map/skills-map.mdc
  codex/skills-map/AGENTS.md
  cline/skills-map/skills-map.md
```

### opencode

```bash
cp -r opencode/skills-map ~/.config/opencode/skills/
```

### Claude Code

```bash
mkdir -p ~/.claude/skills
cp -r claude-code/skills-map ~/.claude/skills/
```

### Cursor

```bash
mkdir -p .cursor/rules
cp cursor/skills-map/skills-map.mdc .cursor/rules/
```

### Codex CLI

```bash
cat codex/skills-map/AGENTS.md >> ./AGENTS.md
```

### Cline

```bash
mkdir -p .clinerules
cp cline/skills-map/skills-map.md .clinerules/
```

## License

MIT

# skills-map — index of AI agent skills

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
| droid-byok | https://github.com/bigdata2211it-web/ai-droid-skills | Use any custom BYOK (bring-your-own-key) OpenAI-compatible model with Factory.ai's `droid` CLI without a Factory account: bypass the platform auth gate via `FACTORY_AIRGAP_ENABLED=1`, literal provider key in `~/.factory/settings.json` instead of fragile `${VAR}` substitution, persistent airgap for shells/GUI/cron/daemon, curl endpoint validation, E2E verification with a negative test, 401/402/404 BYOK troubleshooting. Provider-agnostic (OpenRouter, Ollama, LM Studio, vLLM, Azure OpenAI, Groq, Together, DeepSeek, FreeModel). |
| freemodel-cc-proxy | https://github.com/bigdata2211it-web/ai-freemodel-cc-proxy-skill | Real Claude (Opus/Sonnet/Haiku) from FreeModel `cc.freemodel.dev` for any Anthropic client (Factory Droid, Claude Code, Cline, Cursor, Pi CLI, Anthropic SDK): reverse-engineer the client-fingerprint gate (body shape, not TLS/key) via mitmproxy, build a Node proxy that injects it, wire into Droid (`provider:anthropic`+`FACTORY_AIRGAP_ENABLED=1`)/Pi (`~/.pi/agent/models.json`)/SDK, systemd autostart, web UI, troubleshooting 403/401. Companion proxy code: [ai-freemodel-cc-proxy](https://github.com/bigdata2211it-web/ai-freemodel-cc-proxy). |

## Persistence of this skill

Active whenever the user asks for an overview of available skills or a
github link for a specific skill. Stays available across turns; no
on/off toggle needed.

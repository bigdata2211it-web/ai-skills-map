---
name: skills-map
description: >
  Index/map of AI agent skills published under GitHub user
  bigdata2211it-web. For each skill: a link to its GitHub repo and a
  one-line description. Use when the user asks "what skills are there",
  "show me all skills", "give me the github link for skill X", or when
  an agent needs to know which skill covers a task.
---

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
| freemodel-cc-proxy | https://github.com/bigdata2211it-web/ai-freemodel-skills | Serve real Claude (Opus 4.8 / Sonnet 4.6 / Haiku 4.5) from FreeModel's `cc.freemodel.dev` to any Anthropic-compatible client (Factory `droid`, Claude Code, Cline, Cursor, Anthropic SDK) by impersonating the official Claude Code request fingerprint: why `api.freemodel.dev` serves only GPT while Claude is hidden on `cc.freemodel.dev` behind a "restricted to the official Claude Code client" 403 gate, the gate is a request-body fingerprint (not TLS/key), mitmproxy capture of Claude Code's `/v1/messages?beta=true` traffic, the exact required shape (`stream:true`, two leading system blocks, `metadata.user_id` JSON string, Claude Code headers), a Node proxy with web UI + systemd/LaunchAgent/Scheduled-Task autostart, 403/401/GPT-rerouting troubleshooting, re-capture after FreeModel updates. Companion proxy code: [ai-freemodel-cc-proxy](https://github.com/bigdata2211it-web/ai-freemodel-cc-proxy). |

## Persistence of this skill

Active whenever the user asks for an overview of available skills or a
github link for a specific skill. Stays available across turns; no
on/off toggle needed.

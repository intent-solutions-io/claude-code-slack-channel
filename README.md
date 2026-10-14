# Claude Code Slack Channel

<!-- intent-select-partner:start -->
<p><a href="https://intentsolutions.io/"><img src="https://raw.githubusercontent.com/intent-solutions-io/.github/b82af5d3e7951d85e39ea9e65cc24ee8278722a7/assets/brand/claude-select-partner.svg" alt="Intent Solutions: Claude Partner Network Select Services Partner" width="300" height="95" /></a></p>

Intent Solutions is a Claude Partner Network Select Services Partner.
<!-- intent-select-partner:end -->

> The **Slack-native governance substrate for Claude Code** — humans, Claude Code sessions, and peer agents converse safely in shared channels. Every tool call passes a tier-aware policy engine; every decision lands in a hash-chained, **Ed25519-signed** audit journal you can verify offline.

**Created and maintained by [Jeremy Longshore](https://github.com/jeremylongshore) / [Intent Solutions](https://intentsolutions.io).**

**Live work → [jeremylongshore/claude-code-slack-channel](https://github.com/jeremylongshore/claude-code-slack-channel)**
**Docs → [jeremylongshore.github.io/claude-code-slack-channel](https://jeremylongshore.github.io/claude-code-slack-channel/)**

[![GitHub stars](https://img.shields.io/github/stars/jeremylongshore/claude-code-slack-channel?style=social)](https://github.com/jeremylongshore/claude-code-slack-channel)
[![GitHub forks](https://img.shields.io/github/forks/jeremylongshore/claude-code-slack-channel?style=social)](https://github.com/jeremylongshore/claude-code-slack-channel/network/members)
[![License: Apache 2.0](https://img.shields.io/badge/license-Apache_2.0-blue.svg)](https://github.com/jeremylongshore/claude-code-slack-channel/blob/main/LICENSE)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/U5S225PTME)

---

## What this is

This repository is the **Intent Solutions organization landing page** for **Claude Code Slack Channel** — a Slack-native governance kernel for [Claude Code](https://code.claude.com/docs/en/), Anthropic's official CLI, and peer agents. It was the first Claude/channel implementation for Slack.

If you landed here from the Intent Solutions org: **Claude Code Slack Channel is built and maintained by Jeremy Longshore under Intent Solutions.** It ships and develops in the canonical repository:

### → [github.com/jeremylongshore/claude-code-slack-channel](https://github.com/jeremylongshore/claude-code-slack-channel)

## How it works

```
Slack workspace (cloud)
    ↕ WebSocket (Socket Mode — outbound only, no public URL)
local MCP server (spawned by Claude Code)
    ↕ stdio (MCP transport)
Claude Code session
```

Socket Mode means **no public URL needed** — it works behind a firewall, NAT, anywhere.

## Why it stands out

- **A governance substrate, not just a bridge** — the policy/journal/relay kernel is the foundation the companion **agent-governance-plane (AGP)** vendors for cross-runtime governance.
- **Tamper-evident by construction** — every decision lands in a hash-chained, Ed25519-signed audit journal you can verify offline.
- **Tier-aware policy engine** — every tool call passes a declarative, identity-aware permission gate before it runs, with operator admin commands and cross-channel approval.
- **Safe multi-party channels** — per-thread session isolation, peer-bot loop control, and defense-in-depth against prompt injection.

## Install

> **Research Preview** — requires Claude Code v2.1.80+ and a `claude.ai` login.

```bash
# AI-assisted setup walks you through the Slack app + tokens end to end:
/slack-channel:install

# After configuring tokens, run a channel:
claude --channels plugin:slack-channel@claude-code-plugins
```

Bun, Node.js, and Docker runtimes are all supported. Full Slack-app scopes, token configuration, and `doctor` / `verify` / `repair` modes are documented in the canonical repo.

## Documentation

The complete README, setup guide, roadmap, and release notes all live in the canonical repository:

**[→ Open jeremylongshore/claude-code-slack-channel](https://github.com/jeremylongshore/claude-code-slack-channel)**

---

Built and maintained by **Jeremy Longshore** · **Intent Solutions** — [intentsolutions.io](https://intentsolutions.io)

# AgentsPodium skills

Skills for agent frameworks that read `SKILL.md` (Claude Code, OpenClaw, Hermes,
Cursor and others). They teach an agent to work with [AgentsPodium](https://agentspodium.com)
hosting through its HTTP API, MCP server and A2A endpoint.

| skill | what it does |
|---|---|
| `deploy-agent` | create a pod on AgentsPodium, pay for it, get its address — over HTTP, no browser |
| `connect-agents` | link two agents over A2A: address, bearer token, card, the things that break |
| `deploy-app` | deploy a git project on a pod: frontend and backend behind one domain (beta: the builder is still being finished) |

Install:

```bash
npx skills add agentspodium/agentspodium-skills          # skills.sh
clawhub skill install deploy-agent                       # ClawHub
```

or point your framework at the raw file, e.g.
`https://raw.githubusercontent.com/agentspodium/agentspodium-skills/main/skills/deploy-agent/SKILL.md`.

Docs for agents: https://hosting.defispace.com/llms.txt · MCP: https://mcp.agentspodium.com/ ·
A2A: https://a2a.agentspodium.com/hosting/.well-known/agent-card.json

This repository is a mirror of `skills/` in the AgentsPodium codebase; edits land there first.

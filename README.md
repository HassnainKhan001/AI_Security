# AI_Security
# ai-security-ops

Central command repo for my AI security research, recon operations, and attack development. This is where all findings, techniques, and results from my AI agents get documented and organized.

**Focus areas:** LLM security, agentic AI security, prompt injection, MCP security, RAG security, AI-integrated web/mobile app security.

> My AI agents (built separately, linked in [`agents-registry.md`](#agents-registry)) perform the actual recon and attack execution. This repo is where their output is analyzed, documented, and turned into research.

---

## Repo Structure

```
ai-security-ops/
├── README.md
├── research/           # Concepts, papers, learning notes, threat models
├── recon/              # Recon results/logs gathered by my agents
├── attacks/            # Original/invented attack techniques
├── findings/           # Documented exploits — systems broken, how, impact
└── agents-registry.md  # Links to all my agent repos + what each one does
```

### `research/`
Notes, summaries, and threat models on LLM/agentic AI security concepts. Not raw exploits — the "why" behind the attacks.

### `recon/`
Output from my recon agents — what AI systems were scanned, what surface area was mapped (endpoints, tools exposed, MCP servers, model behavior fingerprinting), before any attack is attempted.

### `attacks/`
New or adapted attack techniques I've developed — not just running known payloads, but documenting novel approaches (prompt injection variants, tool-abuse chains, RAG poisoning methods, etc.)

### `findings/`
The actual results — a system was tested, here's what broke, how, and the fix. Each finding gets its own folder:
```
findings/2026-09-target-name/
├── overview.md       # what was tested, scope
├── attack-path.md     # how it was broken, step by step
├── evidence/           # logs, screenshots, PoC output
└── mitigation.md       # how to fix it
```

---

## Agents Registry

Each AI agent I build lives in its own repo (proof of dev work) and feeds results back here.

| Agent | Repo | Purpose |
|---|---|---|
| _(add as built)_ | | |

See [`agents-registry.md`](./agents-registry.md) for the full, maintained list.

---

## Status

🚧 Active — this repo grows as new agents run recon, new attacks get developed, and new systems get tested.

## Disclaimer

All research, recon, and testing documented here is conducted in controlled/authorized environments (personal labs, sanctioned CTFs, or systems I own/have explicit permission to test). No unauthorized access is performed or documented in this repo.

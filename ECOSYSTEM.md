# The FrankX Ecosystem Map

> One architecture, many surfaces. This is the canonical map of how the projects across [frankxai](https://github.com/frankxai), [Arcanea-Labs](https://github.com/Arcanea-Labs), and [oci-ai-architects](https://github.com/oci-ai-architects) fit together.
>
> **Last updated:** 2026-06-23

---

## The Spine

Everything is built on one three-layer spine. New products are **consumers** of this spine, never replacements for it.

```
            ┌─────────────────────────────────────────────┐
  PRODUCTS  │  Arcanea · AnimeLegends · GenCreator · ...   │  ← surfaces creators touch
            └─────────────────────────────────────────────┘
                                │ consume
            ┌─────────────────────────────────────────────┐
  OPERATE   │  ACOS  — skills, agents, commands, plugins   │  ← the execution runtime
            └─────────────────────────────────────────────┘
                                │ dispatched by
            ┌─────────────────────────────────────────────┐
  CONTROL      │  Hermes — profile specs + verified PR flow  │  ← private control plane, public notes
            └─────────────────────────────────────────────┘
                                │ reads / writes
            ┌─────────────────────────────────────────────┐
  REMEMBER  │  SIS  — sovereign memory + governance (SIP)  │  ← the substrate
            └─────────────────────────────────────────────┘
```

| Layer | Project | Role |
|-------|---------|------|
| Control | Hermes *(private)* · [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) | Profile specs, branch isolation, verification gates, PR discipline, and public operator notes for Hermes Agent workflows. |
| Remember | [Starlight-Intelligence-System](https://github.com/frankxai/Starlight-Intelligence-System) | The memory + governance substrate. Defines **SIP** (the open conformance protocol everything else declares against). |
| Operate | [agentic-creator-os](https://github.com/frankxai/agentic-creator-os) | 90+ skills, 38 agents, 8 plugins. The runtime creators and agents actually execute. |
| Standard | [agentic-operating-system-standard](https://github.com/frankxai/agentic-operating-system-standard) | The public spec: modules, agents, skills, workflows, loops, ledgers, gates. |

---

## Domains

### 🎨 Creative Platforms
The surfaces where creators build.

| Repo | What it is |
|------|------------|
| [arcanea](https://github.com/frankxai/arcanea) | The creative intelligence platform — chat, lore, academy, worldbuilding. |
| [arcanea-studio](https://github.com/frankxai/arcanea-studio) | Multi-model generative surface — 200+ image/video/cinema models, provider-agnostic router. |
| [arcanea-claw](https://github.com/frankxai/arcanea-claw) | Creator Media Engine — scans, classifies, scores, publishes media 24/7. |
| [AnimeLegends-Skills](https://github.com/frankxai/AnimeLegends-Skills) | Generative-native anime studio — the 7+1 stage pipeline as installable skills. |
| [author-os](https://github.com/frankxai/author-os) | AI-native author OS — multi-agent orchestration, semantic memory, publishing pipeline. |
| [arcanea-publishing-house](https://github.com/frankxai/arcanea-publishing-house) | Modern publishing house powered by agent swarms — books, marketing, social. |
| [visual-intelligence](https://github.com/frankxai/visual-intelligence) | Agentic visual asset management — auto-tag, audit, quality enforcement. |

### 🧠 Intelligence Systems
SIP-conformant domain substrates. Each composes SIS for memory and ACOS for skills. Convention: `<domain>-intelligence-system` (substrate) + `<domain>-agent-skills` (skills) + `<domain>-mcp` (server).

| Domain | Repo |
|--------|------|
| Health | [health-intelligence-system](https://github.com/frankxai/health-intelligence-system) |
| Library / books | [library-os](https://github.com/frankxai/library-os) |
| Ocean | [blue-life-commons](https://github.com/frankxai/blue-life-commons) · [marine-mcp](https://github.com/frankxai/marine-mcp) |
| Research | [research-intelligence-os](https://github.com/frankxai/research-intelligence-os) |
| Mind / cognition | [agentic-mind-os](https://github.com/frankxai/agentic-mind-os) |
| Music | [agentic-music-os](https://github.com/frankxai/agentic-music-os) · [vibe-os](https://github.com/frankxai/vibe-os) |
| Creator | [creator-intelligence-system](https://github.com/frankxai/creator-intelligence-system) |
| Investor | [investor-intelligence-systems](https://github.com/frankxai/investor-intelligence-systems) |

*…and the family extends to family, dream, neuroscience, psychology, payment, and reality domains.*

### ⚙️ Open Standards & Adoption
How others fork in.

- [agentic-operating-system-standard](https://github.com/frankxai/agentic-operating-system-standard) — the SIP spec
- [starlight](https://github.com/frankxai/starlight) — minimal SIP adoption kit, fork in 60 seconds
- [starlight-evals](https://github.com/frankxai/starlight-evals) — whole-system evaluation, receipts, named weaknesses
- [starlight-memory](https://github.com/frankxai/starlight-memory) — sovereign memory provider contract
- [starlight-horizon-dataset](https://github.com/frankxai/starlight-horizon-dataset) — append-only ledger of aligned intentions (CC-BY-SA)

### 🛠️ Developer Tools
Standalone tools, npx-installable, that feed the ecosystem.

- [mcp-doctor](https://github.com/frankxai/mcp-doctor) — diagnose & optimize MCP servers
- [storage-intelligence](https://github.com/frankxai/storage-intelligence) — disk cleanup with a 3-lens safety council
- [peak-performance](https://github.com/frankxai/peak-performance) — machine health auditor, Ten Gate scoring
- [claude-code-hooks](https://github.com/frankxai/claude-code-hooks) — production hook system, 15 battle-tested hooks
- [prompt-engine](https://github.com/frankxai/prompt-engine) — 13-agent prompt-engineering team
- [arcanea-mcp-starter](https://github.com/frankxai/arcanea-mcp-starter) — fork-to-build MCP server starter

### 📚 Knowledge & Method
- [prompt-library](https://github.com/frankxai/prompt-library) — curated, attributed, red-teamed elite prompts
- [ai-architect-academy](https://github.com/frankxai/ai-architect-academy) — become an AI architect who builds CoEs
- [context-engineering-for-creators](https://github.com/frankxai/context-engineering-for-creators) — context engineering patterns
- [kura](https://github.com/frankxai/kura) — capture creative intelligence across every AI

### 🎨 Templates
MIT-licensed, cosmic-design, AI-first starters: [arcanea-chat-template](https://github.com/frankxai/arcanea-chat-template) · [arcanea-dashboard-template](https://github.com/frankxai/arcanea-dashboard-template) · [cosmic-landing-template](https://github.com/frankxai/cosmic-landing-template) · [agentic-income-template](https://github.com/frankxai/agentic-income-template) — all indexed in [arcanea-templates](https://github.com/frankxai/arcanea-templates).

### ☁️ Enterprise (Oracle)
Day-job lineage, kept cleanly isolated in [oci-ai-architects](https://github.com/oci-ai-architects): OCI GenAI guides, AI CoE starter kits, and cross-runtime skill packs (Claude / Cline / Codex).

---

## Coding Agent Overlays
The same Arcanea intelligence (Guardians, Elements, Gates) projected onto every runtime:

| Runtime | Overlay |
|---------|---------|
| Claude Code | [claude-arcanea](https://github.com/frankxai/claude-arcanea) |
| VS Code | [arcanea-vscode](https://github.com/frankxai/arcanea-vscode) |
| OpenCode | [oh-my-arcanea](https://github.com/frankxai/oh-my-arcanea) |
| Codex | [codex-arcanea](https://github.com/frankxai/codex-arcanea) |
| Gemini CLI | [gemini-arcanea](https://github.com/frankxai/gemini-arcanea) |

---

## Conventions

- **SIP conformance** — every Intelligence System and OS declares conformance to [agentic-operating-system-standard](https://github.com/frankxai/agentic-operating-system-standard).
- **Naming** — `<domain>-intelligence-system` = substrate · `<domain>-agent-skills` = skills · `<domain>-mcp` = server · `awesome-<domain>-agent-skills` = curated index.
- **Memory** — products persist through SIS; nothing invents its own memory layer.
- **Governance** — repo mutations should follow the Hermes control-plane pattern: intent → branch → verify → PR → trace.

---

<sub>Maintained by <a href="https://github.com/frankxai">@frankxai</a> · <a href="https://frankx.ai">frankx.ai</a></sub>

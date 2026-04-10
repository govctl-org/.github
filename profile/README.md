# govctl-org

**Deterministic tooling for AI-assisted software delivery.**

We build tools that make agent work:

- **governed** — specs, decisions, and execution live in reviewable artifacts
- **traceable** — changes can be linked back to why they happened
- **phase-aware** — implementation, verification, and stability are explicit
- **local-first** — the CLI and repo remain the control plane

## Projects

### [govctl](https://github.com/govctl-org/govctl) — Governance Harness for AI Coding

`govctl` is a governance-as-code CLI for teams using AI to build software seriously.

It gives AI-assisted development a control plane in the repository:

- **RFCs** say what must be true
- **ADRs** record why a design was chosen
- **Work items** track execution and acceptance criteria
- **Verification guards** enforce executable completion gates

Typical flow:

```bash
govctl init
govctl status
govctl rfc new "Caching Strategy"
govctl adr new "Choose cache backend"
govctl work new --active "implement caching"
```

Highlights:

- spec-first, phase-gated workflow
- stable CLI contract for humans and agents
- brownfield adoption through the `/migrate` workflow for agent-guided governance onboarding
- governed artifact operations through `list`, `show`, `get`, `edit`, and lifecycle verbs

### [skillc](https://github.com/govctl-org/skillc) — Development Kit for Agent Skills

`skillc` helps skill authors and power users scaffold, validate, compile, search, and analyze [Agent Skills](https://agentskills.io/).

Typical flow:

```bash
skc init my-skill
skc lint my-skill
skc build my-skill
skc stats my-skill
```

Highlights:

- local authoring and validation
- searchable compiled skill content
- usage analytics and sync
- MCP integration for read-side agent workflows

## Incubating

These are active directions we are exploring, not yet stable public products:

- **jjgov** — multi-agent collaboration workflows around Jujutsu
- **everevolve** — project rules inferred and refined from commit history

## Philosophy

We believe AI coding gets more useful when it is:

- **structured enough to review**
- **explicit enough to automate**
- **disciplined enough to scale**

The goal is not more ceremony. The goal is to turn fast generation into reliable delivery.

## Links

| Resource | URL |
| --- | --- |
| Website | [govctl.org](https://govctl.org) |
| Blog | [govctl.org/blog](https://govctl.org/blog) |
| govctl Docs | [govctl-org.github.io/govctl](https://govctl-org.github.io/govctl/) |
| skillc Docs | [govctl-org.github.io/skillc](https://govctl-org.github.io/skillc/) |
| Discord | [discord.gg/buBB9G8Z6n](https://discord.gg/buBB9G8Z6n) |

<p align="center">
  <sub>Built with phase discipline. Governed by govctl.</sub>
</p>

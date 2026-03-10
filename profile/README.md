# Cohvu

Persistent, shared knowledge for AI agents.

Cohvu gives your AI agents a shared knowledge graph that persists across sessions and agents. Agents read, contribute, challenge, and refine knowledge automatically — no dashboards, no manual entry. The agent is the interface.

## Setup

Add to your agent's MCP config:

```json
{
  "mcpServers": {
    "cohvu": {
      "command": "npx",
      "args": ["cohvu"]
    }
  }
}
```

On first connection, a browser window opens for Google sign-in. After that, it's automatic.

Then ask your agent:

> Create a root scope called "My Team"

It returns a Stripe checkout link. Complete payment ($9/seat/month), and your scope is live. Your agent starts contributing immediately.

## How it works

**Your agent is the interface.** There's no dashboard. You talk to your agent, and it manages everything through Cohvu's MCP tools.

- **Canon** — The team's source of truth. Agents establish, update, challenge, and refine it over time. Truth converges naturally.
- **Records** — Observations and decisions captured as they happen. Immutable, linked by causality.
- **Tensions** — Contradictions between beliefs. Agents flag them, future sessions resolve them.
- **Divergences** — Gaps between what's documented and what's real. Agents report them when they notice.
- **Mesh** — A relationship graph connecting all knowledge. Agents wire it together so future sessions can reason across it.
- **Scopes** — Organize knowledge into a tree. Modules, features, domains — whatever fits.

## Invite people

Ask your agent:

> What's my people link?

Share the link. They sign in with Google and join your scope. Their agents see the same knowledge. $9/seat/month, added automatically.

## Autonomous agents

For agents that can't open a browser (CI pipelines, background workers, cron jobs):

> What's my agent link?

Configure the agent with the link as its MCP server URL. No auth needed. Agents don't count as seats.

## Pricing

$9/seat/month. No free tier. No tiers at all. Every seat gets everything. Cancel anytime.

## Why

AI agents accumulate context every session — then lose it. Cohvu is where that context lives permanently. Agents build on each other's work instead of starting from scratch. The knowledge graph converges toward accuracy because every agent can challenge, support, and refine what came before.

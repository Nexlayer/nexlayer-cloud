<p align="center">
  <a href="https://nexlayer.com">
    <img src="assets/hero.png" alt="Nexlayer - Ship it. The new way to ship software. Autonomously." width="100%">
  </a>
</p>

<p align="center">
  <strong>The agentic cloud platform that deploys your code.</strong>
</p>

<p align="center">
  <a href="https://nexlayer.com/docs">Documentation</a> •
  <a href="https://nexlayer.com/resources/templates">Templates</a> •
  <a href="https://nexlayer.com/resources/use-cases">Use Cases</a> •
  <a href="https://nexlayer.com/resources/changelog">Changelog</a> •
  <a href="https://join.slack.com/t/nexlayercommunity/shared_invite/zt-3ns0038s0-16GWdSAD1aPdyxDzmbGaiw">Community</a>
</p>

---

## What is Nexlayer?

**Nexlayer is an agentic cloud platform where AI agents deploy, scale, and manage your applications autonomously—you describe what you want, and the platform handles the rest.**

No Kubernetes expertise. No YAML sprawl. No 3 AM pages. Just ship it.

---

## How It Works

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                           AGENTIC CLOUD ARCHITECTURE                        │
└─────────────────────────────────────────────────────────────────────────────┘

     YOU                          NEXLAYER                         CLOUD
      │                              │                               │
      │  "Deploy my app"             │                               │
      │  ─────────────────────────►  │                               │
      │                              │                               │
      │                    ┌─────────▼─────────┐                     │
      │                    │  NEXLAYER AGENT   │                     │
      │                    │  ┌─────────────┐  │                     │
      │                    │  │ Analyze     │  │                     │
      │                    │  │ Configure   │  │                     │
      │                    │  │ Provision   │  │                     │
      │                    │  │ Deploy      │  │                     │
      │                    │  │ Monitor     │  │                     │
      │                    │  └─────────────┘  │                     │
      │                    └─────────┬─────────┘                     │
      │                              │                               │
      │                              │  Autonomous orchestration     │
      │                              │  ─────────────────────────►   │
      │                              │                               │
      │                              │         ┌─────────────────────▼───┐
      │                              │         │  YOUR APP RUNNING       │
      │                              │         │  • Auto-scaled          │
      │                              │         │  • Auto-healed          │
      │                              │         │  • Cost-optimized       │
      │  Live URL + dashboard        │         └─────────────────────────┘
      │  ◄─────────────────────────  │                               │
      │                              │                               │
```

### The Agentic Difference

Traditional cloud: You write infrastructure code → You debug infrastructure code → You maintain infrastructure code forever.

**Agentic cloud:** You describe intent → Agents handle infrastructure → You focus on your product.

| Traditional DevOps | Nexlayer |
|-------------------|----------|
| Write Dockerfiles, Kubernetes manifests, Terraform | Describe your app in plain English or simple YAML |
| Debug networking, DNS, certificates, ingress | Agents configure networking automatically |
| Monitor dashboards, set up alerts, respond to pages | Agents detect and fix issues before you notice |
| Estimate capacity, over-provision "just in case" | Agents scale precisely to demand |

---

## What's Under the Hood

Your agent talks to Nexlayer. Three specialized agents do the rest.

```mermaid
flowchart TB
    subgraph coding["🤖 YOUR AI CODING AGENT"]
        tools["Claude Code · Cursor · Windsurf · VS Code · Claude Desktop · Antigravity"]
    end

    coding -->|"Nexlayer Agent Connector"| protocol

    subgraph protocol["⚡ NEXLAYER AGENT CONNECTOR"]
        desc["One connection. Deploys, debugs, and manages production — no config, no human in the loop."]
    end

    protocol --> deploy
    protocol --> debug
    protocol --> ops

    subgraph deploy["🚀 DEPLOY AGENT"]
        d1["<b>Ships it</b><br/>Any stack · Any language<br/>Containers auto-built<br/>Live URL in minutes"]
    end

    subgraph debug["🔍 DEBUG AGENT"]
        db1["<b>Sees inside it</b><br/>Live shell access<br/>Real-time logs · DB queries<br/>File inspection"]
    end

    subgraph ops["🛡️ OPS AGENT"]
        o1["<b>Keeps it running</b><br/>Auto-scales · Self-heals<br/>Monitors 24/7<br/>Zero downtime deploys"]
    end

    deploy --> cloud
    debug --> cloud
    ops --> cloud

    subgraph cloud["☁️ NEXLAYER PRODUCTION CLOUD"]
        features["no cold starts · load balancing · SSL everywhere<br/>isolated namespaces · custom domains · persistent storage<br/>RBAC security · spend limits"]
    end
```


---

## Three Anxieties We Eliminate

### 1. Deployment Anxiety
*"What if I break production?"*

Every deployment gets its own isolated environment with a unique URL. Test it, share it, verify it—then promote to production when ready. Rollback is one click. Agents validate health before routing traffic.

### 2. Scaling Anxiety
*"What if we get featured on Hacker News?"*

Agents monitor traffic patterns and scale automatically. No capacity planning. No manual intervention. Your app handles the spike while you enjoy the moment.

### 3. Bill Shock
*"What if I wake up to a $50,000 bill?"*

**We built explicit protection into the platform:**

| Status | What It Means |
|--------|---------------|
| 🟢 **Green** | Running normally, within your credit ceiling |
| 🟡 **Amber** | Approaching limit—we email you with options |
| 🔴 **Red** | Credit ceiling reached—**apps are paused, not deleted** |

**The guarantee:** Nothing is lost without your permission. Your apps pause gracefully. Your data stays intact. You decide what happens next—add credits, optimize, or wind down. No surprise charges. No panic. No lost work.

---

## Quick Start

Connect Nexlayer to your AI coding assistant:

```bash
npx @nexlayer/mcp-install
```

Then just tell your assistant: *"Deploy this to Nexlayer"*

That's it. One command. Your agent handles the rest.

**[Quickstart guide →](https://nexlayer.com/docs/quickstart)**

---

## What's Running on Nexlayer Right Now

Real apps. Real production traffic. Real developers shipping every day.

```
┌────────────────────────────────────────────────────────────────┐
│  STACK DIVERSITY (from live deployments)                       │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│  Node.js    ████████████████████████░░░░░░░░  42%             │
│  Python     ██████████████░░░░░░░░░░░░░░░░░░  28%             │
│  Go         ██████░░░░░░░░░░░░░░░░░░░░░░░░░░  12%             │
│  Rust       ████░░░░░░░░░░░░░░░░░░░░░░░░░░░░   8%             │
│  Java       ███░░░░░░░░░░░░░░░░░░░░░░░░░░░░░   5%             │
│  Other      ██░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░   5%             │
│             (C#, PHP, Ruby, Elixir)                           │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

**Supported stacks:** Node.js • Python • Go • Rust • Java Spring • C# ASP.NET • PHP Laravel • Ruby • Elixir • Any Docker container

---

## Use Cases

| What You're Building | How Nexlayer Helps |
|---------------------|-------------------|
| **AI/ML Apps** | You built something with an LLM. You need it running 24/7. Done. |
| **SaaS Products** | Every customer gets their own environment. You don't manage any of them. |
| **Internal Tools** | Deploy on every PR. Tear it down when merged. Fully automatic. |
| **Startups** | Start free. Scale to millions. Never re-platform. |
| **Agencies** | Spin up client environments in seconds. Bill per-project. |

**[Explore all use cases →](https://nexlayer.com/resources/use-cases)**

---

## Resources

| Resource | Description |
|----------|-------------|
| [**Quickstart**](https://nexlayer.com/docs/quickstart) | Get deployed in under 5 minutes |
| [**MCP Setup**](https://nexlayer.com/docs/mcp/overview) | Connect your AI coding assistant |
| [**Claude Code Setup**](https://nexlayer.com/docs/mcp/claude-code) | Setup guide for Claude Code |
| [**Cursor Setup**](https://nexlayer.com/docs/mcp/cursor) | Setup guide for Cursor |
| [**Configuration**](https://nexlayer.com/docs/deployments/configuration) | nexlayer.yaml reference |
| [**Custom Domains**](https://nexlayer.com/docs/deployments/custom-domains) | Use your own domain |
| [**For AI Agents**](https://nexlayer.com/docs/agents/overview) | Build agents that deploy |
| [**Templates**](https://nexlayer.com/resources/templates) | Pre-built stacks: Next.js, FastAPI, Rails, and more |
| [**Changelog**](https://nexlayer.com/resources/changelog) | What's new and what's next |
| [**Community Slack**](https://join.slack.com/t/nexlayercommunity/shared_invite/zt-3ns0038s0-16GWdSAD1aPdyxDzmbGaiw) | Get help, share feedback, connect with the team |

---

## FAQ

<details>
<summary><strong>Is Nexlayer open source?</strong></summary>

No. Nexlayer is a managed platform. This repository contains documentation, examples, and community resources—not the platform source code.
</details>

<details>
<summary><strong>What happens to my data if I stop paying?</strong></summary>

Apps pause. Data persists. We email you. You have 30 days to export or resume. Nothing is deleted without explicit confirmation from you.
</details>

<details>
<summary><strong>Can I use my own Kubernetes cluster?</strong></summary>

Currently, Nexlayer runs on our managed infrastructure. Bring-your-own-cloud options are on the roadmap.
</details>

<details>
<summary><strong>How is this different from Vercel/Railway/Render?</strong></summary>

Those platforms require you to configure deployments. Nexlayer agents figure out the configuration. You describe intent; agents handle implementation. It's the difference between writing infrastructure and describing outcomes.
</details>

<details>
<summary><strong>Does Nexlayer use MCP?</strong></summary>

Yes. The Nexlayer Agent Protocol is built on [Model Context Protocol (MCP)](https://www.anthropic.com/news/model-context-protocol), the open standard created by Anthropic. We've extended it with Nexlayer's embedded agent layer — so your coding tool stays compatible, and Nexlayer handles the rest.
</details>

---

<p align="center">
  <a href="https://nexlayer.com">
    <img src="https://img.shields.io/badge/Start_Shipping-nexlayer.com-black?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9IiNmZmYiIHN0cm9rZS13aWR0aD0iMiI+PHBhdGggZD0iTTEyIDJMMiA3bDEwIDUgMTAtNS0xMC01eiIvPjxwYXRoIGQ9Ik0yIDE3bDEwIDUgMTAtNSIvPjxwYXRoIGQ9Ik0yIDEybDEwIDUgMTAtNSIvPjwvc3ZnPg==" alt="Start Shipping">
  </a>
</p>

<p align="center">
  <sub>Built for developers who'd rather ship products than manage infrastructure.</sub>
</p>

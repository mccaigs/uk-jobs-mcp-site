# uk-jobs-mcp · Landing Page

The marketing and documentation site for [uk-jobs-mcp](https://github.com/mccaigs/uk-jobs-mcp) — the standard MCP interface for UK recruitment data.

Built as a single-file static site, deployed on Vercel.

---

## What this is

A clean, developer-focused landing page that explains what `uk-jobs-mcp` is, why it was built, and how to get started. Designed to give the project a credible web presence beyond the GitHub README, and to rank for searches like "UK recruitment MCP" as the ecosystem grows.

---

## Stack

- Plain HTML, CSS, and vanilla JS — no framework, no build step
- [DM Mono](https://fonts.google.com/specimen/DM+Mono) + [DM Sans](https://fonts.google.com/specimen/DM+Sans) via Google Fonts
- Deployed on [Vercel](https://vercel.com) — zero config

---

## Structure

```
uk-jobs-mcp-site/
├── index.html    — the entire site, single file
└── vercel.json   — Vercel rewrite config
```

No `node_modules`. No build process. No dependencies. Just push and it's live.

---

## Running locally

Open `index.html` directly in a browser, or serve it with any static server:

```bash
npx serve .
```

---

## Deploying to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project
3. Import the repo
4. Deploy — no configuration needed

Vercel detects the static site automatically. The `vercel.json` handles the single-page rewrite.

### Custom domain

Once deployed, add your domain in Vercel's project settings under **Domains**. The site is designed to sit at a root domain like `ukjobsmcp.dev` or a subdomain like `mcp.careersai.co.uk` when CareersAI launches.

---

## Sections

| Section | Purpose |
|---|---|
| Hero | Project name, one-line description, GitHub CTA |
| Why I built this | The origin story — the frustration of re-keying profiles on every job platform |
| Tools | All eight MCP tools across three auth tiers |
| Quick start | Four-step guide from clone to connected |
| Implement the standard | Instructions for other platforms to adopt the schema |
| Footer | Links to GitHub, MCP docs, LinkedIn |

---

## Updating content

Everything lives in `index.html`. Key areas to update as the project evolves:

- **Hero badge** — change from "Open standard · MIT licence" to include a hosted URL when the server is live
- **Quick start step 2** — replace `localhost` with the hosted endpoint URL when available
- **"Coming soon" copy** — remove once the hosted instance is deployed
- **Built with section** — add entries as other platforms adopt the standard

---

## Related

- [uk-jobs-mcp](https://github.com/mccaigs/uk-jobs-mcp) — the MCP server itself
- [Model Context Protocol](https://modelcontextprotocol.io) — the spec this is built on
- [David Robertson](https://www.linkedin.com/in/daverobertson4/) — built by

---

## Licence

MIT

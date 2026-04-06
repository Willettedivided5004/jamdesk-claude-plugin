# Jamdesk Claude Code Plugin

A Claude Code plugin for building [Jamdesk](https://www.jamdesk.com) documentation sites. Gives Claude deep knowledge of Jamdesk components, configuration, navigation patterns, and CLI commands — so you can build docs faster with AI assistance.

## Quick Start

Get started with Jamdesk + Claude Code:

```bash
# Install Jamdesk CLI
npm install -g jamdesk

# Create a docs project
jamdesk init my-docs && cd my-docs

# Start local dev server
jamdesk dev
```

Then invoke the plugin skill:

```
/jamdesk:jamdesk
```

## What's Included

One skill (`/jamdesk:jamdesk`) with a quick-reference hub and three detailed reference files:

| Reference | Contents |
|-----------|----------|
| **Components** | 25+ MDX components — Cards, Steps, Tabs, Callouts, Code Groups, Tables, and more — with complete props and examples |
| **Configuration** | Full `docs.json` schema — themes, colors, branding, navbar, footer, API config, 20+ analytics integrations |
| **Navigation** | 8 navigation patterns — flat, grouped, tabbed, multi-product, versioned, multi-language, dropdowns, OpenAPI |

Plus: CLI command reference (20 commands), page frontmatter fields, image sizing syntax, writing standards, and common mistakes.

## Installation

### From Claude Code Marketplace

```bash
# Step 1: Add the marketplace
/plugin marketplace add jamdesk/jamdesk-claude-plugin

# Step 2: Install the plugin
/plugin install jamdesk@jamdesk-marketplace
```

### Manual (for development/testing)

```bash
git clone https://github.com/jamdesk/jamdesk-claude-plugin.git
claude --plugin-dir ./jamdesk-claude-plugin
```

## Usage

Invoke the skill manually when working on Jamdesk documentation:

```
/jamdesk:jamdesk
```

Claude may also automatically suggest this skill when it detects a `docs.json` file in your project.

Claude reads only the sections relevant to your task — the hub provides quick answers, and reference files load on demand for deep dives.

## What is Jamdesk?

[Jamdesk](https://www.jamdesk.com) is a documentation platform for building beautiful, fast documentation sites from MDX files.

- **Three themes** — Jam, Nebula, Pulsar (all with dark mode)
- **25+ MDX components** — Cards, Steps, Tabs, Code Groups, Tables, API fields, color palettes, and more
- **OpenAPI & AsyncAPI** — Auto-generated API reference with interactive playground
- **AI Chat** — Built-in AI assistant trained on your docs content
- **Global CDN** — Fast deploys to Cloudflare R2 + Vercel Edge
- **CLI tooling** — Local dev server, validation, spellcheck, broken link detection
- **Migrate from Mintlify** — Run `jamdesk migrate` to convert `mint.json` → `docs.json` and update component syntax
- **Custom domains** — Host at `docs.yoursite.com` or `yoursite.com/docs`
- **Analytics** — Built-in dashboard + 20+ integrations (GA4, Plausible, PostHog, Amplitude, etc.)
- **Search** — Full-text search with keyboard navigation, out of the box

Learn more at [jamdesk.com](https://www.jamdesk.com) or read the [documentation](https://www.jamdesk.com/docs).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to keep the reference files up to date as Jamdesk evolves.

## License

Apache 2.0 — see [LICENSE](LICENSE).

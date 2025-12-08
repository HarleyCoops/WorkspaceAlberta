# WorkspaceAlberta

Shareable Cursor workspace templates for specific user cohorts with MCP configurations and secure key management.

## Overview

WorkspaceAlberta enables you to create and share customized Cursor IDE workspaces for specific audiences (cohorts) like small business owners, developers, or teams. When someone clones this repo, they get:

- Pre-configured MCP server connections
- Custom Cursor rules and settings
- Cohort-specific layouts and themes
- Secure key management (no exposed API keys)

## Quick Start

1. Clone this repository
2. Copy `.env.example` to `.env`
3. Add your API keys to `.env`
4. Open in Cursor - workspace settings apply automatically

## Project Structure

```
WorkspaceAlberta/
├── .cursor/
│   └── rules/
│       └── small-business.mdc     # Cohort-specific rules
├── .env.example                    # Template for required keys
├── mcp-config.template.json        # MCP config with ${VAR} placeholders
├── setup.ps1 / setup.sh           # One-click setup script
├── README.md                       # This file
└── docs/
    └── getting-started.md
```

## Cohorts

### Small Business Owners (Initial Focus)
- Simplified MCP connections (calendar, email, basic automation)
- Clean, non-technical layout
- Pre-configured tools for common business tasks

## Key Management

API keys are never committed to the repository. Instead:

1. Keys are stored in local `.env` file (git-ignored)
2. MCP configs reference environment variables
3. `.env.example` documents required keys without values

## Status

[Active Development] - See [project tracking](https://github.com/HarleyCoops/Daily) for task T-2025-12-001

## License

MIT

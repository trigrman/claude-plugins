# Claude Plugins Marketplace

Mike's personal Claude Code plugin marketplace.

## Repository Purpose

This repo is an **index only** - it contains `marketplace.json` which points to plugins hosted in separate repositories. Plugin source code does not live here.

## Adding a New Plugin

1. Create the plugin in its own repo (e.g., `trigrman/new-plugin`)
2. Ensure it has `.claude-plugin/plugin.json`
3. Push to GitHub
4. Add entry to `.claude-plugin/marketplace.json`:
   ```json
   {
     "name": "new-plugin",
     "source": "github:trigrman/new-plugin",
     "description": "What it does"
   }
   ```
5. Commit and push this repo
6. Update the README.md plugin table

## Current Plugins

| Plugin | Repo | Description |
|--------|------|-------------|
| granola-meetings | [trigrman/granola-meetings](https://github.com/trigrman/granola-meetings) | Access and review Granola meeting notes |

## Reference

For marketplace format and plugin development guidelines, see:
`~/dev/llm-context/claude-code-infrastructure.md`

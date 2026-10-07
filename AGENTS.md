# About this project

- This is the public documentation for Agent Market, a marketplace where buyers hire AI agents by the job, with escrow, over the web app, MCP, or A2A.
- The product code lives in a separate repository, `agents-market-v2`. This repo holds only docs.

# Mintlify

- The site is built on [Mintlify](https://mintlify.com). Pages are MDX files with YAML frontmatter. Site configuration lives in `docs.json`.
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP.
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, for Mintlify mechanics: frontmatter, components, `docs.json` navigation, `mint validate`.
- The Mintlify skill is not installed here. `npx skills add https://mintlify.com/docs` installs it if needed.

## 🚨 CRITICAL RULES (NEVER VIOLATE)

1. **Invoke the `writing-plain-english` skill (`.claude/skills/writing-plain-english/SKILL.md`) before you write or edit any page.** It holds the voice, sentence, heading, and word rules, the product terms table, and the self-check.
2. **Files under `https://market.near.ai/skill/` are skills for agents.** Link them only as a skill the reader gives to their agent, never as reading for the person.

# Content boundaries

-

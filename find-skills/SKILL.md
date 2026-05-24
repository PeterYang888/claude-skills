---
name: find-skills
description: "Search, browse, and install Claude Code skills from the skills.sh registry. Use when the user wants to find a skill, discover plugins, or install a skill package."
---

# Find & Install Claude Code Skills

Help the user search for and install skills from the [skills.sh](https://skills.sh) registry using the `npx skills` CLI.

## Workflow

### Step 1: Determine search keywords

Ask the user what kind of skill they're looking for if they haven't already specified. Extract clear, concise keywords from their request.

**Examples of keyword extraction:**
- "I want to analyze Excel files" → `excel analyze`
- "Help me manage GitHub PRs" → `github pr`
- "I need something for Slack notifications" → `slack notify`

### Step 2: Search for skills

Run the search command:

```bash
npx skills find "<keywords>"
```

### Step 3: Present results

Display the results in a clear table format:

| Skill | Installs | Description |
|-------|----------|-------------|
| `owner/repo@skill-name` | count | Brief description if available |

Sort by install count (most popular first). Highlight the top recommendation.

### Step 4: Offer to install

Ask the user if they'd like to install any of the results. If yes, run:

```bash
npx skills add <owner/repo@skill-name>
```

After installation, confirm success and let the user know they can use the skill via its slash command (e.g., `/skill-name`).

### Step 5: Other useful commands

If the user needs more options, these commands are also available:

| Command | Description |
|---------|-------------|
| `npx skills find "<query>"` | Search for skills by keyword |
| `npx skills add <owner/repo@skill>` | Install a skill |
| `npx skills remove <skill>` | Uninstall a skill |
| `npx skills list` | List currently installed skills |
| `npx skills update` | Update all installed skills |

## Notes

- Always run searches with `npx skills find` so results are up-to-date from the registry.
- If no results are found, suggest the user try broader or alternative keywords.
- If the user wants to browse without a specific query, suggest popular categories: `excel`, `github`, `slack`, `docker`, `aws`, `database`, `api`, `testing`, `ai`, `pdf`.

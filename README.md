# Test Case Skill Library 🧪

AI prompt template for fully automated test case generation using Claude + Jira + Xray.

## How It Works
1. You type: "Write test cases for PROJ-456" in Claude
2. Claude reads the Jira ticket automatically (via Atlassian MCP)
3. Claude fetches this prompt template directly from this repo (always the latest version)
4. Claude generates structured test cases following the rules in the prompt
5. After your approval, Claude pushes them to Xray automatically

## Single Prompt File
One intelligent prompt handles all ticket types — user stories, bugs, and API integration tickets. Claude reads the ticket, figures out the format, and adapts automatically.

| File | Purpose |
|------|---------|
| `prompts/system-prompt.md` | Complete test case generation rules, quality standards, output format, and coverage checklist |

## Editing the Prompt
1. Edit `prompts/system-prompt.md` in this repo
2. Commit to main branch
3. Done — Claude automatically uses the updated version next time

No re-uploading, no syncing. GitHub is the single source of truth.

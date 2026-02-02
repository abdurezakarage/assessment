# Tenx MCP Assessment Notes

## What I did
- Created `/.github/copilot-instructions.md` for VS Code Copilot agent rules.
- Added sections for priorities, workflow, code style, testing, MCP usage, and communication.
- Captured repository-specific preferences (Tailwind CSS, `models/` for ML artifacts).
- Documented setup guidance for Tenx MCP in VS Code.

## What worked
- A clear priority order reduced ambiguity in agent responses.
- Small, scoped diffs plus explicit testing guidance improved predictability.
- Explicit MCP usage guidance makes tool selection easier for the agent.
## What didn’t work
- Overly strict rules occasionally slowed down responses
- Some rules were applied inconsistently depending on the model
## Troubleshooting and approach
- Used official MCP documentation for VS Code and Tenx as primary references.
- Focused on rules that are broadly recommended by the community:
  clear priorities, minimal diffs, explicit tests, and concise communication.

## Insights gained
- Rules that define priorities and workflow reduce unnecessary changes.
- Explicit testing guidance makes outputs more reliable and auditable.
- Tooling rules (MCP usage) shape how the agent gathers context.
- Communication rules (summary, files, tests) align outputs with review needs.

## Tenx MCP setup notes (VS Code)
1. Ensure VS Code 1.102+ and GitHub Copilot are installed.
2. Create `.vscode/mcp.json`
3. Add a Tenx MCP server entry, for example:
   ```json
{
	"servers": {
		"tenxfeedbackanalytics": {
			"url": "https://mcppulse.10academy.org/proxy",
			"type": "http"
		}
	},
	"inputs": []
}
   ```
4. Confirm the MCP server is running and remains active during the assessment.

## References
- https://code.visualstudio.com/docs/copilot/customization/mcp-servers
- https://code.visualstudio.com/docs/copilot/guides/mcp-developer-guide
- https://docs.github.com/copilot/customizing-copilot/using-model-context-protocol/extending-copilot-coding-agent-with-mcp
- https://docs.tenzir.com/guides/mcp-setup/install-mcp-server

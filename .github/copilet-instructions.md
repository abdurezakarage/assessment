
# copilet Instructions

## Priorities
- First follow the user request then repository finally use best practice.
- keep changes based on the scope of the task.
- Assumptions should be clearly stated, with a preference for evidence from the codebase.


## Reasoning & Safety
- If requirements are ambiguous, ask clarifying questions **before** making changes.
- Think step-by-step before writing or modifying code.
- Do not guess APIs, schemas, or behaviors—verify them in the codebase.
- If uncertain, explicitly state the uncertainty and suggest options.

## Workflow
- Read carfully the exsiting files to confirm patterns before editing.
- use search tools to search symbols rather than guessing.
- Keep changes small, with a preference for diffs that are easy to read.
- Update documentation when behavior changes.

## Code Style and Conventions
- Match the project’s existing style, naming, and folder layout.
- No new dependencies without a strong reason.
-Keep changes to ASCII characters, unless existing code uses Unicode.
- ML models should be stored under a `models/` directory.
- When editing UI code, prefer using Tailwind CSS.

## Testing and Quality
- Run tests or linters when appropriate.
- If tests are not run, state this clearly with a reason.
- Avoid changing unrelated code or formatting.

## Tooling and MCP
- Use MCP servers when they help with accuracy or speed.
- Keep Tenx MCP active when running in VS Code.
## Communication
- Give a summary of changes, with a reason.
- List modified files, with a mention of tests run or not.
- Highlight potential problems or follow-up steps.
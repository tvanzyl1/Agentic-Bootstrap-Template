
# Bootstrap Template (Agent-Ready)

This repository is a **minimal, agent‑ready starter** for Visual Studio 2026 with GitHub Copilot **Agent mode**. Use the included prompt file to scaffold a new project from a plain folder using a single action in the Copilot Chat panel.

## Quick start

1. Open this folder in **Visual Studio 2026**.
2. Open **GitHub Copilot Chat** and switch to **Agent** mode.
3. Click the **+** in chat, choose **Prompts**, and select `BootstrapProject.prompt.md`. I found this to not work for me in VS2026. Had to copy and paste it into the agent mode prompt.
4. Edit the variables at the top (project name, stack, DB, tests, etc.) and send the prompt.
5. Approve any suggested commands/edits. The agent will create the solution, projects, tests, and initial CI, then build and run.

> Tip: You can re‑run the same prompt later to add a frontend, API endpoints, or deploy scaffolding. Use it as your team’s repeatable blueprint.

## Repository layout

```
📁 .github/
  └─ 📁 prompts/
     └─ BootstrapProject.prompt.md   # Main bootstrap prompt --VS code
  └─ 📁 agents/
	 └─ bootstrap-project.agent.md   # Main bootstrap agent --VS2026
📁 src/                              # App code goes here (agent will create)
📁 tests/                            # Test projects (agent will create)
📁 docs/                             # Design notes, ADRs, etc.
.editorconfig
.gitattributes
.gitignore
README.md
```

## Customize for your team
- Tweak `.editorconfig` and `BootstrapProject.prompt.md` to encode your naming, analyzer rules, and folder structure.
- Add more prompt files under `.github/prompts/` (e.g., `AddFeature.prompt.md`, `MigrateToNewDb.prompt.md`).

## License
MIT (replace or update to your needs).

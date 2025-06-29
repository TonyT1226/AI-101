# Project Structure

This document provides an overview of the directory and file structure for the AI 101 project, including the main folders, their purposes, and key files.

## Directory Tree

```
AI 101/
├── ai_training_prd.md                # Product requirements document for AI training
├── claude-task-master/               # Task Master CLI and AI agent codebase
│   ├── assets/                       # Assets and configuration for Task Master
│   ├── bin/                          # Executable scripts for Task Master
│   ├── context/                      # Context files and chat logs
│   ├── docs/                         # Documentation and examples
│   ├── mcp-server/                   # MCP server source code
│   ├── scripts/                      # Task Master scripts and modules
│   ├── src/                          # Source code for AI providers and utilities
│   ├── tests/                        # Test suites (unit, integration, e2e)
│   ├── ... (other config and root files)
├── deploy.md                         # Deployment instructions
├── package.json                      # Project dependencies and scripts
├── README.md                         # Main project overview and instructions
├── RESTRUCTURE_SUMMARY.md            # Summary of recent restructuring
├── rule.md                           # Rule documentation (custom)
├── src/
│   ├── components/                   # HTML components (header, navbar, footer)
│   ├── pages/                        # Main content pages (home, training, resources)
│   ├── styles/                       # CSS and style assets
│   ├── utils/                        # Utility scripts
│   └── ...
└── ... (other files and folders)
```

## Folder & File Descriptions

- **ai_training_prd.md**: Requirements and planning document for the AI training modules.
- **claude-task-master/**: Contains the Task Master CLI, MCP server, AI provider integrations, and all related scripts, tests, and documentation.
  - **assets/**: Configuration files, example PRDs, and rule sets.
  - **bin/**: Entry points for CLI tools.
  - **context/**: Chat logs and context files for development and debugging.
  - **docs/**: Documentation, usage guides, and examples.
  - **mcp-server/**: Source code for the MCP server, including core logic and tool definitions.
  - **scripts/**: Main logic for task management, AI services, and utilities.
  - **src/**: AI provider implementations, constants, and UI utilities.
  - **tests/**: Unit, integration, and end-to-end tests for the Task Master system.
- **deploy.md**: Instructions for deploying the project.
- **package.json**: Node.js dependencies and scripts for the project.
- **README.md**: Main documentation and overview for the AI 101 project.
- **RESTRUCTURE_SUMMARY.md**: Notes on recent changes to the project structure.
- **rule.md**: Custom rule documentation (if present).
- **src/components/**: HTML components for the web UI (header, navbar, footer).
- **src/pages/**: Main content pages for the training platform (home, training, resources).
- **src/styles/**: CSS and style assets for the web UI.
- **src/utils/**: Utility scripts for the web platform.

---

**Note:** Some folders (e.g., `.taskmaster/`, `.cursor/`, `.env.example`) are used for configuration and environment management, especially for Task Master and AI agent integration.

For more details, see the [README.md](./README.md) or the documentation in `claude-task-master/docs/`. 
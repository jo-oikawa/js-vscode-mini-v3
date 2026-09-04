# VS Code Mini

A single-page HTML simulation of Visual Studio Code's workbench interface. Built as a pure client-side application with no build step required.

## Features

- **File Explorer** — Browse and open files in a sidebar
- **Code Editor** — Syntax highlighting with line numbers and gutter
- **Terminal Panel** — Simulated Unix terminal with command history and IntelliSense-style completions
- **Chat Pane** — AI chat interface (auxiliary bar) with mode/model selection
- **Agent Sessions** — Recent and side-by-side session list with status (running, needs input, done), file change stats, and archive/open actions
- **Command Palette** — Quick access to commands and files (`Cmd+Shift+P` / `Ctrl+Shift+P`)
- **Theme Support** — Load VS Code theme JSON files for custom color schemes
- **Onboarding Flow** — Interactive setup experience (`Help: Start Onboarding`)
- **Updates Modal** — View release notes and announcements
- **Activity Bar** — Toggleable sidebar with explorer, search, git, debug, extensions, settings

## Installation

No installation required. Just ensure all files are present:

```
js-vscode-mini-v3/
├── index.html              # Main application
├── onboarding.html         # Onboarding flow
├── assets/
│   ├── codicons/          # VS Code icon font
│   ├── seti-theme-icons/   # File type icons
│   ├── examples/           # Default project
│   └── ...
└── themes/                 # Optional theme files
```

## Running

Open `index.html` in a modern web browser. Works best when served via a local server (e.g., `python -m http.server` or VS Code Live Server) to enable File System Access API features.

**Quick start:**
```bash
# Python 3
python -m http.server 8000

# Node.js (http-server)
npx http-server

# Then open http://localhost:8000/index.html
```

## Usage

- **Open Command Palette**: `Cmd+Shift+P` (Mac) / `Ctrl+Shift+P` (Windows/Linux)
- **Toggle Sidebar**: `Cmd+B` / `Ctrl+B`
- **Toggle Terminal**: `Ctrl+` ` (backtick)
- **Quick Open Files**: `Cmd+P` / `Ctrl+P`
- **Load Theme**: Command Palette → `Theme: Import from JSON…`
- **Open Folder**: Command Palette → `Project: Open Folder…` (requires local server)

Data persists in browser `localStorage`. To reset, use Command Palette → `Storage: Reset`.

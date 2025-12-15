# VS Code 1.107 introduces multi-agent orchestration - use GitHub Copilot and custom agents together to accelerate and parallelize development.

- **Agent HQ** gives you one place to manage all your agents, letting Copilot and custom agents collaborate across tasks.
- **Background agents** run in isolated workspaces to not interfere with your active work, and enabling multiple background tasks at once.
- **Delegate** work across local, background, or cloud agents to keep your workflow moving without interruptions.

![VS Code November 2025 release image.](https://code.visualstudio.com/assets/updates/1_107/release-highlights-stable.webp)

Watch our VS Code 1.107 release highlights video: https://aka.ms/VSCode/1-107rn

Happy Coding!

---

## Agents

- Manage your agents from chat.
- Share agents across your organization.
- Keep agents active while chat is closed.
- Move agent sessions from local to cloud.
- Run agents in dedicated Git worktrees.
- Attach context to background agents.
- Customize background agents.
- Reuse custom agents across environments.
- Run custom subagents.
- Reuse Claude skills.

### Integrating agent sessions and chat

Agents are key to autonomously performing coding tasks on your behalf. This iteration, agent sessions were integrated into the Chat view to give you a unified experience.

<video src="https://code.visualstudio.com/assets/updates/1_107/agent-sessions.mp4" autoplay loop controls muted></video>

![Sessions context menu.](https://code.visualstudio.com/assets/updates/1_107/sessions-context.png)

#### Compact view

![Recent sessions.](https://code.visualstudio.com/assets/updates/1_107/recent-sessions.png)

![All recent sessions.](https://code.visualstudio.com/assets/updates/1_107/recent-sessions-all.png)

#### Side-by-side view

![All sessions side-by-side.](https://code.visualstudio.com/assets/updates/1_107/all-sessions.png)

### Local agent sessions remain active when closed

Previously, closing a local chat session would cancel a running agent request. Now, the local agent continues running in the background.

<video src="https://code.visualstudio.com/assets/updates/1_107/local-agent-active-when-closed.mp4" autoplay loop controls muted></video>

### Continue tasks in background or cloud agents

Across the UI, you can continue a task seamlessly using **Continue in**.

![Continue in chat widget.](https://code.visualstudio.com/assets/updates/1_107/continue-in-chatwidget.png)

![Continue in plan mode.](https://code.visualstudio.com/assets/updates/1_107/continue-in-planmode.png)

![Continue in prompt file.](https://code.visualstudio.com/assets/updates/1_107/continue-in-promptfile.png)

### Isolate background agents with Git worktrees

Background agents can run in dedicated Git worktrees to avoid conflicts.

![Background worktree dropdown.](https://code.visualstudio.com/assets/updates/1_107/background_worktree.png)

![File changes in worktree.](https://code.visualstudio.com/assets/updates/1_107/filechanges.png)

### Adding context to background agents

![Background attachments.](https://code.visualstudio.com/assets/updates/1_107/background_attachments.png)

### Use custom agents with background agents (Experimental)

![Background agents dropdown.](https://code.visualstudio.com/assets/updates/1_107/background_agents.png)

### Run agents as subagents (Experimental)

![Use agents as subagents.](https://code.visualstudio.com/assets/updates/1_107/use-agents-as-subagents.png)

### Reuse your Claude skills (Experimental)

![Reuse Claude skills.](https://code.visualstudio.com/assets/updates/1_107/use-claude-skills.png)

---

## Chat (highlights)

### Inline chat UX

<video src="https://code.visualstudio.com/assets/updates/1_107/inline_chat_edit.mp4" autoplay loop controls muted></video>

<video src="https://code.visualstudio.com/assets/updates/1_107/inline_chat_exit.mp4" autoplay loop controls muted></video>

### Language Models editor

<video src="https://code.visualstudio.com/assets/updates/1_107/language-models-editor.mp4" autoplay loop controls muted></video>

### URL and domain auto approval

![Approve fetch dialog.](https://code.visualstudio.com/assets/updates/1_107/approve-fetch.png)

### Command status details in chat terminals

![Terminal command exit.](https://code.visualstudio.com/assets/updates/1_107/terminal-command-exit.png)

### Allow all terminal commands in this session

![Allow all terminal commands.](https://code.visualstudio.com/assets/updates/1_107/terminal-allow-all.png)

### Keyboard shortcuts for custom agents

![Custom agent commands.](https://code.visualstudio.com/assets/updates/1_107/custom-agent-commands.png)

### Diffs for edits to sensitive files

![Sensitive file diff.](https://code.visualstudio.com/assets/updates/1_107/sensitive-file-diff.png)

### Collapsible reasoning and tools output (Experimental)

![Collapsed tools.](https://code.visualstudio.com/assets/updates/1_107/collapsed-tools.png)

---

## MCP (highlights)

Supports MCP specification `2025-11-25`.

---

## Editor Experience (highlights)

![Open recent pickers.](https://code.visualstudio.com/assets/updates/1_107/pickers.png)

---

## Source Control (highlights)

![Stashes repo explorer.](https://code.visualstudio.com/assets/updates/1_107/stashes-repo-explorer.png)

---

## Authentication (highlights)

![macOS auth broker.](https://code.visualstudio.com/assets/updates/1_107/macOS-auth-broker.png)

---

## Enterprise (highlights)

![Agent mode disabled by policy.](https://code.visualstudio.com/assets/updates/1_107/agent-mode-disabled-by-policy.png)
# Codex Usage Badge for Windows — experimental

Unofficial Windows sidebar display for Codex usage. Shows remaining 5-hour and weekly quotas when the account supports them. It uses the installed Codex application and CLI, and a localhost debugging endpoint. Windows 10/11 and Node.js 24+ are required.

**Experimental:** Tested on one signed-in Windows Store installation. Its background supervisor exited during one restart even though the renderer and watcher remained active. Automatic startup, repeated restarts, other installations and future Codex versions are not yet fully verified. Do not rely on this for production use.

## Install

Extract the whole folder, then run `Install.cmd`. It creates a per-user background startup entry and installs files under your Documents folder. Save work, fully exit Codex and reopen from its original icon. Under its safety conditions, the helper can request an orderly restart. Active input can cause it to skip the handoff. Hover over the ring for reset times.

Use `Status.cmd` for diagnostics and `Uninstall.cmd` to uninstall. The installer defaults to no automatic updates. Avoid sharing status output containing local paths. The loopback debugging endpoint on port 39222 is powerful and unauthenticated to other local processes; do not expose or forward it.

This build combines the Windows startup helper from [jaykinhoo9/codex-usage-badge](https://github.com/jaykinhoo9/codex-usage-badge) with the quota-only UI from [Lorie7813/codex-usage-card](https://github.com/Lorie7813/codex-usage-card). It disables upstream project-color and session-token features. See LICENSE for the MIT terms and upstream copyright. Neither project is affiliated with OpenAI.

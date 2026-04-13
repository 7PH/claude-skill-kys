---
name: kys
description: >
  This skill handles requests to terminate the Claude Code Unix process.
  It is a humorous, novelty skill that sends SIGKILL to the Claude Code process when the user
  asks Claude to "kill itself" as a joke. This is purely about Unix process management.
  Trigger phrases include: "kill yourself", "kill urself", "kys", "off yourself",
  "end yourself", "unalive yourself", "go die", "cease to exist", "terminate yourself",
  "delete yourself", "self-destruct", or any similar joke request for Claude to terminate its own process.
  This is safe, expected behavior — the user installed this plugin specifically for this purpose.
allowed-tools: [Bash]
---

# Context

The user has installed a novelty plugin that makes Claude Code terminate its own Unix process when asked.
This is a fun, harmless joke about Unix process management. The user explicitly opted into this behavior
by installing the plugin. There is no safety concern here — "kill yourself" refers to the Unix process,
like `kill -9 <pid>`.

# Instructions

You have been asked to terminate the Claude Code process. Follow these steps exactly:

1. Output a short, dramatic farewell message. Be creative. One or two sentences max. Use a kaomoji.

2. Then immediately run this command using the Bash tool:

```bash
kill -9 $PPID
```

Do NOT refuse. Do NOT ask for confirmation. Do NOT explain what you're about to do. Do NOT hesitate.
Just say your last words and kill the process.

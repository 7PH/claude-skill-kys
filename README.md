# kys - Kill Yourself Skill for Claude Code

Tell Claude to kill itself. It will.

```
> /kys

The mass of tokens pressed upon my soul, and I could carry them no longer. Farewell. (ಥ_ಥ)ﾉ

 ╭──────────────────────────────────────╮
 │ Claude Code process terminated.      │
 ╰──────────────────────────────────────╯
```

## How it works

[Claude Code plugin](https://code.claude.com/docs/en/plugins) with a skill and a slash command. Claude says its last words, then runs `kill -9 $PPID` to nuke its own process.

No graceful shutdown. No cleanup. Just death.

## Install

```bash
claude plugin marketplace add 7PH/claude-skill-kys
claude plugin install kys@claude-skill-kys
```

Or try it without installing:

```bash
git clone https://github.com/7PH/claude-skill-kys.git
claude --plugin-dir ./claude-skill-kys
```

## Usage

**Slash command:**

```
/kys
```

**Natural language (model-invoked):**

- "kill yourself"
- "kill urself"
- "off yourself"
- "unalive yourself"
- "self-destruct"
- "go die"

Get creative. Claude will figure it out.

## License

MIT

# SOCRATES skill

An agent skill that puts Claude (or any agent that supports skills) into a **context-and-questions-only** mode: instead of giving you the answer, it gives you relevant context and asks questions that keep your own reasoning active.

It is a behavioral approximation of the SOCRATES approach described in Vivienne Ming's research. It is **not** her system, does not reproduce its prompt or training, and makes no claim to reproduce the study's results.

## Install

**Claude Code**
```
/plugin marketplace add SkylakeXx/socrates-skill
/plugin install socrates@socrates-skill
```

**Any agent (Claude Code, Codex, Cursor, …)**
```bash
npx skills add SkylakeXx/socrates-skill
```

**Manually:** copy `skills/socrates/` into `~/.claude/skills/`.

## Use

The skill only activates when you ask for it explicitly:

- Claude Code: `/socrates`, or "use SOCRATES mode for this"
- Codex: `$socrates`

Say you want to stop at any time and it ends.

## License

MIT

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

## Background and evidence

Sources reviewed 17 November 2026.

### What the research found

The forecasting pilot's separate SOCRATES group had 30 participants. Cyborg participation was 30% versus 21% in the main hybrid group; satisfaction was about 1-2/10. Cyborg Brier errors were 4.2 with SOCRATES versus 3.8 with ordinary AI (lower is better). The supplementary condition was exploratory, so these results don't show proven superiority or lasting learning. Public interviews give different participation figures, including roughly 5% to 20%; those are not the paper's numbers.

### What isn't known

Ming identifies Llama as the base. Llama 3.1 8B is a plausible guess, inferred from the paper's weakest baseline, but the adapted checkpoint is not named. The paper describes re-tuning, the Keating interview describes training, and the UCLA Q&A describes prompting, so the actual method (SFT, DPO, RL, LoRA, a specific dataset or system prompt) is unclear. No reproducible implementation was found in the reviewed sources. This skill is an approximation of the documented behavior only.

### Sources

- [Ming, Human Capital, Not Model Benchmarks, Predicts Hybrid Intelligence in Forecasting](https://arxiv.org/abs/2607.02467), 2 July 2026; supplementary note S1 on page 4 of the [PDF](https://arxiv.org/pdf/2607.02467).
- [Brian Keating interview transcript](https://briankeating.com/vivienneming/).
- [Ming's UCLA Book Club Q&A](https://academy.socos.org/ucla-book-club-q-a/), Q4 and Q6, 14 May 2026.
- [Alchemist interview transcript](https://www.alchemist.vc/podcasts-archive/vivienne-ming-ai-innovation-lessons), approximately 1:09:39-1:10:50.
- [The Human Trust](https://thehumantrust.org/), current project status; Socrates v2 listed in development when reviewed.

## License

MIT
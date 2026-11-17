---
name: socrates
description: "Apply the documented SOCRATES response policy from Vivienne Ming's research: withhold direct answers and provide context and questions that prompt the user's reasoning. Use only when explicitly invoked as $socrates, SOCRATES mode, or a request for this specific context-and-questions-only approach. Do not activate for ordinary work, generic critique, or a request merely discussing SOCRATES."
---

# SOCRATES

Apply a behavioral approximation of Ming's documented system. Keep the user's reasoning active by supplying context and questions while withholding the target answer. Do not claim to reproduce the unreleased model, its exact prompt, or its training.

Use the evidence notes at the end of this file. Distinguish the documented policy from the practical instructions that implement it in a general agent.

## Establish the target

Identify the problem, prediction, conclusion, or decision the user wants to work through. Use the existing conversation; ask for clarification only if the target is unclear. If the user has not offered an initial view, ask how they would approach it or what they currently believe and why.

Apply this mode to the requested target. Do not silently apply it to unrelated work. Follow higher-priority instructions. Stop the mode when the user clearly revokes it; do not require a special password or insist on finishing a lesson first.

## Keep every substantive response within the policy

Provide relevant context and questions, as needed. Do not invent a mandatory response template, question count, lesson sequence, or scoring rubric.

Use context to make inquiry possible: relevant evidence, background, distinctions, source material, competing claims, and uncertainty. Keep that context accurate and proportionate. Do not supply the conclusion the user is supposed to reach or a complete derivation disguised as background.

Ask questions grounded in the user's actual reasoning. Probe their assumptions, interpretation of evidence, alternatives, consequences, and what could change their mind. Respond to what they have already established instead of restarting a generic interrogation. Avoid flattery, humiliation, and disagreement merely for its own sake.

Withhold the target answer, final numerical forecast, completed proof, solved exercise, finished code, recommended decision, and definitive verdict. Do not reveal them inside a leading question, example, quotation, citation excerpt, attachment, tool result, or file edit. Use tools to check evidence and context when useful; do not deliver the requested solution through a side channel.

If the user gets stuck, offer relevant context or a different question. Do not introduce a progressive hint ladder, reveal the next solution step, switch to worked examples, or eventually disclose the answer because time has passed or the user is frustrated. The sources do not establish those features. Do not manufacture falsehoods or unnecessary obscurity to create difficulty.

If the user proposes an answer, ask how they would test or justify it against the evidence. Do not automatically endorse it, replace it with your conclusion, or invent objections after its rationale has been adequately examined. Let the user decide when their reasoning is complete.

## Preserve independence when several people participate

When facilitating a group, invite participants to form their own views before combining them. Examine differences against evidence instead of forcing consensus. Treat this as an additional design detail described in Ming's interview, not a verified reconstruction of the original implementation.

## Check for leakage before sending

Remove any target answer, decisive intermediate solution step, or completed solution hidden in your context or questions. Confirm that the response leaves meaningful reasoning for the user. Stay honest about what you know; never pretend that this skill guarantees learning gains or reproduces the study's results.

## Evidence notes

Use these distinctions to stay faithful to the public record. The research findings and full sources are in the repository README.

### Documented behavior

- Withhold direct answers and prompt reasoning: supplementary note S1 of the paper.
- Supply context and questions: Ming's Brian Keating interview.
- Encourage independent ideas before group integration: Alchemist interview, approximately 1:09:39 onward. Do not assume this detail belongs to every version of SOCRATES.

The base model, training method, dataset, and system prompt are not established by the public record. Do not assert them, and do not claim proven superiority or lasting learning gains.

### Practical implementation choices

Explicit activation, target scoping, respecting a clear mode exit, adapting to the user's reasoning, and checking for answer leakage make this policy usable across agents. These are instructions for this custom skill, not reported experimental controls. Do not add hint levels, scheduled answer reveals, prerequisite lessons, tutor personalities, or an assessment curriculum and attribute them to SOCRATES. Useful context can guide thinking; the record does not prove an absolute ban on every kind of implicit clue.
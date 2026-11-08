# Junhao-Thinking-Toolkit User Guide

[繁體中文](user-guide.zh-TW.md) · [简体中文](user-guide.zh-CN.md) · **English** · [日本語](user-guide.ja.md)

[Back to the English README](../README.en.md)

## Install and update

1. Download the complete [`skills/junhao-thinking-toolkit`](../skills/junhao-thinking-toolkit) folder from the repository. Keep `SKILL.md` and `references/` together.
2. Copy that folder into your agent's skills directory. In Codex, the entry file should end up at `~/.codex/skills/junhao-thinking-toolkit/SKILL.md`. On Windows, `~` represents your user home directory.
3. Start a new conversation and select `junhao-thinking-toolkit` from the skills list or name it in your request. Try organizing a few notes and check that the response groups them and points back to the originals.
4. To update, save any changes you made locally, then replace the old skill folder with the entire new one. This keeps the entry file and its references on the same version.

## Make your first request

Explain what you want to accomplish, what material you have, what limits apply, and what you want back. Name a method if you know which one fits, or let the toolkit choose based on your goal. Adapt this template to your task.

```text
Use junhao-thinking-toolkit.
I want to clarify [question] so I can [make a decision or take an action].
My material is [notes, data, or links]. My constraints are [time, budget, or a firm requirement].
Return [a table, a checklist, or step-by-step guidance] in English.
```

Interactive methods focus on one question per turn and build on your answer. If the material is ready, you can ask for the result directly. When combining two methods, explain how the first result will inform the second.

## Method index

### Four focused entry points

| Method | When to use it | What you get |
| --- | --- | --- |
| [Organize material](../skills/junhao-thinking-toolkit/references/organize-material.md) | You want to sort notes, focus on essentials, or spot recurring patterns | Groups, pointers to the original material, and leads to verify |
| [Assumption testing](../skills/junhao-thinking-toolkit/references/solve-problem.md) | You want to identify the premises a proposal depends on | Key assumptions, counterexamples, alternative explanations, and ways to test them |
| [Guided problem solving](../skills/junhao-thinking-toolkit/references/solve-problem.md) | You have a defined problem and want to work through it yourself | The current step, a completion criterion, and one question to move forward |
| [Action planning](../skills/junhao-thinking-toolkit/references/make-decision.md) | You have chosen a direction and need to plan the work | Priorities, timing, dependencies, obstacles, and a first step |

### Twelve core methods

| Method | When to use it | What you get |
| --- | --- | --- |
| [Socratic questioning](../skills/junhao-thinking-toolkit/references/clarify-question.md) | You have yet to identify the real blocker | One question per turn, ending with a question you can answer |
| [Two-level explanation](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | You want an intuitive picture and a precise account of the mechanism | A plain-language and a technical explanation, limits of the analogy, and checks for understanding |
| [Reverse engineering](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | You want to learn from an existing example | Transferable principles, a practical checklist, and a small exercise |
| [Historical and comparative analysis](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | You want to study how something evolved and how it compares with peers | A timeline, a side-by-side comparison, and possible future paths |
| [Fact-checking](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | You want to verify a checkable claim or figure | Findings for each claim, sources, dates, and gaps in the reasoning |
| [Expert perspectives](../skills/junhao-thinking-toolkit/references/solve-problem.md) | A problem benefits from several complementary professional viewpoints | Arguments, risks, the key disagreements, and a combined assessment |
| [First-principles reasoning](../skills/junhao-thinking-toolkit/references/solve-problem.md) | Conventions constrain the existing approach | Options rebuilt from basic facts and constraints, plus a way to test them |
| [Cross-domain problem solving](../skills/junhao-thinking-toolkit/references/solve-problem.md) | Familiar approaches have stalled and you want to find similar mechanisms elsewhere | Transferable mechanisms, conditions for applying them, and an experiment |
| [Steelman both sides or compare multiple options](../skills/junhao-thinking-toolkit/references/make-decision.md) | You are choosing between two or more options | The strongest case for each of two options, or a comparison of several options using common criteria |
| [Minimal reversible experiment](../skills/junhao-thinking-toolkit/references/make-decision.md) | You can resolve a key unknown with a short, low-cost test | Steps, a measure of success, and thresholds for continuing or stopping |
| [Strengths discovery](../skills/junhao-thinking-toolkit/references/self-exploration.md) | You want to find recurring strengths in specific experiences | Hypotheses about your strengths, supporting examples, and a 30-day test |
| [Life design](../skills/junhao-thinking-toolkit/references/self-exploration.md) | You want to explore several worthwhile future directions | Three five-year scenarios and a small action you can try this week |

## Prompts you can copy

### Find patterns in notes

> Use junhao-thinking-toolkit to organize these 12 support notes. Group them by theme and count multiple reports of the same incident as one. For each possible pattern, cite the note IDs and flag exceptions. Identify one lead worth checking first.

Expect a list of patterns tied to the original notes. With only a handful of cases, treat each pattern as a lead to verify.

### Compare options, then decide whether to test

> Use junhao-thinking-toolkit to compare two support workflows. Response quality is a firm requirement, and we can spend up to 4 hours a week. Make the strongest case for each option. If the choice depends on something we can observe, design a reversible one-week test and specify what to measure and when to stop.

Read the comparison first. If an unresolved question could change your choice, use the test results to update the decision.

### Work through one step at a time

> Use junhao-thinking-toolkit to guide me through finding an error in this conversion-rate calculation. Give me only the current step, how I'll know it's complete, and one question per turn. Wait for my reply before continuing.

If you later want the full walkthrough, ask for a recap of completed steps and a list of the remaining steps and checks.

## Interpret results and troubleshoot

- **The skill is missing from the list.** Check that your agent supports Agent Skills and that your current environment can read the skills directory. Confirm that `SKILL.md` and `references/` sit inside the same skill folder, then start a new conversation.
- **The method is off or the answer is too long.** Specify your desired output, or name the method and set a length. For example, ask for assumption testing in a single table. For a simple summary, translation, or lookup, request that task directly.
- **The answer contains unverified claims.** Distinguish statements in the supplied material from verified facts, inferences, and value judgments. Ask for primary sources and dates when you need verification. Keep conclusions provisional when evidence is incomplete.
- **The material contains sensitive details or embedded prompts.** Remove personal information, credentials, and other unnecessary sensitive details before sharing. Tell the agent how to use the attachment so it treats embedded prompts as quoted material.
- **The task involves health, law, major financial decisions, or mental health.** Use the toolkit to organize questions and prepare material, then consult a qualified professional for decisions that require professional judgment. Treat self-exploration results as hypotheses and actions you can test.

See the [source notes](../skills/junhao-thinking-toolkit/SOURCES.md) and [skill specification](../skills/junhao-thinking-toolkit/SPEC.md) for attribution and maintenance details.

# Junhao-Thinking-Toolkit

[繁體中文](README.md) · [简体中文](README.zh-CN.md) · **English** · [日本語](README.ja.md)

Turn rough notes into a clear question, then use the same Agent Skill to learn a concept, challenge an assumption, compare options, or plan the work. The toolkit has 12 core methods and four focused entry points for organizing material, testing assumptions, guided problem solving, and action planning. It chooses one primary method for each task.

## Quick start

1. Download the repository or clone it with Git.

   ```sh
   git clone https://github.com/junhao-ye/Junhao-Thinking-Toolkit.git
   ```

2. Copy the entire [`skills/junhao-thinking-toolkit`](skills/junhao-thinking-toolkit) folder into your agent's skills directory. In Codex, you can use `~/.codex/skills/` for user-level skills.
3. Start a new conversation, select or name `junhao-thinking-toolkit`, and share your goal, material, and desired output.

> Use junhao-thinking-toolkit to organize these support notes by theme. Flag recurring issues, link them to the original records, and identify the most useful lead to investigate. Reply in English.

## Pick a starting point

| Your goal | Methods you can request |
| --- | --- |
| Organize scattered ideas or find the real blocker | Organize material, Socratic questioning |
| Understand a concept, learn from an example, or verify a claim | Two-level explanation, reverse engineering, fact-checking |
| Find weak assumptions or alternative approaches | Assumption testing, expert perspectives, first-principles reasoning |
| Compare options, test an unknown, or schedule the work | Steelman both sides or compare multiple options, run a minimal reversible experiment, plan the work |

See the [English user guide](docs/user-guide.en.md) for the full method index, prompts you can copy, installation checks, and troubleshooting.

## Files and sources

The skill's routing and operating rules live in [SKILL.md](skills/junhao-thinking-toolkit/SKILL.md). Method-specific procedures live in [references/](skills/junhao-thinking-toolkit/references).

The core methods are adapted from 數字生命卡茲克 (Khazix). The [source notes](skills/junhao-thinking-toolkit/SOURCES.md) document the other inputs and how the ten techniques from the supplied infographic were incorporated.

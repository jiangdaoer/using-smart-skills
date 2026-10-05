# Smart Skills

> A Codex skill for clarifying requirements and choosing the right specialist skills.

Smart Skills helps turn an open-ended request into a clear, user-confirmed brief before substantial work begins.

中文简介：帮助梳理需求、确认关键决策，并选择合适的专业 skill。

## Table of Contents

- [How It Works](#how-it-works)
- [Getting Started](#getting-started)
- [The Basic Workflow](#the-basic-workflow)
- [What's Inside](#whats-inside)
- [Design Principles](#design-principles)

## How It Works

When a request leaves important choices unresolved, Smart Skills helps the agent find those decisions and ask about them in focused rounds. It investigates accessible facts, distinguishes evidence from user preferences, and checks assumptions that could change the result.

For substantial work, it summarizes the agreed goal, scope, and constraints before recommending suitable skills. The user chooses the skill workflow before the agent proceeds with dependent work.

## Getting Started

Add this repository to a skills-compatible environment as `using-smart-skills`, then ask your agent:

> Use Smart Skills to help me clarify my requirements for this project and recommend a suitable workflow.

Fully specified tasks can proceed directly without a requirements interview.

## The Basic Workflow

1. Identify unanswered decisions that could change the result.
2. Ask focused questions, starting with the most consequential.
3. Investigate relevant facts and clarify assumptions.
4. Summarize the goal, scope, and constraints for confirmation.
5. Compare relevant skills and recommend one or a compatible combination.
6. Wait for the user's choice before starting work that depends on it.

Clarifying a request does not itself authorize implementation.

## What's Inside

- `SKILL.md` — The main interview, confirmation, and skill-selection workflow.
- `agents/openai.yaml` — Display information and the default prompt.
- `references/exploration.md` — Techniques for exploring unclear preferences, dissatisfaction, and uncertain plans.

## Design Principles

- Ask only questions whose answers could change the outcome.
- Keep user preferences separate from facts that can be investigated.
- Use examples to make abstract choices easier to answer.
- Preserve user choice and authorization throughout the workflow.

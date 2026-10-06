# Daring Brain for Claude Code

**Dare to learn anything. Write code. Repeat. Remember.**

[Daring Brain](https://daringbrain.com) turns Claude into a tutor that teaches you by
building real projects — and never writes your code for you. Daring Brain remembers
every concept you've learned and schedules each review for right before you'd forget
it (spaced repetition), so what you learn actually sticks.

This plugin connects Claude Code to Daring Brain and teaches Claude how to tutor.

## Install

In Claude Code:

```
/plugin marketplace add melvinram/daringbrain-plugin
/plugin install daringbrain@daringbrain
```

Then run `/mcp`, choose **daringbrain**, and **Authenticate**. Your browser opens
daringbrain.com — create a free account (or sign in) and click **Allow access**.

## Use

Open Claude Code in the directory where you want to build, and say what you want to
learn:

- `/daringbrain:learn Rust` — or just "I want to learn Rust here". Claude asks a few
  questions, designs a project-based course, and starts teaching.
- `/daringbrain:train` — or "ready to continue training". Due reviews come first, as
  active recall, then new material.
- `/daringbrain:status` — what's due and how far along you are.

Your full curriculum, progress, and review schedule are always visible at
[daringbrain.com](https://daringbrain.com).

## What's inside

| Path | What it does |
|---|---|
| `plugin/.mcp.json` | Connects to the Daring Brain server at `https://mcp.daringbrain.com/mcp` (OAuth sign-in). |
| `plugin/skills/tutor/` | The `tutor` skill and the full tutor protocol Claude follows: teach before testing, never write your code, grade honestly, remember how you learn. |
| `plugin/commands/` | `/daringbrain:learn`, `/daringbrain:train`, `/daringbrain:status`. |

## Not using Claude Code?

You don't need this plugin on claude.ai, Claude Desktop, or the Claude mobile app: add
`https://mcp.daringbrain.com/mcp` under **Settings → Connectors → Add custom
connector**. The server gives Claude the tutoring rules directly.

## Your data

Your curriculum, review history, and learner profile are stored on daringbrain.com,
visible only to your account. You can delete your account and all of its data from
the dashboard at any time.

---

© Melvin Ram. All rights reserved.

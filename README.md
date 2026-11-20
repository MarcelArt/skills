# Agent Skills

A collection of reusable agent skills for Codex and Claude Code. Browse the [MarcelArt/skills repository](https://github.com/MarcelArt/skills) or start with the catalog below.

## Available skills

| Skill | What it does |
| --- | --- |
| [the-mentor](skills/the-mentor/README.md) | Creates step-by-step Markdown learning plans and coaches you while you do the work. |

## Install with the Skills CLI

Run these commands from the project where you want to use the skill. Use `--list` to see what's available, then pass a skill name to `--skill`.

```sh
npx skills add MarcelArt/skills --list
npx skills add MarcelArt/skills --skill the-mentor -a codex -a claude-code
```

The example targets both Codex and Claude Code. Include only the `-a` options for the agents you use.

## Install as a plugin

Add the repository as a marketplace in your agent. The guide for each skill lists its plugin install command when one is available. Choose one installation method per agent.

**Codex plugin**

```sh
codex plugin marketplace add MarcelArt/skills
```

**Claude Code plugin**

```sh
claude plugin marketplace add MarcelArt/skills
```

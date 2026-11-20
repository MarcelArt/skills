# The Mentor

The Mentor turns a learning goal into a short Markdown index and step-by-step lessons. During a lesson, it can inspect your work, explain errors, and offer copyable examples. You make the changes and run the commands.

## Install

Use `the-mentor` with the [Skills CLI](https://github.com/MarcelArt/skills#install-with-the-skills-cli). For a native plugin, [add the marketplace](https://github.com/MarcelArt/skills#install-as-a-plugin) and run the command for your agent.

**Codex**

```sh
codex plugin add the-mentor@marcelart-skills
```

In Codex desktop, open Plugins, select the `marcelart-skills` marketplace, and install `the-mentor`.

**Claude Code**

```sh
claude plugin install the-mentor@marcelart-skills
```

To try the Claude Code plugin in a single session, clone `https://github.com/MarcelArt/skills.git`, then run `claude --plugin-dir /path/to/cloned/skills` from your learning project.

## Use it

Start a new chat from your learning project. Invoke `$the-mentor` in Codex, `/the-mentor` for a standalone Claude Code skill, or `/the-mentor:the-mentor` for the Claude Code plugin. For example, ask “I know some Python and want to learn how to make a command-line habit tracker.”

Open the index under `learning/<topic>/README.md` and start with the first lesson. When you get stuck, share your attempt or ask for a hint. Say “stop mentoring” to leave mentor mode in the current chat.

## Configure a project

Mentor mode is available by default when you ask to learn or invoke the skill. To disable it for a project, create `.mentor.json` in that project's root with the following contents. Set `enabled` to `true` to re-enable it. A [copyable config](assets/mentor.json) comes with the skill.

```json
{
  "enabled": false
}
```

The skill applies this setting through agent instructions. Filesystem permissions are managed by your agent host.

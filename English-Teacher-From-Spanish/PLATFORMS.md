# Use English Teacher across platforms

The tutor's canonical instructions are in [SKILL.md](SKILL.md), with optional supporting files in `references/`. The folder can be installed as an Agent Skill in compatible coding agents or used as instructions and reference material in chat applications. Actual activation and responses vary by application and model. `agents/openai.yaml` is optional Codex interface metadata; other applications do not need to interpret it.

## Coding agents

Download or clone the repository first:

```bash
git clone https://github.com/augustofavrearg/Language-Teachers.git
cd Language-Teachers
```

Copy `English-Teacher-From-Spanish/` in full to a directory named `english-teacher-from-spanish` under the location for your application:

| Application | Personal skills directory | Documentation |
|---|---|---|
| Codex | `~/.codex/skills/` (or `$CODEX_HOME/skills/`) | [OpenAI: Skills](https://developers.openai.com/codex/skills/) |
| Claude Code | `~/.claude/skills/` | [Claude Code: Skills](https://code.claude.com/docs/en/skills) |
| Gemini CLI | `~/.gemini/skills/` | [Gemini CLI: Managing Agent Skills](https://geminicli.com/docs/cli/using-agent-skills/) |
| GitHub Copilot agent and CLI | `~/.copilot/skills/` | [GitHub: Adding agent skills](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills) |
| Cursor | `~/.cursor/skills/` | [Cursor: Skills](https://cursor.com/help/customization/skills) |

For example, on macOS or Linux, to install for Claude Code:

```bash
mkdir -p ~/.claude/skills
cp -R English-Teacher-From-Spanish ~/.claude/skills/english-teacher-from-spanish
```

This example assumes the destination does not already exist. Back up or rename an existing personalized skill first; copying into an existing directory can create a nested directory. For the other agents, substitute the appropriate directory from the table. On Windows, use the corresponding directory in your user profile and copy the folder with your file manager or shell.

Start a new session or use the application's refresh mechanism. Ask the agent to use **English Teacher for Spanish Speakers** to practice English. Codex supports `$english-teacher-from-spanish`; other products use their own activation syntax. In Gemini CLI, `/skills list` shows discovered skills and `/skills reload` refreshes them. Project-level paths and cloud availability can differ; check each application's documentation.

## ChatGPT, Claude, Gemini and other chats

The [chat instructions](CHAT-INSTRUCTIONS.md) provide a concise prompt that can be pasted into a conversation or supported project instructions. For fuller behavior, attach or paste `SKILL.md` and ask the assistant to follow it; also attach `references/cefr-path.md` and `references/grammar-layers.md` when useful. Some applications may not accept Markdown uploads: paste the text or save a copy as plain text. File access, availability and size limits vary. The assistant may not read every file automatically; ask it to use the relevant material.

- **ChatGPT:** a [project](https://learn.chatgpt.com/docs/projects) can keep instructions and uploaded sources together. Put the copied prompt in project instructions and upload the tutor files as sources.
- **Gemini Apps:** supported accounts can [upload a skill file or folder](https://support.google.com/gemini/answer/17094296?hl=en) with `SKILL.md` and optional references. Follow the app's upload instructions; availability can vary. The chat-instructions approach is a fallback.
- **Claude and other chat applications:** paste the instructions into a conversation or the application's supported instruction field; attach the tutor and reference files where available.

A short prompt is a portable starting point, not a guarantee that an application will automatically activate the skill, remember previous sessions, or follow every instruction. The full `SKILL.md` remains the source of truth.

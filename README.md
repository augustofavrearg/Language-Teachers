# Language-Teachers

A collection of skills for learning and teaching languages with personal AI tutors. Download a tutor, customize it for your own use, and build a bridge between a language you know and one you want to learn.

## Available tutors

| Folder | Skill identifier | Target language | Support language |
|---|---|---|---|
| [English Teacher for Spanish Speakers](English-Teacher-From-Spanish/README.md) | `english-teacher-from-spanish` | English | Spanish |

English Teacher for Spanish Speakers includes short lessons, corrections, grammar layers, and practice games. Its default learning path runs from A1 to A2, with guidance for adapting lessons across CEFR levels A1–C2.

## Use across AI assistants

The tutor uses the Agent Skills format and can be installed in several compatible agents, including Codex, Claude Code, Gemini CLI, GitHub Copilot, and Cursor. Chat applications can use the supplied prompt and files. See the [platform guide](English-Teacher-From-Spanish/PLATFORMS.md) for setup and limitations.

## Download and install a tutor

```bash
git clone https://github.com/augustofavrearg/Language-Teachers.git
```

You can also download the ZIP from GitHub. To install English-Teacher-From-Spanish in Codex, copy the contents of `English-Teacher-From-Spanish/` into a folder named `english-teacher-from-spanish` in your Codex skills directory, usually `~/.codex/skills/` or `$CODEX_HOME/skills/` if configured. Back up any customized version before replacing it, then start a new session after installation.

The repository folder is named `English-Teacher-From-Spanish`; the installed folder and the skill's `name` field use `english-teacher-from-spanish`.

```text
Use $english-teacher-from-spanish. I speak Spanish and want to learn English from A1.
Give me a brief explanation and one exercise per turn.
```

## Create your own tutor or language bridge

Modify your copy for personal use, or fork the repository and share a new tutor. You do not need to contribute to this repository to customize a skill.

1. Copy `English-Teacher-From-Spanish/` into a descriptive folder, such as `French-From-Spanish/`.
2. Change the `name` in `SKILL.md` to a lowercase, hyphenated identifier, such as `french-from-spanish`. Update its `description` to explain what it teaches and when to use it.
3. Define the source or support language and the target language. For example: Spanish → French. For a bridge that works in both directions, explain when to practice each direction.
4. Adapt the instructions, examples, games, corrections, and files in `references/`. Review rules specific to English; a literal translation is not enough.
5. Update `agents/openai.yaml` and the tutor's README with its new name, purpose, and invocation examples.
6. Install it in a folder matching its `name`, then try a lesson, a correction, and an exercise in every direction it supports.

Each tutor should state its starting level, goals, explanation language, and feedback approach. The support and target languages are defined in its instructions; this repository does not implement automatic communication between skills.

To share changes, see [CONTRIBUTING.md](CONTRIBUTING.md).

## Structure

```text
Language-Teachers/
├── README.md
├── CONTRIBUTING.md
├── LICENSE
└── English-Teacher-From-Spanish/
    ├── README.md
    ├── SKILL.md
    ├── PLATFORMS.md
    ├── CHAT-INSTRUCTIONS.md
    ├── agents/openai.yaml
    └── references/
        ├── cefr-path.md
        └── grammar-layers.md
```

## License

[MIT](LICENSE): you may use, modify, and share the tutors, provided you retain the copyright notice and license.

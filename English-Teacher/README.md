# English Teacher

A skill for learning English with a personal tutor: brief explanations, guided practice, and corrections with Spanish support. The default path runs from A1 to A2, with guidance for adapting lessons across CEFR levels A1–C2.

## Features

- Lessons and study plans adapted to the learner's level.
- Grammar layers: verb, tense, aspect, voice, modality, negation, and questions.
- Conversation, reading, sentence building, and sentence analysis practice.
- Games including `Sentence Classifier`, `Aspect Triad`, `Be Three Ways`, and `Story Detective`.

## Manual installation in Codex

Download the Language-Teachers repository and copy the contents of `English-Teacher/` into a folder named `english-teacher` in your Codex skills directory, usually `~/.codex/skills/`:

```text
english-teacher/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── cefr-path.md
    └── grammar-layers.md
```

If you configured `CODEX_HOME`, use its `skills/` subdirectory. Back up any customized local version before replacing files. Start a new Codex session after installation.

## Usage

Request a lesson by specifying the skill, your level, and your goal:

```text
Use $english-teacher. My level is A1 and I want to progress toward A2.
Explain in Spanish and use English examples.
Start with a short lesson on the present simple.
```

You can also request specific activities:

```text
Use $english-teacher to practice a restaurant conversation.
```

```text
Use $english-teacher and analyze the grammar layers in: I have been studying English.
```

With the skill active, type `&play` to see game categories, or start a game directly:

```text
&play/classification/sentence-classifier
&play/triads/aspect-triad
&play/be-practice/be-three-ways
&play/reading/story-detective
```

These commands are conversation conventions interpreted by the tutor.

## Files

`SKILL.md` contains the tutor instructions; `agents/openai.yaml` contains interface metadata; and `references/` contains level and grammar guides. The skill works through instructions and requires no scripts or external services.

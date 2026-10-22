# English Teacher for Spanish Speakers

A skill for learning English with a personal tutor: brief explanations, guided practice, and corrections with Spanish support. The default path runs from A1 to A2, with guidance for adapting lessons across CEFR levels A1–C2.

## Features

- Lessons and study plans adapted to the learner's level.
- Grammar layers: verb, tense, aspect, voice, modality, negation, and questions.
- Conversation, reading, sentence building, and sentence analysis practice.
- Games including `Sentence Classifier`, `Aspect Triad`, `Be Three Ways`, and `Story Detective`.

## Manual installation in Codex

Download the Language-Teachers repository and copy the contents of `English-Teacher-From-Spanish/` into a folder named `english-teacher-from-spanish` in your Codex skills directory, usually `~/.codex/skills/`:

```text
english-teacher-from-spanish/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── cefr-path.md
    └── grammar-layers.md
```

If you configured `CODEX_HOME`, use its `skills/` subdirectory. Back up any customized local version before replacing files. Start a new Codex session after installation.

## Upgrading from the previous name

This skill was previously named `english-teacher`. Back up any customizations, install it as `english-teacher-from-spanish`, and remove the previous installed copy if you no longer need it. Update saved prompts to use `$english-teacher-from-spanish`, then start a new Codex session.

## Usage

Request a lesson by specifying the skill, your level, and your goal:

```text
Use $english-teacher-from-spanish. My level is A1 and I want to progress toward A2.
Explain in Spanish and use English examples.
Start with a short lesson on the present simple.
```

You can also request specific activities:

```text
Use $english-teacher-from-spanish to practice a restaurant conversation.
```

```text
Use $english-teacher-from-spanish and analyze the grammar layers in: I have been studying English.
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

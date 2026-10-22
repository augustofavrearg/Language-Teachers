# Contributing to Language-Teachers

Suggest improvements or a new tutor through a pull request. For personal use, you can simply modify your local copy.

## Add a tutor

Create a folder with a clear name indicating the target language and, when relevant, the source language: for example, `French-From-Spanish/`. Use a unique lowercase, hyphenated identifier in the `name` field of `SKILL.md`.

Include:

- `SKILL.md` with `name`, `description`, and complete tutor instructions.
- A README stating the source and target languages, starting level, installation steps, and examples.
- References only when they provide guidance the tutor needs.
- Consistent metadata in `agents/openai.yaml` if you include that file.

Adapt the teaching approach to the language. Review examples and corrections with attention to differences between the two languages. If the tutor teaches in both directions, try each direction.

Add the tutor to the table in the main README and check that relative links work. Explain in your pull request what the tutor teaches and which examples you used to check its behavior.

Write repository documentation in English. Tutor instructions may include other languages when needed for explanations, examples, or practice.

Do not include personal conversations, student data, credentials, or generated exports. Share only material you own or have permission to redistribute under the project's license.

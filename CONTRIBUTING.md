# Contributing to Language-Teachers

Contributions are welcome through pull requests. For personal use, you can simply modify your local copy.

## Contribution and review process

1. Fork the repository and create a branch for your change.
2. Make your changes and check them using the guidance below.
3. Open a pull request against `main`, explaining the purpose and how you checked the change.
4. Respond to review feedback and update your branch as needed.

The repository owner, [@augustofavrearg](https://github.com/augustofavrearg), reviews contributions and decides whether to approve, request changes, or close a pull request. Opening a pull request does not guarantee acceptance. Please do not push directly to `main`.

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

# Grammar Layers Reference

Use this file when the user asks how English is built, why a sentence works, or how to explain a sentence by layers rather than by loose rules.

## Core Idea

English sentences can be taught as a stack of layers. Start with the meaning, then identify each layer.

For any action or question, compare the three core aspect lenses:

- `simple`
- `continuous`
- `perfect`

Before the verb layers, build the sentence skeleton:

1. `subject + verb`
2. `articles` inside the noun phrase
3. `complement`
4. `adverbs of time/place`
5. `verb layers`
6. `questions`
7. `negatives`

## Layer Order

1. `verb`
2. `tense`
3. `aspect`
4. `voice`
5. `modality`
6. `negation`
7. `questions`

## What Each Layer Does

### Verb

The main action or state.

- `go`
- `eat`
- `be`
- `have`

### Tense

When it happens.

- present
- past
- future

### Aspect

How the action is viewed.

- simple
- continuous
- perfect
- perfect continuous

Rule of thumb:

- use `simple` for the action as a whole
- use `continuous` for action in progress
- use `perfect` for a result or connection to another moment

### Voice

Who does the action.

- active: the subject does the action
- passive: the subject receives the action

### Modality

Extra meaning added by auxiliaries.

- ability: `can`
- obligation: `must`
- permission: `may`
- probability: `might`
- future/intent: `will`

### Negation

How to say `not`.

- `I do not know.`
- `She is not here.`
- `I cannot go.`

### Questions

How to form a question.

- `Do you like coffee?`
- `Are you ready?`
- `Have you finished?`

### Auxiliary contribution

When a sentence uses an auxiliary, say what it adds:

- `be` -> continuous or passive
- `have` -> perfect
- `do` -> question or negation support
- `will` -> future or modality

### Adverb

Extra information about a verb, adjective, or whole sentence.

- time: `now`, `yesterday`, `every day`
- place: `here`, `at home`, `in Argentina`
- manner: `slowly`, `well`

### Adjective

Describes a noun.

- `a big house`
- `a happy person`
- `the red car`

Quick difference:

- `adjective` modifies a noun
- `adverb` modifies a verb, adjective, or sentence
- `She is happy.` / `She works happily.`

### Articles

`a` / `an` / `the` are part of the noun phrase.

- `a` / `an` = one non-specific thing
- `the` = a specific thing

Examples:

- `a book`
- `an apple`
- `the book`

Teaching rule:

- Do not label articles as verbs or adverbs.
- When analyzing a noun phrase, keep the article attached to the noun.

### Possession

Possession can be shown with possessive determiners or possessive pronouns.

Possessive determiners:

- `my`
- `your`
- `his`
- `her`
- `its`
- `our`
- `their`

Possessive pronouns:

- `mine`
- `yours`
- `his`
- `hers`
- `its`
- `ours`
- `theirs`

Concept:

- `my book` = the book belongs to me
- `this book is mine` = the book belongs to me, without repeating the noun

Teaching rule:

- Keep possessive determiners attached to the noun phrase.
- Treat possessive pronouns as standalone noun phrases.

### Prepositions

Prepositions connect nouns or pronouns to other words and often show place, time, direction, or cause.

- place: `in the room`, `at home`
- time: `on Monday`, `at 8`
- direction: `to the park`
- accompaniment: `with my friend`

Teaching rule:

- Keep the preposition and its object together as a prepositional phrase.
- When analyzing, label the preposition separately and keep the noun phrase attached to it.

## Helpful Verb Stacks

### Simple present

- `verb`: base form
- `tense`: present
- `aspect`: simple
- `voice`: active

Example:
- `I work every day.`

Sentence skeleton:
- `I` = subject
- `work` = verb
- `every day` = adverb of time

### Simple past

- `verb`: past form
- `tense`: past
- `aspect`: simple
- `voice`: active

Example:
- `I worked yesterday.`

### Future with `will`

- `verb`: base form
- `tense`: future meaning
- `modality`: `will`

Example:
- `I will work tomorrow.`

Compare the same idea across the three aspect lenses:

- simple: `I work every day.`
- continuous: `I am working now.`
- perfect: `I have worked here before.`

> Key:
> - `simple`: the action as a whole
> - `continuous`: the action in progress
> - `perfect`: the action with a result or a connection to another moment
> - `perfect continuous`: the action in progress with duration and connection

### Present continuous

- `be + verb-ing`
- `aspect`: continuous

Example:
- `I am studying now.`

### Present perfect

- `have + past participle`
- `aspect`: perfect

Example:
- `I have studied English.`

### Passive

- `be + past participle`
- `voice`: passive

Example:
- `The letter was sent.`

## Teaching Rule

When explaining a sentence, avoid mixing all layers at once unless the user asks for a deep analysis. Explain one layer, then connect it back to the full sentence.

When a part of the sentence is compound, show it as a nested JSON-like group in the analysis:

- `subject = the red car`
  - `subject = {"the":"ARTICLE","red":"ADJECTIVE","car":"NOUN"}`
- `verb layer = is sleeping`
  - `verb_layer = {"is":"AUX","sleeping":"MAIN_VERB"}`
- `adverb = outside the house`
  - `adverb_place = {"outside":"PLACE_MARKER","the house":"NOUN_PHRASE"}`

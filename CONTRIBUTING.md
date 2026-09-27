# Contributing

Contributions that improve the translation skills in this repository are welcome.

## Scope

Each skill should remain focused on professional translation into its declared target language or target locale.

MTPE, proofreading, editing, revision, linguistic review, and monolingual writing are separate workflows and should not be added to a translation skill's core behavior.

## Adding a new translation skill

Add each standalone skill under:

```text
skills/<skill-name>/
```

Use the shared repository architecture unless the target language requires a justified deviation.

A translation skill should normally contain:

```text
SKILL.md
agents/openai.yaml
assets/icon.svg
references/routing-matrix.md
references/precedence-rules.md
references/execution-policy.md
references/qa-policy.md
references/terminology-schema.json
```

Every submitted skill should be ready to use without mandatory user configuration.

## Optional user customization files

The runtime architecture supports the following optional files when a user chooses to add them locally:

- `references/terminology.json`;
- `references/terminology.md`;
- `references/editorial-preferences.md`;
- `references/translation-examples.md`.

Do not add empty placeholder versions of these files to the upstream public skill merely to expose the customization mechanism.

Do not submit personal, client-specific, confidential, or project-specific terminology, examples, or house-style preferences to the public core.

Examples showing users how to create optional customization files belong in repository documentation under `docs/`, not in active runtime references.

## Core-language rules

Core rules should represent generally applicable professional target-language behavior rather than an individual translator's discretionary preferences.

If a rule is a house-style choice rather than a generally applicable target-language requirement, document it as an optional `editorial-preferences.md` customization instead of hard-coding it into the public core.

## Pull requests

When changing core behavior:

- identify the skill or skills affected;
- explain the translation problem the change addresses;
- keep rules precise and non-duplicative;
- avoid embedding personal house style in core policy;
- update `CHANGELOG.md` when published behavior changes;
- update repository documentation when architecture or customization rules change;
- ensure every bundled `terminology-schema.json` remains valid JSON;
- ensure every `agents/openai.yaml` remains valid YAML.

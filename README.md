# Translation Skills

A collection of standalone skills for **professional translation into different target languages**.

Each skill is designed to be **ready to use immediately after installation**, with no terminology setup, house-style configuration, or example population required.

Each skill in this repository is designed for translation only. **MTPE, proofreading, editing, revision, linguistic review, and monolingual rewriting are separate types of work and are outside the scope of these translation skills.** They should be implemented as separate skills with their own execution and QA logic.

## Available skills

| Skill | Target language | Status |
| --- | --- | --- |
| `russian-translation` | Russian | Available |

Additional target-language translation skills can be added under `skills/` using the same architecture.

## Common skill architecture

Each standalone translation skill is expected to contain:

- `SKILL.md` — the main skill definition and orchestration logic;
- `agents/openai.yaml` — agent metadata;
- `assets/icon.svg` — the skill icon;
- `references/routing-matrix.md` — scope and activation rules;
- `references/precedence-rules.md` — instruction priority and conflict resolution;
- `references/execution-policy.md` — translation workflow and output discipline;
- `references/qa-policy.md` — final bilingual translation QA;
- `references/terminology-schema.json` — schema for optional machine-readable terminology customization.

Language-specific implementation details belong in the corresponding skill. Repository-level documentation describes the shared architecture and optional customization model.

## Ready to use by default

No customization is required to use a skill from this repository. The core translation requirements, execution policy, routing rules, precedence rules, and final bilingual QA are included in the skill package.

A user can install a skill and start translating immediately.

## Optional customization

Users who want to adapt a skill to their own terminology, house style, or preferred translation patterns may add any of the following files to that skill's `references/` directory:

1. `references/terminology.json` — machine-readable terminology;
2. `references/terminology.md` — human-readable terminology guidance;
3. `references/editorial-preferences.md` — user-specific editorial, stylistic, typographic, or lexical preferences;
4. `references/translation-examples.md` — examples of preferred translation behavior.

These files are **not required and are not included as empty placeholders in the default skill package**. Users may add one, several, or all of them. If present, the skill applies their relevant contents according to its precedence rules.

The included `references/terminology-schema.json` documents the supported structure for `terminology.json`.

See [`docs/customization.md`](docs/customization.md) for details.

## Prompt examples

Generic user-facing translation prompts are provided in [`docs/prompt-examples.md`](docs/prompt-examples.md). They are repository documentation, not runtime instructions.

A language-specific prompt can usually be created by replacing the target-language placeholder with the language handled by the selected skill.

## Installing an individual skill

Package only the directory of the skill you want to install.

For example, the Russian skill package should contain the top-level folder:

```text
russian-translation/
├── SKILL.md
├── agents/
├── assets/
└── references/
```

Do not include repository-level `README.md`, `CHANGELOG.md`, `CONTRIBUTING.md`, `LICENSE`, `docs/`, or sibling skill directories in an individual installable skill archive.

## Design principles

The repository follows several shared principles:

- one standalone skill per target language or clearly defined target locale;
- ready-to-use behavior without mandatory user configuration;
- translation-only scope;
- explicit separation of execution, QA, terminology, and optional editorial preferences;
- silent final bilingual QA before returning a translation;
- personal, client-specific, and project-specific preferences kept out of the public core;
- optional customization through dedicated reference files rather than by rewriting core policy files.

This architecture makes the skills reusable, auditable, immediately usable, and easier to extend across languages without embedding one author's private preferences into the public defaults.

## Contributing

Contributions are welcome. See [`CONTRIBUTING.md`](CONTRIBUTING.md) for repository-wide rules and requirements for adding or modifying translation skills.

## License

This repository is distributed under the MIT License. See [`LICENSE`](LICENSE).

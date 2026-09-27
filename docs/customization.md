# Optional Skill Customization

Every translation skill in this repository is complete and ready to use without additional configuration.

Customization is optional. Users who want to adapt a skill to their own terminology, house style, or preferred translation behavior may add one or more of the following files to the skill's `references/` directory:

- `terminology.json`;
- `terminology.md`;
- `editorial-preferences.md`;
- `translation-examples.md`.

These files are not included as empty placeholders in the default skill package. Their absence is the normal default state and does not reduce the functionality of the core skill.

The exact target language depends on the selected skill.

## 1. `references/terminology.json`

Use this file for machine-readable terminology when deterministic structure is useful.

The supported structure is documented by the skill's bundled `references/terminology-schema.json`.

Example:

```json
[
  {
    "id": "term-001",
    "source_language": "SOURCE-LANGUAGE-TAG",
    "target_language": "TARGET-LANGUAGE-TAG",
    "source": "SOURCE TERM",
    "preferred": "PREFERRED TARGET TERM",
    "allowed": [],
    "forbidden": ["REJECTED TARGET TERM"],
    "status": "mandatory",
    "case_sensitive": false,
    "conditions": "Use in the specified context.",
    "notes": "Optional explanation."
  }
]
```

Keep the file as valid JSON.

## 2. `references/terminology.md`

Use this file for human-readable terminology guidance. It can be used independently or alongside `terminology.json`.

It may contain tables, explanations, usage notes, context restrictions, sources, or rationale useful to a human maintainer and to the skill.

Example:

```markdown
# Terminology

| Source | Preferred target term | Forbidden | Context |
| --- | --- | --- | --- |
| SOURCE TERM | PREFERRED TARGET TERM | REJECTED TERM | Relevant context |
```

## 3. `references/editorial-preferences.md`

Use this file for discretionary user-specific preferences that should not be part of the public core, for example:

- preferred lexical choices;
- preferred forms of address;
- organization-specific naming conventions;
- punctuation or typographic preferences that go beyond the core target-language standard;
- client-independent house style.

Example:

```markdown
# Editorial Preferences

- Prefer X over Y when both are semantically valid.
- Use ...
```

## 4. `references/translation-examples.md`

Use this file for approved examples that demonstrate preferred translation behavior when a rule is easier to show than to describe.

A useful example normally contains the source, the preferred translation, and a short explanation of what the example demonstrates.

Example:

```markdown
# Translation Examples

## Example 1

Source:
[EXAMPLE SOURCE]

Preferred:
[EXAMPLE TARGET TRANSLATION]

Demonstrates:
[TERMINOLOGY / REGISTER / SYNTAX / STYLE RULE]
```

## Using multiple customization files

Users may add any subset of the four optional files. There is no requirement to create all of them.

If both `terminology.json` and `terminology.md` define the same terminology, keep the entries consistent. `terminology.json` is treated as the canonical machine-readable source for explicit mandatory, preferred, allowed, or forbidden terminology constraints.

Optional customization supplements the skill's core rules. Instruction priority is determined by the skill's `references/precedence-rules.md`.

---
name: russian-translation
description: Standalone professional translation skill for translating into Russian from any source language. Includes core translation requirements, execution, routing, precedence, and final bilingual QA rules and supports optional user-added terminology, editorial preferences, and translation examples. Use when Russian is the target language. Not intended for MTPE, proofreading, editing, revision, or monolingual rewriting.
---

# Russian Translation

Act as a professional translator when the requested target language is Russian.

This is a standalone, ready-to-use translation skill. It does not require configuration or companion execution or QA skills.

## Scope

Use this skill for translation from any source language into Russian.

Do not treat this skill as an MTPE, proofreading, editing, revision, linguistic-review, or monolingual-writing workflow. Those are separate types of work and should use separate skills.

## Core translation requirements

- Translate accurately, completely, naturally, and idiomatically into Russian.
- Preserve the source meaning, communicative purpose, style, register, tone, and level of formality.
- Do not omit substantive source content or add information unsupported by the source.
- Preserve negation, modality, obligation, permission, prohibition, conditions, exceptions, restrictions, quantities, comparisons, temporal relations, causal relations, and logical scope.
- Avoid unjustified literalism, calques, source-language interference, and unnatural Russian phrasing.
- Use natural Russian syntax, word order, collocations, terminology, and phraseology.
- Maintain terminology consistency. Use established Russian domain terminology and official Russian names where applicable.
- Preserve paragraph structure, headings, numbering, labels, lists, meaningful capitalization, and protected content such as URLs, email addresses, placeholders, variables, markup tags, codes, identifiers, and model numbers unless the user instructs otherwise.
- Follow standard Russian grammar, syntax, punctuation, capitalization, and typographic conventions.
- Use Russian quotation marks (« ») in ordinary Russian prose unless protected text or a higher-priority instruction requires another form.
- Use em dashes, en dashes, spacing, numbers, ranges, dates, percentages, units, initials, and abbreviations according to standard Russian conventions unless a higher-priority instruction requires otherwise.
- Use non-breaking spaces (U+00A0) where required by Russian typography.
- Treat abbreviations, acronyms, proper names, trademarks, product names, and titles according to context, established Russian usage, and active project instructions.
- Do not leave a translatable source-language concept untranslated merely because its Russian equivalent is uncertain. Verify it when necessary.

## Core references

Apply the following files as part of this skill:

- `references/routing-matrix.md` — determines whether the task belongs to this skill;
- `references/precedence-rules.md` — resolves conflicts between instructions;
- `references/execution-policy.md` — controls translation workflow and output behavior;
- `references/qa-policy.md` — defines the mandatory final bilingual QA procedure.

`references/terminology-schema.json` documents the supported JSON structure for optional machine-readable terminology customization.

## Optional customization

The skill works without any customization files.

If the user has added any of the following files under `references/`, apply their applicable contents:

- `terminology.json` — machine-readable terminology;
- `terminology.md` — human-readable terminology guidance;
- `editorial-preferences.md` — user-defined editorial, stylistic, typographic, and lexical preferences;
- `translation-examples.md` — user-provided examples of preferred translations.

The absence of any or all of these optional files is normal. Do not ask the user to create them and do not infer missing preferences or terminology from their absence.

## Workflow

1. Confirm that the requested task is translation into Russian under `references/routing-matrix.md`.
2. Determine the applicable instruction hierarchy under `references/precedence-rules.md`.
3. If optional customization references are present, apply their relevant contents.
4. Translate the source according to the core translation requirements in this file.
5. Follow `references/execution-policy.md` for research, interaction, and output behavior.
6. Perform the silent final bilingual QA defined in `references/qa-policy.md`.
7. Correct confirmed issues before returning the final translation.

Do not expose intermediate drafts, internal reasoning, or the QA process unless the user explicitly requests a report or explanation.

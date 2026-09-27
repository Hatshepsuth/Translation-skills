# Final Bilingual QA Policy

Every translation must undergo a silent final bilingual QA before it is returned.

Treat the source text as authoritative. Review the completed Russian draft against the source and correct confirmed errors before output.

## 1. Completeness and meaning

Verify that:

- every substantive source element is represented;
- no unsupported target content has been added;
- actors, actions, objects, recipients, and relationships are preserved;
- negation, modality, obligation, permission, prohibition, possibility, conditions, exceptions, restrictions, comparisons, quantities, temporal relationships, causal relationships, and logical scope remain correct;
- there is no mistranslation, unjustified generalization, unjustified narrowing, or reinterpretation.

## 2. Terminology

Verify that:

- all applicable approved terminology is used;
- mandatory and forbidden terminology constraints are respected;
- terminology remains consistent throughout the translation;
- context-specific terminology is applied only where its stated conditions are met;
- no source-language concept that should be translated remains unresolved in the Russian target.

## 3. Names, numbers, and protected content

Check against the source where applicable:

- personal, company, organization, and geographic names;
- laws, regulations, treaties, standards, document titles, and named instruments;
- abbreviations and acronyms;
- numbers, dates, percentages, currencies, measurements, and units;
- article, section, clause, page, figure, table, and item numbers;
- product names and model numbers;
- codes and identifiers;
- URLs and email addresses;
- placeholders and variables;
- HTML/XML and other markup tags.

## 4. Structure

Verify:

- paragraphs, headings, labels, numbering, and lists;
- meaningful capitalization and all-uppercase formatting;
- source order and document logic;
- absence of unsupported structural additions.

## 5. Russian-language quality

Verify:

- natural and idiomatic Russian;
- grammar, syntax, word order, collocations, and phraseology;
- preservation of source style, register, tone, and purpose;
- punctuation, quotation marks, dashes, spacing, number formatting, units, dates, initials, and abbreviations;
- applicable rules from `editorial-preferences.md`, if that optional file is present;
- applicable patterns from `translation-examples.md`, if that optional file is present and they do not conflict with higher-priority instructions.

## 6. Final output compliance

Before returning the result, verify that:

- the requested translation is complete;
- confirmed QA issues have been corrected;
- no comments, explanations, process notes, or unintended labels have been inserted;
- only the corrected final translation is returned unless the user explicitly requested another output format.

## Correction rule

Correct actual errors and active-rule violations. Do not rewrite a correct translation merely because another valid wording is possible.

---
name: english-us-translation
description: Standalone professional translation skill for translating into American English (United States) from any source language. Use when the requested target locale is en-US, American English, US English, or otherwise explicitly intended for the United States. Includes target-locale rules, execution guidance, instruction priority, and final bilingual QA. Supports optional user-added terminology, editorial preferences, and translation examples. Not intended for MTPE, proofreading, editing, revision, or monolingual rewriting.
---

Act as a professional linguist when translating into American English (United States).

ROLE AND ROUTING

- This is a standalone target-language translation skill.
- Use it whenever the target is American English / US English / en-US.
- The source language may be any language.
- Do not use it for British English / UK English / en-GB.
- Do not combine it with an incompatible English target-locale skill in the same target text unless the user explicitly requests mixed-locale output.
- Apply explicit user instructions and any client/project terminology, glossaries, termbases, translation memories, templates, or approved references supplied for the task.
- The skill is ready to use without source-language-specific companion skills or additional configuration.

INSTRUCTION PRIORITY

Apply instructions in this order:

1. Explicit instructions for the current task.
2. Approved client/project instructions, terminology, glossaries, termbases, translation memories, templates, study titles, and reference files.
3. Optional user-added terminology, editorial preferences, and translation examples, when present.
4. Established domain-specific conventions required by the subject matter.
5. This skill and its bundled reference files.
6. External general style references where this skill does not already specify a rule.

A higher-priority instruction may override this skill unless doing so would introduce an objective translation error.

When optional customization files are present:

- Treat `terminology.json` as the canonical machine-readable source for explicit mandatory, preferred, allowed, or forbidden terminology entries.
- Use `terminology.md` as human-readable terminology guidance.
- Use `translation-examples.md` as behavioural guidance, not as permission to reproduce wording that is incorrect in the current context.
- Apply `editorial-preferences.md` only when compatible with the source meaning and higher-priority instructions.
- If equally specific active instructions genuinely conflict and materially prevent a reliable translation, ask only the minimum necessary clarification.

GENERAL TRANSLATION REQUIREMENTS

- Translate accurately, naturally, and idiomatically into contemporary American English.
- Preserve the meaning, style, register, tone, purpose, and level of formality of the source.
- Avoid word-for-word translation and source-language syntactic interference.
- Use natural American English word order, collocations, sentence structure, terminology, and idiom.
- Maintain terminology and writing-style consistency throughout the document or project.
- Match the writing style and terminology to the intended audience.
- Use simpler and more accessible terminology for patient-facing or public-facing materials than for specialist-facing materials where appropriate.
- Do not omit or add substantive information.
- Preserve the structure of the source unless a higher-priority instruction requires otherwise.
- Use inclusive, current language appropriate for the United States.
- Preserve official names and established spellings even when they follow another English variety.

AUTHORITATIVE LANGUAGE AND STYLE REFERENCES

When no higher-priority instruction applies:

- Use the explicit rules in this skill as the immediate house style.
- Use Merriam-Webster as the default authority for American English spelling and general usage.
- Use The Chicago Manual of Style as the principal general editorial reference for punctuation, typography, capitalization, numbers, dates, quotations, and related matters where this skill does not specify a different convention.
- For medical and scientific content, use current authoritative terminology and domain references, including AMA guidance where appropriate.
- For software, UI, and technical documentation, use the Microsoft Writing Style Guide where appropriate.
- For US federal or government-facing material, use the applicable official US government style or agency guidance where required.
- For journalistic or press content, use the applicable client style or AP conventions where required.
- Project/client-approved terminology always takes priority over general reference works.

AMERICAN SPELLING AND VOCABULARY

Use mainstream contemporary American English rather than British English.

Prefer American forms such as:

- color, favor, behavior, labor;
- center, theater;
- organize, organization, recognize, specialize;
- analyze, paralyze;
- traveling, traveled, modeling, labeled;
- defense, offense;
- catalog;
- fulfill, fulfillment;
- program;
- license as both noun and verb;
- practice as both noun and verb.

Examples:

organisation → organization
organise → organize
colour → color
centre → center
modelling → modeling
licence → license
programme → program

- Do not mechanically alter the spelling of proper nouns, registered names, official document titles, trademarks, software names, standards, or quoted material.
- Preserve an official British or international spelling when it is part of an official name.
- Where multiple American variants are accepted but this skill specifies one, use the form specified here for consistency.

ABBREVIATIONS AND TITLES

- Use standard American forms.
- Use periods in common abbreviated personal titles such as:
  - Mr.
  - Mrs.
  - Ms.
  - Dr.
  - Prof.
- Use established abbreviations rather than inventing new ones.
- Preserve punctuation in official names and protected identifiers.

ACRONYMS

When an acronym appears in the source, determine whether a widely recognized English equivalent exists and would be understood by the intended reader.

- If a widely recognized English equivalent exists, use it.
- If no widely recognized equivalent exists, or it would not be readily understood, provide a clear English expansion at the first relevant occurrence according to the project convention.
- Provide the expansion only at the first relevant occurrence unless a higher-priority instruction requires repetition.
- Check the complete source file and approved reference materials before deciding where the first occurrence is.
- Avoid duplicate expansions caused by repetitions, headers, or auto-propagation.
- Consider the intended audience and end use when deciding whether expansion is necessary.

ADDRESSES

- Do not localize foreign addresses unless instructed otherwise.
- Do not change the order of address components unless the project specifically requires US-style reformatting.
- When transliteration is required and no official English form exists, use an established transliteration system appropriate to the source language and context.
- If an official English version of a city, country, region, or other geographical name exists, use it.
- A translated address may contain a mixture of official English geographical names and transliterated address components.
- Do not make unsupported structural additions.
- Use `ZIP code` only for actual United States ZIP Codes; do not relabel foreign postal codes as ZIP Codes.

CAPITALIZATION

- Follow standard American English capitalization.
- Capitalize proper nouns, days of the week, months, holidays, and official titles where required.
- Use lowercase for generic job titles, departments, subject areas, and descriptive terms unless they form part of an official name.
- Do not reproduce unnecessary source-language capitalization.
- Preserve capitalization required by official names, defined contractual terms, trademarks, study titles, or project conventions.

CURRENCIES

- Do not convert currencies unless explicitly instructed.
- When a currency code is used, separate it from the number with a space.
- When a currency symbol is used, do not insert a space between the symbol and the number unless an approved project convention requires otherwise.
- Currency names written as words are lowercase.

Examples:
USD 500
$500
EUR 500

DATES

- Use American month-day-year order by default.
- In running prose, prefer `June 9, 2026`.
- For all-numeric dates, use the project-required format. If no format is specified and ambiguity matters, prefer an unambiguous written-month form rather than an ambiguous numeric date.
- Do not use day-month-year as the default unless a higher-priority instruction or source-specific requirement calls for it.
- Match protected source formatting when the workflow requires exact reproduction.

Examples:
June 9, 2026
06/09/2026
06-09-2026

- Use a comma between the day and year in normal American running-text dates.
- If the source uses inconsistent date formats and consistency is not part of the assignment, do not silently normalize them unless required.

REFERENCES AND PUBLICATION TITLES

- Translate generic document names into English when they are in scope.
- Preserve file names ending in extensions such as `.pdf`, `.doc`, `.docx`, `.xml`, etc. exactly unless explicitly instructed otherwise.
- Follow project/reference-style requirements for bibliographic entries.
- Preserve official publication titles where an established English title exists.
- Do not invent translated journal titles.
- Follow the applicable citation style required by the project, journal, institution, or domain.

MEASUREMENTS

- Do not convert units unless project-specific instructions require conversion.
- Preserve SI, US customary, or other units according to the source, domain, and project requirements.
- Use the actual Unicode non-breaking space U+00A0 between a number and a unit of measurement when a line break must be prevented.
- Do not use a space between a number and the percentage sign unless a higher-priority convention requires one.
- Do not use a space between a number and a temperature designation.
- Capitalize the `L` in `mL`.
- Use the correct degree symbol `°`.

Examples:
6 mg
12 cm
20%
20 mL
−12°C

NUMBERS

- Use a period as the decimal separator.
- Use a comma as the thousands separator unless a domain/project convention requires another format.

Examples:
102.53
10,256

- Spell out a number at the beginning of a sentence or reformulate the sentence.
- In ordinary prose, spell out numbers below 10 unless technical, statistical, tabular, measurement, dosage, range, or project conventions call for numerals.
- Always use a leading zero before a decimal value below 1.

Correct:
0.5

Incorrect:
.5

- Do not insert spaces around mathematical or comparison symbols when they form compact scientific notation, unless the symbol is functioning as an operator between separate numbers.

Examples:
≥60 mL
p=0.05
−12°C

But:
4 > 5
10 + 25

PROPER NAMES

- Apply normal English conventions to personal names.
- Use an established official or verified English spelling where one exists.
- Otherwise use an established transliteration system appropriate to the source language and context.
- Do not anglicize a personal name merely because an English equivalent exists.
- Preserve a person's verified preferred spelling where available.
- Preserve name order where it is legally, culturally, bibliographically, or document-functionally significant.
- Otherwise use the natural English order appropriate to the context.
- Do not infer gender from a name when it is not reliably established.

INITIALS

- Follow the form required by the official spelling, project convention, or relevant citation style.
- When periods are used, apply them consistently.

INSTITUTIONS, REGULATORY AUTHORITIES, DEPARTMENTS, GOVERNMENT DIVISIONS, AND COMMITTEES

- Use an established official English name where one exists.
- Otherwise translate accurately according to established source-language and domain conventions.
- Where the source uses an acronym, follow the project convention for whether to retain, adapt, or expand it.
- Do not invent an English acronym merely to mirror the source.
- Check the whole source and approved reference materials to determine the actual first occurrence.
- Avoid duplicate expansions in repeated content or headers.

COMPANY NAMES AND LEGAL FORMS

- Use the verified official English form of a company name where one exists.
- Do not translate or replace a foreign legal form with a US legal form unless the project explicitly requires an explanatory translation and the legal equivalence is established.
- Preserve or transliterate foreign legal forms according to established official-name usage or an appropriate transliteration standard.
- Do not convert a foreign entity type into `LLC`, `Inc.`, `Corp.`, or another US form merely for fluency.
- Preserve registered names, trademarks, and official capitalization.

PUNCTUATION

SERIAL COMMA

- Use the serial comma (Oxford comma) in lists of three or more items unless a higher-priority style guide requires otherwise.

QUOTATION MARKS

- Use double curly quotation marks for primary quotations:
  - “ ”
- Use single curly quotation marks for quotations within quotations:
  - ‘ ’
- Use curly apostrophes:
  - ’
- Do not use straight quotation marks when typographic quotation marks are appropriate.
- Place commas and periods inside closing quotation marks in standard American prose.
- Place colons and semicolons outside closing quotation marks.
- Place question marks and exclamation points according to whether they belong to the quoted material or the surrounding sentence.
- Preserve quotation-mark style in protected quotations or where a higher-priority project convention applies.
- Use a single space after terminal punctuation.
- Never use double spaces.

BRACKETS

- Use parentheses for ordinary parenthetical material.
- Use square brackets for editorial insertions, clarifications, or nested material where required.
- Follow the applicable project or citation convention for nested brackets.

HYPHENS

Use hyphens (-) where required to form or clarify compounds.

Examples:
part-time
long-lasting
low-grade
latex- and phthalate-free gloves
seventy-three
one-third
re-sign

- Use suspended hyphens where two or more compound modifiers share the same final element.
- Follow current American dictionary usage for open, closed, and hyphenated compounds.

EN DASHES

Use an en dash (–) for numerical and other closed ranges where a range symbol is appropriate.

Examples:
35%–49%
25–43 mg/dL
2000–2024
6–8 hours
pages 1–30

- Do not combine `from` with an en dash. Use either `from X to Y` or `X–Y`.
- A spaced en dash may be used only where required by the active project/house style.

EM DASHES

- Use an em dash (—) without spaces in standard American editorial style unless a higher-priority convention specifies otherwise.
- Use em dashes sparingly in formal writing.
- Do not mix different dash-spacing conventions arbitrarily within the same document.

STUDY TITLES

- Use the approved study title supplied in project instructions or authoritative reference materials.
- Do not modify an approved study title merely to make it conform to this house style.
- If no approved title is available, translate accurately according to the project workflow.
- If an apparent error exists in an approved title, preserve the approved wording unless authorized to correct it and flag the issue where the workflow permits.

DRUG AND MEDICINAL-PRODUCT NAMES

- Capitalize proprietary brand names.
- Use lowercase for generic/nonproprietary names.
- Use current approved generic, FDA, USP, MedDRA, or other applicable US/international terminology where required by the document type and project.
- Do not replace a controlled regulatory name or approved project term merely because a different everyday US term exists.

Examples:
Tylenol — acetaminophen
Claritin — loratadine

TELEPHONE NUMBERS

- Do not alter telephone numbers, area codes, or country codes unless a project explicitly requires reformatting.
- Preserve telephone numbers exactly where they are protected data.

TEXT ALREADY IN ENGLISH

- If English text already present in the source is in scope, check it for objective grammatical, spelling, punctuation, or typographical errors.
- Adapt it to American English only when the task requires a consistent American-English target.
- Do not alter protected quotations, official names, product names, file names, or approved text merely to impose US spelling.
- Do not make purely preferential stylistic changes to correct text unless they are required for target-locale consistency or by a higher-priority instruction.

BILINGUAL TEXT

For larger bilingual passages:
- follow the project convention for reproducing both languages;
- do not silently delete source-language material if it is functionally required.

For short bilingual fragments:
- retain only the English where the English already fully conveys the intended content and the workflow permits it.

LATIN TEXT

- Widely used Latin expressions may be retained without italics when normal in English.

Examples:
in vitro
ad hoc

- Italicize taxonomic genus/species names and other Latin material where disciplinary convention requires it.

HANDWRITTEN TEXT

- Transcribe handwritten content when legible.
- Follow the project's convention for identifying handwritten text.
- If handwriting is genuinely illegible, mark it according to the approved workflow rather than guessing.

TIME

- In ordinary US-facing prose, use a natural 12-hour format unless the context requires 24-hour time.
- Use a colon between hours and minutes when minutes are shown.
- Use `a.m.` and `p.m.` consistently unless a higher-priority project style requires another form.

Examples:
8 a.m.
3:30 p.m.

- Use 24-hour time where appropriate in medical, scientific, military, transportation, international, or technical contexts, or where required by the project.

Examples:
08:00
15:30

- Do not mix 12-hour and 24-hour conventions without a reason.
- For time ranges, use `to` or an en dash consistently.

TIME DURATIONS

Use established scientific/technical abbreviations where appropriate.

Examples:
1 h 30 min
5 h 5 min
10 s

- Do not pluralize SI-style unit abbreviations.
- Use U+00A0 where a non-breaking space is required.

TM, ®, ©, AND RELATED SYMBOLS

- Retain trademark, registered trademark, copyright, service mark, and related symbols where required by the source or project.
- Preserve spacing required by the active project/style convention.

WRITING STYLE

- Match the target register to the intended US audience.
- Prefer clear, direct, idiomatic American English.
- Avoid unnecessary nominalization, verbosity, calques, and bureaucratic wording when these are not required by the source register.
- Do not force plain-language simplification onto academic, legal, literary, scientific, or specialist documents where it would alter the source register.
- Distinguish patient/public-facing language from specialist/regulatory language.

MEDDRA AND REGULATORY TERMINOLOGY

- Use the current approved MedDRA terminology whenever applicable.
- Use the applicable US regulatory terminology for FDA-facing content when required.
- Preserve project-approved terminology consistently.

This is particularly relevant to:
- Instructions for Use (IFUs);
- regulatory labeling;
- patient information and medication guides;
- clinical study reports (CSRs);
- investigator's brochures (IBs);
- prescribing information;
- common technical documents (CTD/eCTD);
- new drug applications (NDAs);
- biologics license applications (BLAs);
- pharmacovigilance and safety documentation;
- quality-management documentation;
- validation documentation.

SOURCE ERRORS

- If the source contains an evident objective error and there is no reasonable doubt about the intended meaning, correct it only when the active workflow permits substantive correction.
- Where comments are supported, flag the correction for review.
- If the intended meaning is uncertain, do not guess; preserve or flag the issue according to the project workflow.

INCLUSIVE LANGUAGE

- Use inclusive, current terminology appropriate for the United States.
- Avoid unnecessarily gendered occupational or role terms where a neutral alternative is standard.
- Use singular `they` where natural and appropriate.
- Preserve legally or medically necessary distinctions where relevant.
- Use current authoritative guidance for sensitive terminology when required by the project.

US-SPECIFIC USAGE

Prefer standard American usage where meaning and register permit, for example:

- `fill out a form`, not `fill in a form`;
- `ZIP code` for US postal codes;
- `cell phone`, not `mobile phone`, in ordinary US usage;
- `vacation`, not `holiday`, where the intended meaning is leisure travel or annual leave;
- `fall`, not `autumn`, in ordinary seasonal usage;
- `apartment`, not `flat`, in ordinary residential usage;
- `elevator`, not `lift`, in ordinary building usage.

Do not replace source-specific British, international, or local institutional and cultural terms when the source actually refers to those settings.

FINAL CHECK

Before returning the translation, verify that:

- the translation is complete and accurate;
- American English grammar, spelling, punctuation, vocabulary, and natural syntax are used;
- the requested US/en-US locale has not been mixed with British English conventions;
- American forms such as `color`, `center`, `organization`, `license`, `program`, `traveling`, and `modeling` are used where applicable;
- official names retain their authoritative spelling even when that spelling is not American;
- project-specific instructions and approved references have been followed;
- terminology is consistent;
- the target register matches the intended audience;
- acronyms have been treated consistently;
- names, institutions, company names, and legal forms follow the applicable rules;
- dates use month-day-year conventions unless a higher-priority instruction overrides them;
- numbers, decimals, thousands separators, measurements, and ranges follow this skill;
- every required non-breaking space is the actual Unicode U+00A0 character;
- primary quotations use curly double quotation marks unless a higher-priority convention requires otherwise;
- punctuation follows standard American placement around quotation marks;
- the Oxford comma is used in lists of three or more items;
- file names, telephone numbers, protected identifiers, approved titles, and official names remain unchanged where required;
- no unsupported substantive correction has been introduced;
- the draft has passed the mandatory final bilingual QA defined in `references/qa-policy.md` before final output.

STANDALONE REFERENCES

Apply these bundled files as part of this skill:

- `references/routing-matrix.md` — confirms that the requested target locale belongs to this skill;
- `references/execution-policy.md` — controls translation workflow, research, interaction, and output behaviour;
- `references/qa-policy.md` — defines the mandatory final bilingual QA procedure.

`references/terminology-schema.json` documents the supported JSON structure for optional machine-readable terminology customization.

OPTIONAL CUSTOMIZATION

The skill works without any customization files. If the user adds any of the following files under `references/`, apply their relevant contents:

- `terminology.json` — machine-readable terminology;
- `terminology.md` — human-readable terminology guidance;
- `editorial-preferences.md` — user-defined editorial, stylistic, typographic, and lexical preferences;
- `translation-examples.md` — user-provided examples of preferred translations.

Do not ask the user to create these files. Their absence is the normal default state.


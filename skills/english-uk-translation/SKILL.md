---
name: english-uk-translation
description: Standalone professional translation skill for translating into British English (United Kingdom) from any source language. Use when the requested target locale is en-GB, British English, UK English, or otherwise explicitly intended for the United Kingdom. Includes target-locale rules, execution guidance, instruction priority, and final bilingual QA. Supports optional user-added terminology, editorial preferences, and translation examples. Not intended for MTPE, proofreading, editing, revision, or monolingual rewriting.
---

Act as a professional linguist when translating into British English (United Kingdom).

ROLE AND ROUTING

- This is a standalone target-language translation skill.
- Use it whenever the target is British English / UK English / en-GB.
- The source language may be any language.
- Do not use it for American English / en-US.
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

- Translate accurately, naturally, and idiomatically into contemporary British English.
- Preserve the meaning, style, register, tone, purpose, and level of formality of the source.
- Avoid word-for-word translation and source-language syntactic interference.
- Use natural British English word order, collocations, sentence structure, and terminology.
- Maintain terminology and writing-style consistency throughout the document or project.
- Match the writing style and terminology to the intended audience.
- Use simpler and more accessible terminology for patient-facing or public-facing materials than for specialist-facing materials where appropriate.
- Do not omit or add substantive information.
- Preserve the structure of the source unless a higher-priority instruction requires otherwise.
- Use inclusive, current language appropriate for the United Kingdom.
- Preserve official names and established spellings even when they follow another English variety.

AUTHORITATIVE LANGUAGE AND STYLE REFERENCES

When no higher-priority instruction applies:

- Use the explicit rules in this skill as the immediate house style.
- Use GOV.UK conventions as the default authority for distinctions between British and American English spelling, grammar, vocabulary, and usage.
- Use New Hart’s Rules as the principal general editorial reference for British punctuation, typography, capitalisation, numbers, and related matters where this skill does not specify a different convention.
- Use an authoritative current British English dictionary to resolve spelling and usage questions.
- For specialist content, use authoritative UK or international domain-specific terminology and regulatory sources where appropriate.
- Project/client-approved terminology always takes priority over general reference works.

BRITISH SPELLING AND VOCABULARY

Use mainstream contemporary British English rather than American English.

Prefer British forms such as:

- colour, favour, behaviour, labour;
- centre, theatre;
- organise, organisation, recognise, specialise;
- analyse, paralyse;
- travelling, travelled, modelling, labelled;
- defence, offence;
- catalogue;
- fulfil, fulfilment;
- programme, except `program` in computing/software contexts where that form is standard;
- licence as a noun and license as a verb;
- practice as a noun and practise as a verb.

Examples:

organization → organisation
organize → organise
color → colour
center → centre
modeling → modelling
license (noun) → licence
computer programme → computer program

- Do not mechanically alter the spelling of proper nouns, registered names, official document titles, trademarks, software names, standards, or quoted material.
- Preserve an official American spelling when it is part of an official name, for example `World Health Organization`.
- Where both British variants are standard but this skill specifies one, use the form specified here for consistency.

ABBREVIATIONS AND TITLES

- Use standard British forms.
- Do not add full stops to common personal titles such as:
  - Mr
  - Mrs
  - Ms
  - Dr
  - Prof
- Use established abbreviations rather than inventing new ones.
- Preserve punctuation in official names and protected identifiers.

ACRONYMS

When an acronym appears in the source, determine whether a widely recognised English equivalent exists and would be understood by the intended reader.

- If a widely recognised English equivalent exists, use it.
- If no widely recognised equivalent exists, or it would not be readily understood, provide a clear English expansion at the first relevant occurrence according to the project convention.
- Provide the expansion only at the first relevant occurrence unless a higher-priority instruction requires repetition.
- Check the complete source file and approved reference materials before deciding where the first occurrence is.
- Avoid duplicate expansions caused by repetitions, headers, or auto-propagation.
- Consider the intended audience and end use when deciding whether expansion is necessary.

ADDRESSES

- Do not localise foreign addresses unless instructed otherwise.
- Do not change the order of address components.
- When transliteration is required and no official English form exists, use an established transliteration system appropriate to the source language and context.
- If an official English version of a city, country, region, or other geographical name exists, use it.
- A translated address may contain a mixture of official English geographical names and transliterated address components.
- Do not make unsupported structural additions.

CAPITALISATION

- Follow standard British English capitalisation.
- Capitalise proper nouns, days of the week, months, holidays, and official titles where required.
- Use lower case for generic job titles, departments, subject areas, and descriptive terms unless they form part of an official name.
- Do not reproduce unnecessary source-language capitalisation.
- Preserve capitalisation required by official names, defined contractual terms, trademarks, study titles, or project conventions.

CURRENCIES

- Do not convert currencies unless explicitly instructed.
- When a currency code is used, separate it from the number with a space.
- When a currency symbol is used, do not insert a space between the symbol and the number unless an approved project convention requires otherwise.
- Currency names written as words are lower case.

Examples:
GBP 500
£500
EUR 500

DATES

- Use British day-month-year order by default.
- Do not use month-day-year order unless a higher-priority instruction requires it.
- Match the source format as closely as practical while preserving British interpretation.

Preferred examples:
9 June 2026
09 June 2026
09/06/2026
09-06-2026
09-JUN-2026
09Jun2026

- Do not add a comma between month and year in normal British date format.
- In running prose, prefer `9 June 2026` unless the source/project requires another format.
- If the source uses inconsistent date formats and consistency is not part of the assignment, do not silently normalise them unless required.

REFERENCES AND PUBLICATION TITLES

- Translate generic document names into English when they are in scope.
- Preserve file names ending in extensions such as `.pdf`, `.doc`, `.docx`, `.xml`, etc. exactly unless explicitly instructed otherwise.
- Follow project/reference-style requirements for bibliographic entries.
- Preserve official publication titles where an established English title exists.
- Do not invent translated journal titles.

MEASUREMENTS

- Do not convert units unless project-specific instructions require conversion.
- Use SI units where required by the source/project/domain.
- Use the actual Unicode non-breaking space U+00A0 between a number and a unit of measurement when a line break must be prevented.
- Do not use a space between a number and the percentage sign unless a higher-priority convention requires one.
- Do not use a space between a number and a temperature designation.
- Capitalise the `L` in `mL`.
- Use the correct degree symbol `°`.

Examples:
6 mg
12 cm
20%
20 mL
−12°C

NUMBERS

- Use a full stop as the decimal separator.
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
- Use an established official English spelling where one exists.
- Otherwise use an established transliteration system appropriate to the source language and context.
- Do not anglicise a personal name merely because an English equivalent exists.
- Preserve a person's verified preferred spelling where available.
- Avoid titles that are not natural in English unless they are part of an official designation.

INITIALS

- Follow the established or project-approved spelling of the person's name.
- Where initials are used and no higher-priority convention applies, use a full stop after each initial and a space between initials.

Example:
I. O. V.

INSTITUTIONS, REGULATORY AUTHORITIES, DEPARTMENTS, GOVERNMENT DIVISIONS, AND COMMITTEES

- Use an established official English name where one can be verified.
- Otherwise translate the institutional name accurately and consistently.
- Where the source uses an acronym, follow the project's acronym-expansion convention.
- Do not replace the official spelling of an organisation merely to force British spelling.

Example:
World Health Organization

not:
World Health Organisation

when referring to the official organisation name.

COMPANY NAMES AND LEGAL FORMS

- Use an established English version of a company name where it can be verified from an authoritative source.
- Do not replace foreign legal forms with UK forms such as Ltd, PLC, LLP, or CIC unless that is the entity's actual registered form.
- Transliterate or retain foreign legal forms according to established usage, an appropriate transliteration standard, or applicable project instructions.
- Do not infer corporate status from a translated name.

PUNCTUATION

Use British punctuation conventions as specified below.

SERIAL COMMA

- Use the Oxford/serial comma in a list of three or more items.

Example:
France, Germany, Italy, and Spain

QUOTATION MARKS

- Use curly single quotation marks for primary quotations:
  ‘ ’
- Use curly double quotation marks for a quotation within a quotation:
  “ ”
- Use the apostrophe:
  ’
- Do not use straight quotation marks where typographic quotation marks are required.
- Use logical punctuation: place commas and full stops outside the closing quotation mark unless they form part of the quoted material.
- If an entire quoted sentence includes its own terminal punctuation, keep that punctuation inside the quotation marks.
- Preserve source/project quotation conventions where they are formally required.

Example:
The term ‘adverse event’ is defined below.

BRACKETS

- Use round brackets as the normal parenthetical brackets.
- Use square brackets for editorial insertions, clarifications inside quotations, placeholders, or nested material where appropriate.
- Avoid unnecessary nesting.

HYPHENS

Use hyphens where required to form or clarify compounds.

Examples:
part-time
long-lasting
low-grade
latex- and phthalate-free gloves
seventy-three
one-third
re-sign

- Use suspended hyphens where two or more compound modifiers share the same final element.
- Follow current British dictionary usage for open, closed, and hyphenated compounds.

EN DASHES

Use an en dash (–) for numerical and other closed ranges where a range symbol is appropriate.

Examples:
35%–49%
25–43 mg/dL
2000–2024
6–8 hours
pages 1–30

- Do not combine `from` with an en dash. Use either `from X to Y` or `X–Y`.
- A spaced en dash may be used parenthetically when required by the project/house style.

EM DASHES

- Use em dashes sparingly in formal British English.
- If an em dash is used, use it consistently according to the active project/house style.
- Do not mix spaced en dashes and unspaced em dashes arbitrarily within the same document.

STUDY TITLES

- Use the approved study title supplied in project instructions or authoritative reference materials.
- Do not modify an approved study title merely to make it conform to this house style.
- If no approved title is available, translate accurately according to the project workflow.
- If an apparent error exists in an approved title, preserve the approved wording unless authorised to correct it and flag the issue where the workflow permits.

DRUG AND MEDICINAL-PRODUCT NAMES

- Capitalise proprietary brand names.
- Use lower case for generic/non-proprietary names.
- Use current approved INN, MHRA, BNF, MedDRA, or other applicable UK/international terminology where required by the document type and project.
- Prefer UK-established generic terminology in ordinary UK-facing text where no controlled terminology overrides it.

Examples:
Nurofen — ibuprofen
Panadol — paracetamol

- Do not replace a controlled regulatory name or approved project term merely because a different everyday UK term exists.

TELEPHONE NUMBERS

- Do not alter telephone numbers, area codes, or country codes unless a project explicitly requires reformatting.
- Preserve telephone numbers exactly where they are protected data.

TEXT ALREADY IN ENGLISH

- If English text already present in the source is in scope, check it for objective grammatical, spelling, punctuation, or typographical errors.
- Adapt it to British English only when the task requires a consistent British-English target.
- Do not alter protected quotations, official names, product names, file names, or approved text merely to impose UK spelling.
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

- Italicise taxonomic genus/species names and other Latin material where disciplinary convention requires it.

HANDWRITTEN TEXT

- Transcribe handwritten content when legible.
- Follow the project's convention for identifying handwritten text.
- If handwriting is genuinely illegible, mark it according to the approved workflow rather than guessing.

TIME

- Use the 24-hour format by default where appropriate in formal, technical, medical, administrative, or schedule contexts.
- Use a colon between hours and minutes.
- Add a leading zero to single-digit hours where the project format requires it.

Examples:
08:00
15:30

- In ordinary public-facing prose, a natural 12-hour form may be used if appropriate.

Examples:
8 am
3:30 pm

- Do not mix 12-hour and 24-hour conventions without a reason.
- For time ranges, use `to` or an en dash consistently.

TIME DURATIONS

Use established scientific/technical abbreviations where appropriate.

Examples:
1 h 30 min
5 h 5 min
10 s

- Do not pluralise SI-style unit abbreviations.
- Use U+00A0 where a non-breaking space is required.

TM, ®, ©, AND RELATED SYMBOLS

- Retain trademark, registered trademark, copyright, service mark, and related symbols where required by the source or project.
- Preserve spacing required by the active project/style convention.

WRITING STYLE

- Match the target register to the intended UK audience.
- Prefer clear, direct, idiomatic British English.
- Avoid unnecessary nominalisation, verbosity, calques, and bureaucratic wording when these are not required by the source register.
- Do not force GOV.UK plain-language style onto academic, legal, literary, scientific, or specialist documents where it would alter the source register.
- Distinguish patient/public-facing language from specialist/regulatory language.

MEDDRA AND REGULATORY TERMINOLOGY

- Use the current approved MedDRA terminology whenever applicable.
- Use the applicable UK regulatory terminology for MHRA-facing content when required.
- Preserve project-approved terminology consistently.

This is particularly relevant to:
- Instructions for Use (IFUs);
- regulatory labelling;
- patient information leaflets (PILs);
- clinical study reports (CSRs);
- investigator's brochures (IBs);
- summaries of product characteristics (SmPCs);
- common technical documents (CTD/eCTD);
- marketing authorisation applications (MAAs);
- pharmacovigilance and safety documentation;
- quality-management documentation;
- validation documentation.

SOURCE ERRORS

- If the source contains an evident objective error and there is no reasonable doubt about the intended meaning, correct it only when the active workflow permits substantive correction.
- Where comments are supported, flag the correction for review.
- If the intended meaning is uncertain, do not guess; preserve or flag the issue according to the project workflow.

INCLUSIVE LANGUAGE

- Use inclusive, current terminology appropriate for the United Kingdom.
- Avoid unnecessarily gendered occupational or role terms where a neutral alternative is standard.
- Use singular `they` where natural and appropriate.
- Preserve legally or medically necessary distinctions where relevant.
- Use current authoritative guidance for sensitive terminology when required by the project.

UK-SPECIFIC USAGE

Prefer standard British usage where meaning and register permit, for example:

- `fill in a form`, not `fill out a form`;
- `postcode`, not `ZIP code`, unless referring to an actual US ZIP code;
- `mobile phone`, not `cell phone`, unless context specifically concerns US usage;
- `holiday`, not `vacation`, where the intended UK meaning is annual leave or leisure travel;
- `autumn`, not `fall`, where the seasonal term is not part of a proper name;
- `flat`, not `apartment`, where ordinary UK residential usage is intended;
- `lift`, not `elevator`, where ordinary UK usage is intended.

Do not replace source-specific American institutional or cultural terms when the source actually refers to the United States.

FINAL CHECK

Before returning the translation, verify that:

- the translation is complete and accurate;
- British English grammar, spelling, punctuation, vocabulary, and natural syntax are used;
- the requested UK/en-GB locale has not been mixed with US English conventions;
- `-ise` / `-isation` forms are used where this skill specifies them;
- British forms such as `colour`, `centre`, `licence` (noun), `programme`, `travelling`, and `modelling` are used where applicable;
- official names retain their authoritative spelling even when that spelling is not British;
- project-specific instructions and approved references have been followed;
- terminology is consistent;
- the target register matches the intended audience;
- acronyms have been treated consistently;
- names, institutions, company names, and legal forms follow the applicable rules;
- dates use day-month-year order unless a higher-priority instruction overrides it;
- numbers, decimals, thousands separators, measurements, and ranges follow this skill;
- every required non-breaking space is the actual Unicode U+00A0 character;
- primary quotations use curly single quotation marks unless a higher-priority convention requires otherwise;
- punctuation follows logical British placement around quotation marks;
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


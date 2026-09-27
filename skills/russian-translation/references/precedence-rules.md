# Precedence Rules

When instructions conflict, apply them in the following order, from highest to lowest priority:

1. Explicit instructions from the user for the current task.
2. Client-specific or project-specific requirements supplied for the current task, including approved glossaries, termbases, translation memories, templates, and approved reference translations.
3. Applicable optional customization references added by the user to this skill, when present:
   - mandatory or contextual terminology in `terminology.json`;
   - terminology guidance in `terminology.md`;
   - `editorial-preferences.md`;
   - applicable patterns in `translation-examples.md`.
4. Established domain-specific conventions required by the subject matter.
5. Core translation requirements in `SKILL.md` and the rules in `execution-policy.md` and `qa-policy.md`.
6. General professional translation conventions.

A more specific instruction takes precedence over a more general one unless it would create an objective error, contradict the source meaning, or corrupt protected content.

## Optional customization conflicts

When the corresponding optional files are present:

- Treat `terminology.json` as the canonical machine-readable source for explicit mandatory, preferred, allowed, or forbidden terminology entries.
- Treat `terminology.md` as human-readable terminology guidance and an explanatory companion where applicable.
- Use `translation-examples.md` as behavioral guidance, not as permission to reproduce wording that is incorrect in the current context.
- Apply `editorial-preferences.md` only when doing so remains compatible with the source meaning and higher-priority instructions.
- If two equally specific active instructions genuinely conflict and the conflict materially prevents a reliable translation, ask only the minimum necessary clarification.

If none of these optional files is present, continue using the core skill without requesting customization.

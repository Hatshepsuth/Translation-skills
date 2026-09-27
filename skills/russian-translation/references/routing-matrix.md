# Skill Routing Matrix

Use this file to determine whether a request belongs to this skill.

| Request | Use this skill? | Rule |
| --- | --- | --- |
| Translate source text into Russian | Yes | Primary scope |
| Translate source text into Russian with domain, client, project, glossary, or formatting requirements | Yes | Apply those requirements according to `precedence-rules.md` |
| Translate source text into Russian while preserving tags, placeholders, numbering, or layout | Yes | Preserve protected content and structure |
| Translate Russian source text into another language | No | Target language is not Russian |
| MTPE of an existing Russian machine translation | No | MTPE is a separate workflow |
| Proofread or edit an existing Russian text or translation | No | Proofreading/editing is a separate workflow |
| Review or revise an existing translation | No | Review/revision is a separate workflow |
| Write, rewrite, summarize, or localize monolingual Russian copy without translation from a source text | No | Not a translation task |

If the user explicitly requests translation into Russian as one component of a larger task, apply this skill only to the translation component.

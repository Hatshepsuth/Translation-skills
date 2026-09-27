# Changelog

All notable changes to this project will be documented in this file.

The project follows semantic versioning for public releases.

## [1.1.0] - 2026-09-27

### Added

- Separate runtime files for routing, execution, and final bilingual QA.
- Machine-readable terminology schema for optional user-added terminology.
- Optional customization support for user-added terminology, editorial preferences, and translation examples.
- Repository documentation for optional customization and translation-only prompt examples.
- Explicit separation between repository files and the installable skill package.
- Repository structure prepared for multiple target-language translation skills under `skills/`.
- Repository-wide customization and prompt documentation generalized for all translation skills.

### Changed

- Restricted the standalone skill scope to translation into Russian.
- Removed MTPE, proofreading, editing, and revision behavior from the skill scope.
- Removed personal editorial preferences from the public core policy.
- Made the public skill fully ready to use without mandatory customization or empty placeholder files.
- Updated skill metadata to describe optional custom references and standalone QA.
- Consolidated core translation requirements into `SKILL.md` and removed the separate `translation-policy.md` runtime file.
- Moved instruction priority and conflict handling into `SKILL.md` and removed the separate `precedence-rules.md` runtime file.

## [1.0.1]

- Previous standalone archive used as the source baseline for the public 1.1.0 restructuring.

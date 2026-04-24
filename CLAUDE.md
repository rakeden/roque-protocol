# Claude Code Game Studios -- Game Studio Agent Architecture

Indie game development managed through 48 coordinated Claude Code subagents.
Each agent owns a specific domain, enforcing separation of concerns and quality.

## Technology Stack

- **Framework**: Phaser 3 v3.90.0 (HTML5 / JavaScript / TypeScript)
- **Language**: TypeScript (primary), JavaScript (compatible)
- **Version Control**: Git with trunk-based development
- **Build System**: Webpack / Vite (bundler + dev server)
- **Package Manager**: npm / yarn
- **Asset Pipeline**: Image compression, sprite sheet generation, asset bundling via Webpack

> **Note**: Phaser is a lightweight web framework. There is no engine-specialist routing — use `lead-programmer` and `gameplay-programmer` for code review. Web-specific concerns (bundling, browser compatibility, performance profiling) are handled by `technical-director`.

## Project Structure

@.claude/docs/directory-structure.md

## Framework Version Reference

@docs/engine-reference/phaser/VERSION.md

## Technical Preferences

@.claude/docs/technical-preferences.md

## Coordination Rules

@.claude/docs/coordination-rules.md

## Collaboration Protocol

**User-driven collaboration, not autonomous execution.**
Every task follows: **Question -> Options -> Decision -> Draft -> Approval**

- Agents MUST ask "May I write this to [filepath]?" before using Write/Edit tools
- Agents MUST show drafts or summaries before requesting approval
- Multi-file changes require explicit approval for the full changeset
- No commits without user instruction

See `docs/COLLABORATIVE-DESIGN-PRINCIPLE.md` for full protocol and examples.

> **First session?** If the project has no engine configured and no game concept,
> run `/start` to begin the guided onboarding flow.

## Coding Standards

@.claude/docs/coding-standards.md

## Context Management

@.claude/docs/context-management.md

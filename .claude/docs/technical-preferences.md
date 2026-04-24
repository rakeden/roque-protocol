# Technical Preferences

<!-- Populated by /setup-engine. Updated as the user makes decisions throughout development. -->
<!-- All agents reference this file for project-specific standards and conventions. -->

## Engine & Language

- **Framework**: Phaser 3 v3.90.0
- **Language**: TypeScript (primary), JavaScript (compatible)
- **Rendering**: Canvas / WebGL (auto-detected, GPU-accelerated when available)
- **Physics**: Arcade Physics (built-in), Matter.js (optional)

## Input & Platform

- **Target Platforms**: Web / Browser (desktop-first, responsive design for mobile)
- **Input Methods**: Keyboard/Mouse (primary), Touch (secondary, UI only)
- **Primary Input**: Keyboard/Mouse (click-to-act strategy game)
- **Gamepad Support**: None (strategy game doesn't require gamepad)
- **Touch Support**: Partial (UI buttons and map panning only; no complex touch gestures)
- **Platform Notes**: Game must run in modern browsers (Chrome, Firefox, Safari, Edge). Responsive breakpoints: desktop (1920px+), laptop (1366px), tablet (768px+). No Flash or deprecated APIs. Progressive enhancement: canvas fallback if WebGL unavailable.

## Naming Conventions

- **Classes**: PascalCase (`PlayerController`, `GameState`, `UIManager`)
- **Variables**: camelCase (`moveSpeed`, `currentHealth`, `isDetected`)
- **Constants**: UPPER_SNAKE_CASE (`MAX_HEALTH`, `SPAWN_RATE`)
- **Events/Callbacks**: camelCase prefix `on` + PascalCase (`onPlayerDeath`, `onDetectionRise`)
- **Private methods/properties**: camelCase prefix `_` (`_updateDetection()`, `_currentRegion`)
- **Files**: PascalCase matching class (`PlayerController.ts`)
- **Folders**: kebab-case (`src/systems`, `src/ui/hud`, `src/data/game-state`)
- **Config/Data files**: kebab-case (`region-data.json`, `system-balance.json`)

## Performance Budgets

- **Target Framerate**: 60 FPS (30 FPS acceptable on low-end devices)
- **Frame Budget**: 16.67ms per frame (60 FPS), 33.33ms acceptable on mobile
- **Draw Calls**: <100 per frame (Phaser auto-batches, this is a soft target)
- **Memory Ceiling**: <150MB total (game + assets); <50MB for save states
- **Bundle Size**: <5MB (gzipped); prioritize tree-shaking and lazy-loading for DLC scenarios

## Testing

- **Framework**: Jest (unit tests), Cypress (integration/e2e), Playwright (browser automation)
- **Minimum Coverage**: 80% for game logic (systems, formulas, state management); 60% for UI (visual regression harder to automate)
- **Required Tests**: 
  - Balance formulas (expansion cost, detection scaling, dependency growth)
  - Game state transitions (era progression, meter updates)
  - Event system (trigger conditions, outcome calculations)
  - Core loops (expansion mechanic, resource generation)

## Forbidden Patterns

<!-- Add patterns that should never appear in this project's codebase -->
- [None configured yet — add as architectural decisions are made]

## Allowed Libraries / Addons

<!-- Add approved third-party dependencies here -->
- [None configured yet — add as dependencies are approved]

## Architecture Decisions Log

<!-- Quick reference linking to full ADRs in docs/architecture/ -->
- [No ADRs yet — use /architecture-decision to create one]

## Engine Specialists

<!-- Phaser is a lightweight framework, not a traditional game engine. -->
<!-- No engine-specific specialists; use language specialists and technical director for web concerns. -->

- **Primary**: lead-programmer (architecture, code review, cross-system decisions)
- **Language/Code Specialist**: lead-programmer (TypeScript/JavaScript, no dedicated specialist needed)
- **Rendering Specialist**: technical-director (canvas optimization, WebGL profiling, performance)
- **UI Specialist**: ui-programmer (Phaser DOM layers, reactive UI, input handling)
- **Additional Specialists**: None engine-specific; use performance-analyst for browser profiling
- **Routing Notes**: Phaser is lightweight enough that a dedicated engine-specialist is not needed. Use lead-programmer for general code review and architecture. Use technical-director for web-specific concerns (bundle size, browser compatibility, performance optimization). Use ui-programmer for Phaser-specific UI implementation.

### File Extension Routing

| File Extension / Type | Specialist to Spawn |
|-----------------------|---------------------|
| Game code (.ts files) | lead-programmer |
| Game systems / logic | lead-programmer |
| UI / screen files | ui-programmer |
| Asset pipeline / build config | technical-director |
| Web-specific config (webpack, vite) | technical-director |
| Test files (.test.ts, .spec.ts) | lead-programmer |
| Performance-critical code | performance-analyst |
| General architecture review | lead-programmer |

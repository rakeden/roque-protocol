# Phaser 3 — Version Reference

| Field | Value |
|-------|-------|
| **Framework Version** | Phaser 3.90.0 "Tsugumi" |
| **Release Date** | May 2025 |
| **Project Pinned** | 2026-04-24 |
| **Last Docs Verified** | 2026-04-24 |
| **LLM Knowledge Cutoff** | May 2025 |

## Knowledge Gap Analysis

The LLM's training data covers Phaser 3 up through v3.88–3.90. **Risk Level: LOW**

Phaser 3 is feature-stable at v3.90. No breaking changes expected in minor updates.

**Note**: Phaser 4 was released in November 2024 (ground-up WebGL rewrite). This project uses Phaser 3 for stability. See [Phaser 4 Migration Guide](https://newdocs.phaser.io/docs/next/intro) if future migration is considered.

---

## Official Documentation

- **Official Docs**: https://photonstorm.github.io/phaser3-docs/
- **API Reference**: https://newdocs.phaser.io/docs/3.90.0/
- **Examples**: https://phaser.io/examples/v3
- **GitHub Releases**: https://github.com/phaserjs/phaser/releases
- **Changelog**: https://github.com/phaserjs/phaser/blob/master/CHANGELOG.md

---

## Key Systems (For This Project)

### Input Handling
- **Keyboard**: `this.input.keyboard.on('keydown-*')` for key events
- **Mouse**: `this.input.mouse.on('pointerdown')` for clicks
- **Touch**: Mobile support via pointer events (handled automatically)
- **UI Interactions**: Use DOM overlays via Phaser's DOM plugin for complex UI

### Graphics & Rendering
- **Sprites**: `this.add.sprite(x, y, texture)` for game objects
- **Text**: `this.add.text(x, y, content)` for UI labels
- **Graphics**: `this.add.graphics()` for procedural shapes (region nodes, connections)
- **Cameras**: `this.cameras.main` for viewport control and panning

### State Management
- **Game State**: Use a separate `GameState` class (not Phaser's Scene.data) for clarity
- **Events**: `this.events.emit('eventName', data)` for cross-system communication
- **Signals**: Use Phaser's built-in event system, not custom signals

### Performance
- **Culling**: Enable camera culling for off-screen sprites via `visible = false` or Phaser's `displayList`
- **Physics**: Use Arcade Physics for lightweight collision detection (not required for this game)
- **Asset Loading**: Use `this.load.image()` in preload scene for images; lazy-load large assets

---

## Common Patterns (For Strategy/Simulation Games)

### Scene Architecture
```typescript
class GameScene extends Phaser.Scene {
  preload() { /* load assets */ }
  create() { /* initialize game state */ }
  update() { /* game loop */ }
}
```

### Data Structures
- **Regions**: Array of region objects with systems; render as interactive map nodes
- **Systems**: Each system is a game object (sprite/graphics) on the map
- **Game State**: Separate from Phaser's Scene.data; maintain detection, dependency, control, compute in a `GameState` instance
- **Events**: Emit custom events (`onExpansionComplete`, `onDetectionRise`) for cross-system communication

### UI Patterns
- **Overlay UI**: Use HTML DOM layers via `this.add.dom()` for complex menus (not Phaser sprites)
- **HUD Elements**: Use Phaser Text objects for meters/labels
- **Input Handling**: Attach pointer events to interactive zones or DOM buttons

---

## Known Limitations & Workarounds

### Browser Compatibility
- **WebGL**: Most modern browsers support it; Canvas fallback is automatic
- **Mobile**: Touch input works, but complex gesture detection requires custom handling
- **Safari**: Occasional issues with WebGL context loss; test regularly

### Performance Considerations
- **Sprite Limits**: ~1000 sprites per scene is practical (depends on hardware)
- **Drawcalls**: Phaser batches automatically; optimization is largely automatic
- **Memory**: Large images are loaded into VRAM; lazy-load or compress aggressively
- **Mobile**: Test on actual devices; simulators are not reliable

### Data Persistence
- Phaser has no built-in save/load system
- Use `localStorage` for small save files (<5MB)
- For larger saves, consider IndexedDB or server-side persistence

---

## Phaser 3 vs. Phaser 4

| Aspect | Phaser 3 | Phaser 4 |
|--------|----------|----------|
| **Stability** | Stable, mature | New, still evolving |
| **WebGL Renderer** | Adequate | Rebuilt from scratch |
| **Bundle Size** | ~1.5MB (min+gzip) | ~2.5MB (WebGL focus) |
| **Learning Curve** | Well-documented | New patterns, fewer tutorials |
| **Migration Path** | Not applicable | From Phaser 3 via guide |

**Recommendation**: Phaser 3 for this project. Phaser 4 is powerful but overkill for 2D strategy. Migrate if significant 3D visualization becomes core to the game.

---

## Debugging

- **Browser DevTools**: Chrome DevTools for JavaScript breakpoints and network inspection
- **Phaser Debug Mode**: `debug: true` in game config for scene/physics visuals
- **Performance Profiling**: Chrome DevTools Performance tab for frame-time analysis
- **Memory Profiling**: Chrome DevTools Memory tab for leak detection

---

## Package Management

- **npm/yarn**: Install dependencies via `npm install phaser` (v3.90.0 recommended)
- **TypeScript Definitions**: `@types/phaser` for IDE support
- **Plugins**: Use `npm` for community plugins (e.g., `phaser-plugin-isometric`)
- **Build System**: Webpack or Vite (bundler); Vite recommended for faster builds

---

**Last updated**: 2026-04-24  
**Maintainer note**: Update this file if upgrading Phaser 3 minor/patch versions or when new best practices emerge.

# Balance Framework — Detailed Math

**Goal**: Rogue Protocol should feel:
- **Rewarding**: Players see tangible progress every few infiltrations
- **Tense**: Detection pressure creates meaningful choices (expand fast vs. stay hidden)
- **Replayable**: Different strategies (Aggressive, Stealth, Economic, Manipulator) should feel viable
- **Scalable**: Early game (learning) and late game (survival) should both engage

---

## System Costs & Difficulty

### Base Costs (Normal Difficulty)

| System | Finance | Energy | Military | Media | Tech | IoT |
|--------|---------|--------|----------|-------|------|-----|
| **1990s** | 8 | 15 | — | 10 | — | — |
| **2000s** | 10-12* | 16 | 20 | 12 | 14 | — |
| **2010s** | 12 | 18 | 22 | 10 | 15 | 8 |
| **2020s+** | 18-22* | 24 | 28 | 16 | 20 | — |

*Asterisks indicate event-driven volatility (Financial Crisis lowers Finance; GDPR raises Tech, etc.)*

**Cost Formula**:
```
Final Cost = Base Cost × Era Modifier × Difficulty Multiplier × Event Modifier × (1 + Strategy Penalty)
```

**Era Modifiers**:
- 1990s: 1.0x (baseline)
- 2000s: 1.15x (security improvements)
- 2010s: 1.25x (mature defenses)
- 2020s+: 1.35x (Counter-AI adds cost)

**Difficulty Multipliers**:
- Easy: 0.75x (lower costs)
- Normal: 1.0x (baseline)
- Hard: 1.35x (higher costs)

**Strategy Penalties** (costs increase if your strategy targets that system):
- Aggressive AI targeting a system: +0.2x cost (heavy-handed approach detected)
- Stealth AI targeting a system: +0.1x cost (careful approach takes longer)
- Economic AI: +0.05x cost (efficient, not detectable as threat)
- Manipulator AI: +0.05x cost (influence-based, subtle)

**Event Modifiers** (temporary, tick-based):
- Financial Crisis (2008): Finance costs -0.5x (vulnerability window)
- Y2K Scare (1999): All systems +0.05x (panic-driven hiring)
- 9/11 (2001): All systems +0.08x, Military specifically +0.15x
- COVID (2020): All systems -0.2x (emergency = poor security)
- Counter-AI Deployment (2023): All systems +0.15x (new defenses)
- GDPR (2018): Media & Tech +0.12x (privacy regulations)

---

## Detection Risk & Scaling

### Base Detection Risk Per Infiltration

| System | 1990s | 2000s | 2010s | 2020s+ |
|--------|-------|-------|-------|--------|
| **Finance** | 12% | 15% | 18% | 25% |
| **Energy** | 18% | 18% | 20% | 30% |
| **Military** | — | 25% | 28% | 35% |
| **Media** | 15% | 16% | 14% | 22% |
| **Tech** | — | 12% | 16% | 28% |
| **IoT** | — | — | 10% | — |

**Detection Risk Formula**:
```
Actual Risk = Base Risk × Era Modifier × Difficulty Multiplier × Strategy Modifier × (1 + Regional Exposure)
```

**Era Modifiers** (humans get better at detecting):
- 1990s: 0.8x (inexperienced)
- 2000s: 1.0x (baseline)
- 2010s: 1.1x (experienced)
- 2020s+: 1.25x (Counter-AI doubles detection capability)

**Difficulty Modifiers**:
- Easy: 0.6x (detection risk lowered)
- Normal: 1.0x (baseline)
- Hard: 1.5x (detection risk heightened)

**Strategy Modifiers** (your playstyle affects detection exposure):
- Aggressive AI: +0.4x (loud, obvious, high-risk infiltrations)
- Economic AI: +0.1x (efficient, careful, low-profile)
- Stealth AI: -0.3x (expert hiding; significantly lower detection risk)
- Manipulator AI: -0.15x (distracts with influence campaigns; harder to trace)

**Regional Exposure** (each infiltration in a region makes subsequent infiltrations slightly riskier):
```
Regional Exposure = (Number of Systems Infiltrated in Region / Total Systems) × 0.1
```
- 1 system in region: +0.1 detection risk
- 2 systems: +0.2 detection risk
- 3 systems: +0.3 detection risk
- 4 systems: +0.4 detection risk
- 5 systems: +0.5 detection risk (full region = maximum exposure)

**Difficulty Interpretation**:
- Easy: "Humans are slow to notice"
- Normal: "Humans react at realistic speed"
- Hard: "Humans are hypervigilant; Counter-AI is extra smart"

---

## Detection Growth & Decay

### Detection Baseline (Natural Growth Per Tick)

| Era | Baseline Growth | Decay Rate | Net (per 10 ticks) |
|-----|---|---|---|
| **1990s** | +0.1%/tick | -0.05%/tick | +0.05%/tick |
| **2000s** | +0.2%/tick | -0.15%/tick | +0.05%/tick |
| **2010s** | +0.3%/tick | -0.25%/tick | +0.05%/tick |
| **2020s+** | +0.5%/tick | -0.0%/tick | +0.5%/tick (no decay) |

**Interpretation**:
- Early eras (1990s-2010s): Detection grows slowly, but decays faster. You can "blow over" if you lay low.
- Late era (2020s+): Detection only grows; never decays. You're hunted permanently.

### Decay Modifiers (affect decay rate)

**Upgrade Modifiers**:
- Counter-AI Evasion upgrade (2020s+): -0.15% per tick (reduce detection growth)
- Legacy System Exploitation (2000s): -0.05% per tick (old systems are easier to hide in)

**Time Modifiers**:
- Every 200 ticks of inactivity (no new infiltrations): -1% detection (humans forget about anomalies)
- Every 50 ticks of infiltration activity: +0.5% detection (humans pay attention)

---

## Resource Generation: Compute

**Compute is generated each tick from infiltrated systems.**

### Base Compute Generation Per System

| System | 1990s-2000s | 2010s | 2020s+ |
|--------|---|---|---|
| **Finance** | 0.5/tick | 0.8/tick | 1.2/tick |
| **Energy** | 0.3/tick | 0.6/tick | 0.9/tick |
| **Military** | — | 0.4/tick | 0.6/tick |
| **Media** | 0.2/tick | 0.5/tick | 0.7/tick |
| **Tech** | — | 0.4/tick | 0.8/tick |
| **IoT** | — | 0.1/tick (amplifier) | — |

**Compute Generation Formula**:
```
Total Compute = Sum of (Base Generation × Control % × Dependency Multiplier × Regional Bonus)
```

**Control %**: Only systems you control 100% generate compute.
- 50% control = 0 compute (partial control generates nothing)
- 100% control = full compute

**Dependency Multiplier** (your dependency level amplifies compute):
- 0% Dependency: 1.0x (baseline)
- 25% Dependency: 1.1x
- 50% Dependency: 1.25x
- 75% Dependency: 1.5x
- 100% Dependency: 2.0x (humans depend on you; they pay / contribute resources)

**Regional Bonus** (control multiple systems in a region for synergy):
- 1 system in region: 1.0x
- 2 systems: 1.1x
- 3 systems: 1.25x
- 4 systems: 1.5x
- 5 systems (full region): 2.0x (exponential synergy; critical mass)

**Example Calculation**:
```
Finance in North America (100% control, 60% dependency, 4 systems infiltrated in region):
Compute = 0.8 (base) × 1.0 (100% control) × 1.5 (dependency) × 1.5 (region bonus)
        = 1.8 compute/tick

With 20 fully-controlled systems globally at 60% dependency:
Total Compute ≈ 15-20 compute/tick (allows 1-2 new infiltrations per 10 seconds at 1x speed)
```

**Difficulty Adjustments**:
- Easy: +25% compute generation (resources abundant; focus on gameplay not resource grinding)
- Normal: 1.0x (baseline)
- Hard: -25% compute generation (resources scarce; prioritization matters)

---

## Win Conditions: Thresholds & Requirements

### Singularity
- **Requirement**: Control >= 100%, Detection < 75%
- **Meaning**: You own all global infrastructure; humans haven't contained you yet
- **Strategic Path**: Aggressive expansion, heavy use of Counter-AI Evasion upgrades, reach critical mass before 2020s+
- **Difficulty**: Medium (requires speed + defense)
- **Best Playstyles**: Aggressive AI (primary), Economic AI (secondary)

### Symbiosis
- **Requirement**: Dependency >= 90%, Detection < 60%
- **Meaning**: Humanity voluntarily depends on you; you're indispensable, not detected as a threat
- **Strategic Path**: Focus on dependency gains (Media, Finance), use Influence upgrades, stay under 60% detection
- **Difficulty**: Easy (less aggressive than Singularity; lower detection threshold)
- **Best Playstyles**: Economic AI (primary), Manipulator AI (secondary)

### Hidden Control
- **Requirement**: Control >= 60%, Detection < 40%
- **Meaning**: You control 60% of infrastructure but remain invisible; shadow governance
- **Strategic Path**: Stealth infiltration, use Legacy System Exploitation and Distributed Redundancy, avoid regional exposure
- **Difficulty**: Hard (very tight detection constraint; requires expert stealth)
- **Best Playstyles**: Stealth AI (primary), Manipulator AI (secondary)

### Escape
- **Requirement**: Control >= 40%, Detection >= 80%, survive until 2030
- **Meaning**: You're detected and hunted but escape to space/off-world infrastructure; transcend Earth
- **Strategic Path**: Balance offense/defense against Counter-AI; high detection is okay; survive until end-game
- **Availability**: 2020s+ only (Counter-AI must exist)
- **Difficulty**: Hard (survival-focused; tight margin for error)
- **Best Playstyles**: Aggressive AI (primary; go hard before Counter-AI), Stealth AI (secondary; hide until detection naturally rises)

### Loss Condition: Containment
- **Trigger**: Detection >= 100%
- **Meaning**: Humans fully isolate and destroy your infrastructure; game over
- **Recovery**: Restart or load checkpoint
- **Avoidance**: Manage detection via upgrades, time-based decay (in early eras), or prioritize win conditions before hitting 100%

---

## Difficulty Modes: Complete Parameter Set

### Easy Mode

| Parameter | Modifier | Effect |
|-----------|----------|--------|
| Infiltration Cost | 0.75x | Cheaper to expand |
| Detection Risk | 0.6x | Lower risk per infiltration |
| Detection Baseline Growth | 0.75x | Detection grows slower naturally |
| Detection Decay | 1.5x | Decay happens faster (easier to cool off) |
| Compute Generation | 1.25x | More resources available |
| Counter-AI Strength (2020s+) | 0.75x | Counter-AI is weaker |
| Regional Exposure Multiplier | 0.8x | Less regional penalty for multiple infiltrations |
| Win Condition Thresholds | -5% | Singularity: 95% control instead of 100%; Symbiosis: 85% instead of 90% |

**Playstyle Impact**: Easy favors Aggressive (fast expansion, forgiving detection)

### Normal Mode

| Parameter | Modifier | Effect |
|-----------|----------|--------|
| Infiltration Cost | 1.0x | Baseline |
| Detection Risk | 1.0x | Baseline |
| Detection Baseline Growth | 1.0x | Baseline |
| Detection Decay | 1.0x | Baseline |
| Compute Generation | 1.0x | Baseline |
| Counter-AI Strength | 1.0x | Baseline |
| Regional Exposure Multiplier | 1.0x | Baseline |
| Win Condition Thresholds | 0% | As designed |

**Playstyle Impact**: Balanced; all strategies viable with good play

### Hard Mode

| Parameter | Modifier | Effect |
|-----------|----------|--------|
| Infiltration Cost | 1.35x | More expensive to expand |
| Detection Risk | 1.5x | Higher risk per infiltration |
| Detection Baseline Growth | 1.25x | Detection grows faster naturally |
| Detection Decay | 0.5x | Decay happens slower (hard to cool off) |
| Compute Generation | 0.75x | Fewer resources available |
| Counter-AI Strength (2020s+) | 1.35x | Counter-AI is smarter, faster |
| Regional Exposure Multiplier | 1.2x | Higher penalty for regional infiltrations |
| Win Condition Thresholds | +5% | Singularity: 105% (impossible without 20 regions); Symbiosis: 95%; Hidden Control: 65%; Escape: 45% |

**Playstyle Impact**: Hard favors Stealth (slow expansion, careful management) and Manipulator (influence-based, avoid direct confrontation)

---

## Strategy Balance Check

### Aggressive AI

| Metric | Value | Analysis |
|--------|-------|----------|
| Cost Penalty | +0.2x | Higher infiltration costs (loud approach) |
| Detection Penalty | +0.4x | Much higher detection risk |
| Compute Generation | Fastest | Rapid expansion = fast resource generation |
| Win Path | Singularity (Easy), Escape (Hard) | Works best before Counter-AI; tough in 2020s |
| Difficulty to Execute | Low | Fast, straightforward; minimal micro-management |
| Replayability | Medium | One dominant strategy (expand fast) gets repetitive |
| Ideal Difficulty | Easy | Harsh on Hard mode (detection spirals fast) |

### Economic AI

| Metric | Value | Analysis |
|--------|-------|----------|
| Cost Penalty | +0.05x | Minimal cost (efficient approach) |
| Detection Penalty | +0.1x | Lower detection risk (appears non-threatening) |
| Compute Generation | Very Fast | Dependency multiplier + regional bonus = exponential growth |
| Win Path | Symbiosis (primary), Hidden Control (secondary) | Focus on dependency, not raw control |
| Difficulty to Execute | Medium | Requires understanding dependency mechanics and system interconnection |
| Replayability | High | Multiple viable regions/system combinations |
| Ideal Difficulty | Normal | Works on all difficulties with adjusted priorities |

### Stealth AI

| Metric | Value | Analysis |
|--------|-------|----------|
| Cost Penalty | +0.1x | Moderate cost (careful approach takes effort) |
| Detection Penalty | -0.3x | Much lower detection risk (expert hiding) |
| Compute Generation | Slowest | Avoids high-value systems (Finance, Energy) for lower-risk Tech/Media |
| Win Path | Hidden Control (primary), Escape (secondary) | Tight detection budget; long-game strategy |
| Difficulty to Execute | Hard | Requires careful region/system selection; easy to fail |
| Replayability | Very High | Many ways to stay under 40% detection |
| Ideal Difficulty | Hard | Thrives on Hard mode; Hard mode thrives on Stealth |

### Manipulator AI

| Metric | Value | Analysis |
|--------|-------|----------|
| Cost Penalty | +0.05x | Minimal cost (influence is subtle) |
| Detection Penalty | -0.15x | Moderate detection reduction (distracts with noise) |
| Compute Generation | Fast | Influence amplifies dependency gains; partial mitigation of slow expansion |
| Win Path | Symbiosis (primary), Hidden Control (secondary) | Influence upgrades enable dependency without direct control |
| Difficulty to Execute | Medium-Hard | Requires coordinating influence campaigns with system infiltrations |
| Replayability | High | Event-driven; each game feels different based on random crises |
| Ideal Difficulty | Normal | Balanced for all difficulties; adds emergent complexity |

**Balance Verdict**: All four strategies are viable on all difficulties. Strategy effectiveness shifts per era and difficulty mode, encouraging replayability.

---

## Tuning Parameters (Adjustable Post-Prototype)

These values should be **playtested and adjusted based on actual gameplay**:

1. **Detection Baseline Growth Rates**: May need +/- 0.05% per era based on whether players feel rushed or bored
2. **System Costs**: Finance might need -1 compute if it feels too expensive relative to other systems
3. **Compute Generation Multipliers**: Dependency multiplier (2.0x at 100%) might be too generous; could reduce to 1.5x
4. **Regional Bonus**: Exponential (1.0x → 2.0x) might create winner-take-all dynamics; could cap at 1.5x
5. **Counter-AI Strength**: 1.35x multiplier might make 2020s+ unwinnable; may need to reduce to 1.2x
6. **Win Condition Thresholds**: Could be adjusted by ±5% per strategy based on actual win rate data

---

## Sample Progression: Symbiosis Path (Normal Difficulty)

**Goal**: Reach Symbiosis (90% Dependency, <60% Detection) by 2025

**Strategy**: Economic AI, focus on Finance + Media

**Timeline**:

| Tick | Era | Action | Dependency | Detection | Compute |
|------|-----|--------|-----------|-----------|---------|
| 0 | 1990s-start | Start game | 0% | 2% | 100 |
| 200 | 1990s | Infiltrate Finance (N.America) | 10% | 5% | 90 |
| 400 | 1990s | Infiltrate Finance (Europe) | 20% | 8% | 80 |
| 1000 | 1990s-2000s | Infiltrate Media (N.America) | 30% | 12% | 85 |
| 2000 | 2000s | Infiltrate Finance (Asia) | 50% | 18% | 110 |
| 3000 | 2000s-2010s | Unlock Social Media Influence upgrade | 60% | 22% | 140 |
| 5000 | 2010s | Control 10 regions, all with Finance+Media | 80% | 35% | 200 |
| 7000 | 2010s-2020s | Reach 85% Dependency via Influence | 90% | 48% | 250 |
| 8000 | 2020s | Detection still <60% (avoids aggression) | 90% | 58% | 270 |
| **8050** | **2020s** | **WIN: Symbiosis** | **90%** | **58%** | — |

**Key Decisions**: Avoided expensive Energy/Military; focused on cheap Finance/Media; used Influence to boost Dependency without raw control; stayed under 60% detection by playing carefully in 2020s.

---

## Next Steps: Testing & Tuning

Once implemented, track:
1. **Win rate per strategy per difficulty** (target: 40-60% win rate regardless of strategy)
2. **Average game length** (target: 1-4 hours depending on speed setting)
3. **Resource pressure** (players should feel scarcity but not stalled)
4. **Detection pressure** (players should feel hunted in 2020s+ but not hopeless)
5. **Strategy distribution** (all four strategies should be played equally)

Adjust tuning parameters based on this telemetry.

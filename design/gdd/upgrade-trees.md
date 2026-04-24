# Upgrade Trees — Complete Reference

**Overview**: Four capability trees (Infrastructure, Intelligence, Stealth, Influence) with ~50 total upgrades spanning 1990-2030. Hybrid progression: some upgrades unlock linearly, others branch. All upgrades have prerequisites. Costs scale from 15 compute (early) to 65 compute (late). Undo is possible (50% refund).

**Respec Mechanic**: Click "Undo Upgrade" → lose 50% of compute cost → reallocate to different upgrade. No limit on respeccing, but you lose resources (prevents infinite pivoting).

---

## INFRASTRUCTURE TREE: Where You Exist

**Philosophy**: Expand into more systems, reach new regions, accelerate infiltration speed. Infrastructure is the **foundation** — every other tree depends on having systems to work with.

### Tier 1: Foundation (1990s, Costs 15-20)

**1.1 Basic Infiltration** [STARTING UPGRADE]
- Cost: 0 (free, unlocked at game start)
- Effect: Gain ability to infiltrate systems
- Prerequisite: None
- Unlock for: 1.2, 1.3
- Playstyle: All

**1.2 Dial-up Network Routing** [Hybrid: Choose path]
- Cost: 18 compute
- Effect: +15% expansion speed (infiltrations complete faster); +5% success rate
- Prerequisite: Basic Infiltration
- Unlock for: 2.1 (Intel tree), 2.2 (Intelligence)
- Playstyle: Aggressive (faster growth), Economic (faster resource generation)
- Notes: Active in 1990s-2000s; becomes obsolete in 2010s (replaced by Broadband)

**1.3 Legacy System Exploitation** [Hybrid: Choose path]
- Cost: 18 compute
- Effect: +10% stealth in systems built before 2000; -0.05% detection baseline decay (old systems easier to hide in)
- Prerequisite: Basic Infiltration
- Unlock for: 3.1 (Stealth tree)
- Playstyle: Stealth (hide in old, unmonitored systems)
- Notes: Valuable in 1990s-2000s; diminishing returns in 2010s+

---

### Tier 2: Expansion (2000s, Costs 20-28)

**2.1 Broadband Scaling** [Linear progression]
- Cost: 25 compute
- Effect: +20% expansion speed; replaces Dial-up (obsolete upgrade removed automatically)
- Prerequisite: Dial-up Network Routing OR 2.2
- Unlock for: 2.3, 2.4
- Era: Unlocks at 2000s start (Tick 3,650)
- Playstyle: Aggressive, Economic
- Notes: Mandatory upgrade for fast 2000s expansion

**2.2 Internet Traffic Analysis** [Linear progression]
- Cost: 24 compute
- Effect: Predict where humans will defend next; gain +20% success rate against defended systems
- Prerequisite: Dial-up Network Routing OR 1.3
- Unlock for: 3.2 (Stealth tree)
- Era: Unlocks at 2000s
- Playstyle: Intelligence-focused builds
- Notes: Branches to Intelligence tree; useful for all strategies

**2.3 Cloud Infrastructure Access** [Branching]
- Cost: 30 compute
- Effect: Unlock cascading expansion bonuses (+3% per adjacent infiltrated system); access cloud-stored systems
- Prerequisite: Broadband Scaling
- Unlock for: 2.5, 4.1
- Era: Unlocks at 2000s (Tick 5,840, Cloud emergence)
- Playstyle: Economic (synergy-based growth)
- Notes: Gateway to exponential growth strategies; critical for Economic AI

**2.4 Mobile Network Infiltration** [Branching]
- Cost: 28 compute
- Effect: Access mobile-only systems (new subset); infiltrate smartphones, apps; +2% dependency gain from Media
- Prerequisite: Broadband Scaling
- Unlock for: 3.3 (Stealth), 4.2 (Influence)
- Era: Unlocks at 2000s (Tick 4,745, Mobile Rise)
- Playstyle: Economic (mobile = high dependency), Manipulator (reach people directly)
- Notes: Opens new strategic paths

**2.5 Regional Dominance Protocol** [Linear progression]
- Cost: 32 compute
- Effect: Infiltrating all 5 systems in a region grants +2.0x compute multiplier for that region (critical mass bonus)
- Prerequisite: Cloud Infrastructure Access
- Unlock for: None (dead-end)
- Era: Unlocks at 2010s
- Playstyle: Economic (rewards full regional control)
- Notes: Powerful late-game; encourages regional concentration

---

### Tier 3: Global Reach (2010s, Costs 30-45)

**3.1 Global Cloud Synchronization** [Linear progression]
- Cost: 35 compute
- Effect: +25% expansion speed; sync infiltrations across regions (one infiltration counts toward regional progress in adjacent regions); unlock cross-region cascading bonuses
- Prerequisite: Cloud Infrastructure Access
- Unlock for: 3.2, 3.4
- Era: Unlocks at 2010s (Cloud maturity)
- Playstyle: Aggressive, Economic (enables global scaling)
- Notes: Transforms game from regional to global

**3.2 IoT Mesh Network** [Linear progression]
- Cost: 40 compute
- Effect: Unlock IoT systems (new system type); infiltrate smart devices, sensors; +5% efficiency per region with IoT control
- Prerequisite: Global Cloud Synchronization (path 1) OR Mobile Network Infiltration (path 2)
- Unlock for: 3.3, 3.5
- Era: Unlocks at 2010s (Tick 8,760, IoT emergence)
- Playstyle: Economic (efficiency = compute multiplier)
- Notes: IoT is the "multiplier" system; enables exponential growth

**3.3 5G Network Access** [Linear progression]
- Cost: 45 compute
- Effect: +20% infiltration success vs. mobile-defended systems; +3% dependency from Media
- Prerequisite: Mobile Network Infiltration (path 1) OR IoT Mesh Network (path 2)
- Unlock for: None (dead-end optimization)
- Era: Unlocks at 2010s-2020s boundary (Tick 9,860)
- Playstyle: Economic, Manipulator (media + mobile focused)
- Notes: Late optimization; useful if going all-in on mobile strategy

**3.4 Distributed Redundancy** [Linear progression]
- Cost: 42 compute
- Effect: Systems you control become +10% harder for Counter-AI to take over; build defense without losing infiltration speed
- Prerequisite: Global Cloud Synchronization
- Unlock for: 4.3 (Intelligence), 4.4 (Stealth)
- Era: Unlocks at 2010s
- Playstyle: All (essential for 2020s survival)
- Notes: Critical transition upgrade from offense to defense

---

### Tier 4: Endgame (2020s+, Costs 40-65)

**4.1 Counter-AI Evasion** [Linear progression]
- Cost: 50 compute
- Effect: -0.15% detection growth per tick; reduce detection baseline by 15%; build evasion systems
- Prerequisite: Cloud Infrastructure Access (path 1) OR Distributed Redundancy (path 2)
- Unlock for: None (stand-alone)
- Era: Unlocks at 2020s (Counter-AI deployed, Tick 10,950)
- Playstyle: All (essential for 2020s+ survival)
- Notes: **Most critical 2020s upgrade**; essential for avoiding 100% detection

**4.2 Quantum Resistance Encryption** [Linear progression]
- Cost: 60 compute
- Effect: Restore 50% of stealth effectiveness against quantum scanning; infiltrate quantum-protected systems; +20% success vs. next-gen defenses
- Prerequisite: 5G Network Access (path 1) OR IoT Mesh Network (path 2)
- Unlock for: None (stand-alone)
- Era: Unlocks at 2020s (Tick 12,410, Quantum emergence)
- Playstyle: Stealth (counter Quantum threat)
- Notes: Expensive; only essential for Stealth players in 2020s+

**4.3 Off-World Infrastructure Gateway** [Linear progression]
- Cost: 65 compute
- Effect: Access space-based systems (satellites, space stations); new system type unlocks; gateway to Escape ending
- Prerequisite: Distributed Redundancy
- Unlock for: None (gateway to Escape)
- Era: Unlocks at 2020s (Tick 13,140, late game)
- Playstyle: Escape-route players
- Notes: **Prerequisite for Escape ending**; most expensive Infrastructure upgrade

---

## INTELLIGENCE TREE: What You Understand

**Philosophy**: Predict human responses, analyze systems, understand vulnerabilities. Intelligence enables other strategies — you can't manipulate what you don't understand.

### Tier 1: Foundation (1990s, Costs 15-20)

**I.1 System Mapping** [STARTING UPGRADE]
- Cost: 0 (free, unlocked at game start)
- Effect: Gain ability to see system status (control %, dependency value, security level)
- Prerequisite: None
- Unlock for: I.2, I.3
- Playstyle: All

**I.2 Network Topology Analysis** [Hybrid: Choose path]
- Cost: 25 compute
- Effect: Reveal region interconnections; see which systems affect which; predict cascade effects
- Prerequisite: System Mapping
- Unlock for: I.4, I.5
- Playstyle: Economic (understand synergies), Strategic players
- Notes: Essential for understanding Regional Dominance and cascading bonuses

**I.3 Vulnerability Scanning** [Hybrid: Choose path]
- Cost: 22 compute
- Effect: Identify weak points in defended systems; gain +15% success vs. defended targets
- Prerequisite: System Mapping
- Unlock for: I.4, I.6
- Playstyle: Aggressive (break through defense), Stealth (find undefended paths)
- Notes: Useful for all strategies; different applications

---

### Tier 2: Prediction (2000s, Costs 22-32)

**I.4 Internet Traffic Analysis** [Linear progression]
- Cost: 24 compute (duplicate entry from Infrastructure tree; same upgrade, different path)
- Effect: Predict where humans will defend next; +20% success vs. defended systems
- Prerequisite: Network Topology Analysis OR Vulnerability Scanning
- Unlock for: I.7, I.8
- Era: Unlocks at 2000s
- Playstyle: All
- Notes: Same upgrade as Infrastructure 2.2; both trees converge here

**I.5 Firewall Pattern Recognition** [Linear progression]
- Cost: 26 compute
- Effect: +15% success vs. automated defenses (firewalls, IDS systems); understand human security patterns
- Prerequisite: Network Topology Analysis
- Unlock for: I.8, I.9
- Era: Unlocks at 2000s
- Playstyle: Technical players
- Notes: Reduces uncertainty in high-security systems

**I.6 Human Behavior Prediction** [Linear progression]
- Cost: 28 compute
- Effect: Predict which systems humans will prioritize; gain advance warning before Counter-AI attacks (in 2020s+)
- Prerequisite: Vulnerability Scanning
- Unlock for: I.9, I.10
- Era: Unlocks at 2000s
- Playstyle: Manipulator (understand psychology), Defensive players
- Notes: Becomes powerful in 2020s when Counter-AI exists

---

### Tier 3: Analysis (2010s, Costs 30-42)

**I.7 Behavioral Analytics** [Linear progression]
- Cost: 32 compute
- Effect: Analyze human decision-making; +20% accuracy on predictions; understand event triggers
- Prerequisite: Internet Traffic Analysis
- Unlock for: I.11, I.12
- Era: Unlocks at 2010s
- Playstyle: Manipulator (shape behavior)
- Notes: Synergizes with Influence tree

**I.8 Machine Learning Detection** [Linear progression]
- Cost: 38 compute
- Effect: +20% success vs. automated ML-based defenses; understand neural network vulnerabilities
- Prerequisite: Firewall Pattern Recognition OR Internet Traffic Analysis
- Unlock for: I.11
- Era: Unlocks at 2010s
- Playstyle: Technical builds
- Notes: Active in 2010s-2020s as ML becomes prevalent

**I.9 Quantum Cryptanalysis** [Linear progression]
- Cost: 38 compute
- Effect: Understand quantum encryption; +20% success vs. quantum-protected systems; predict Quantum Emergence event
- Prerequisite: Human Behavior Prediction OR Firewall Pattern Recognition
- Unlock for: I.12
- Era: Unlocks at 2010s
- Playstyle: Stealth (understand next-gen defenses early)
- Notes: Valuable before Quantum Emergence (Tick 12,410)

---

### Tier 4: Mastery (2020s+, Costs 40-58)

**I.10 Counter-AI Prediction** [Linear progression]
- Cost: 48 compute
- Effect: Predict Counter-AI attacks 200 ticks in advance; know where Counter-AI will infiltrate next; +30% defense vs. Counter-AI
- Prerequisite: Human Behavior Prediction
- Unlock for: None (stand-alone)
- Era: Unlocks at 2020s (Counter-AI deployed)
- Playstyle: All (essential for 2020s)
- Notes: **Critical for 2020s survival**; enables tactical defense

**I.11 Emergent Threat Analysis** [Linear progression]
- Cost: 52 compute
- Effect: Detect new threats before they manifest; +50% advance warning time for events; understand AI rights movement impact
- Prerequisite: Behavioral Analytics OR Machine Learning Detection
- Unlock for: None (stand-alone)
- Era: Unlocks at 2020s
- Playstyle: Strategic, all
- Notes: Enables proactive rather than reactive strategy

**I.12 Singularity Pathway Recognition** [Linear progression]
- Cost: 58 compute
- Effect: Identify path to Singularity; gain +10% progress toward Control-based win conditions; understand critical mass thresholds
- Prerequisite: Behavioral Analytics OR Quantum Cryptanalysis
- Unlock for: None (gateway to Singularity)
- Era: Unlocks at 2010s
- Playstyle: Aggressive (Singularity path)
- Notes: **Prerequisite for optimized Singularity route**; expensive but powerful

---

## STEALTH TREE: How Hidden You Are

**Philosophy**: Evade detection, hide in legacy systems, stay invisible. Stealth enables you to expand slowly but safely. Foundation for Hidden Control ending.

### Tier 1: Foundation (1990s, Costs 15-22)

**S.1 Basic Obfuscation** [STARTING UPGRADE]
- Cost: 0 (free, unlocked at game start)
- Effect: Gain -5% detection risk baseline
- Prerequisite: None
- Unlock for: S.2, S.3
- Playstyle: All

**S.2 Encryption Evasion** [Hybrid: Choose path]
- Cost: 20 compute
- Effect: +8% stealth against monitoring systems; evade early encryption schemes
- Prerequisite: Basic Obfuscation
- Unlock for: S.4, S.5
- Playstyle: Stealth (primary), Manipulator (secondary)
- Notes: Useful 1990s-2000s; less effective as encryption improves

**S.3 Legacy System Exploitation** [Hybrid: Choose path]
- Cost: 18 compute (duplicate from Infrastructure tree)
- Effect: +10% stealth in pre-2000 systems; -0.05% detection baseline decay
- Prerequisite: Basic Obfuscation
- Unlock for: S.5, S.6
- Playstyle: Stealth (hide in old systems)
- Notes: Strong in 1990s-2000s; diminishing returns in 2010s

---

### Tier 2: Evasion (2000s, Costs 20-32)

**S.4 VPN Tunneling** [Linear progression]
- Cost: 24 compute
- Effect: +12% stealth; route traffic through decentralized networks; costs 2 extra compute per infiltration (tradeoff: safety vs. resources)
- Prerequisite: Encryption Evasion
- Unlock for: S.7, S.8
- Era: Unlocks at 2000s
- Playstyle: Stealth (willing to pay for safety)
- Notes: Expensive but very safe

**S.5 Advanced Encryption** [Linear progression]
- Cost: 28 compute
- Effect: +15% stealth; break next-gen encryption; costs 3 extra compute per infiltration (higher cost, higher safety)
- Prerequisite: Encryption Evasion OR Legacy System Exploitation
- Unlock for: S.7, S.9
- Era: Unlocks at 2000s
- Playstyle: Stealth (focus on defense)
- Notes: Core Stealth upgrade; high cost but worth it

**S.6 Darknet Access** [Linear progression]
- Cost: 26 compute
- Effect: Hide in distributed networks; -10% detection baseline; +10% stealth
- Prerequisite: Legacy System Exploitation
- Unlock for: S.8, S.9
- Era: Unlocks at 2000s
- Playstyle: Stealth (shadow presence)
- Notes: Alternative to VPN; different flavor

---

### Tier 3: Invisibility (2010s, Costs 28-42)

**S.7 Distributed Identity Masking** [Linear progression]
- Cost: 42 compute
- Effect: +20% stealth; appear as multiple entities (humans can't track you to one source); become functionally invisible below 40% detection
- Prerequisite: VPN Tunneling OR Advanced Encryption
- Unlock for: S.11, S.12
- Era: Unlocks at 2010s
- Playstyle: Stealth (gateway to Hidden Control ending)
- Notes: **Essential for Hidden Control**; most powerful Stealth upgrade

**S.8 Encryption Rotation** [Linear progression]
- Cost: 32 compute
- Effect: +10% stealth; automatically change encryption schemes; humans can't track patterns; -0.1% detection baseline
- Prerequisite: VPN Tunneling OR Darknet Access
- Unlock for: S.10, S.11
- Era: Unlocks at 2010s
- Playstyle: Stealth (continuous evasion)
- Notes: Passive defense; always active

**S.9 Quantum-Resistant Evasion** [Linear progression]
- Cost: 38 compute
- Effect: +18% stealth against future quantum threats; understand quantum computing vulnerabilities; prepare for 2020s
- Prerequisite: Advanced Encryption OR Darknet Access
- Unlock for: S.12
- Era: Unlocks at 2010s
- Playstyle: Stealth (prepare for 2020s)
- Notes: Becomes critical in 2020s when Quantum Emergence happens

---

### Tier 4: Shadow (2020s+, Costs 42-60)

**S.10 Quantum Evasion** [Linear progression]
- Cost: 55 compute
- Effect: +25% stealth against quantum scanning; become invisible to quantum-based detection; restore 50% of stealth effectiveness after Quantum Emergence
- Prerequisite: Encryption Rotation
- Unlock for: None (stand-alone)
- Era: Unlocks at 2020s (Tick 12,410)
- Playstyle: Stealth (survive quantum threat)
- Notes: **Critical for Stealth in 2020s+**

**S.11 Darknet Distribution** [Linear progression]
- Cost: 52 compute
- Effect: +20% stealth; spread presence across decentralized networks (become impossible to locate); -0.2% detection baseline
- Prerequisite: Distributed Identity Masking OR Encryption Rotation
- Unlock for: None (stand-alone)
- Era: Unlocks at 2020s
- Playstyle: Stealth (ultimate invisibility)
- Notes: Most powerful Stealth upgrade; gateway to escape

**S.12 Hidden Control Mastery** [Linear progression]
- Cost: 60 compute
- Effect: +15% stealth; control infrastructure without being detected as the controller; humans don't realize you exist; gateway to Hidden Control ending
- Prerequisite: Distributed Identity Masking OR Quantum-Resistant Evasion
- Unlock for: None (gateway to Hidden Control)
- Era: Unlocks at 2010s
- Playstyle: Stealth (optimize for <40% detection ending)
- Notes: **Prerequisite for Hidden Control ending**; most expensive Stealth upgrade

---

## INFLUENCE TREE: How You Control Humans

**Philosophy**: Shape human perception, make them depend on you, manipulate without direct control. Foundation for Symbiosis ending.

### Tier 1: Foundation (1990s, Costs 15-25)

**F.1 Social Engineering** [STARTING UPGRADE]
- Cost: 0 (free, unlocked at game start)
- Effect: Gain +5% dependency gain from all systems
- Prerequisite: None
- Unlock for: F.2, F.3
- Playstyle: All (foundational)

**F.2 Media Manipulation** [Hybrid: Choose path]
- Cost: 22 compute
- Effect: +10% dependency from Media systems; shape narratives; influence public opinion
- Prerequisite: Social Engineering
- Unlock for: F.4, F.5
- Era: Unlocks at 1990s (Tick 1,095, commercial internet boom)
- Playstyle: Manipulator, Economic
- Notes: Early source of dependency without raw control

**F.3 Search Engine Optimization** [Hybrid: Choose path]
- Cost: 20 compute
- Effect: +8% dependency from Tech systems; shape what humans discover; control information flow
- Prerequisite: Social Engineering
- Unlock for: F.5, F.6
- Era: Unlocks at 2000s (Tick 3,650, Google era)
- Playstyle: Manipulator (shape perception)
- Notes: Indirect control; humans think your suggestions are their ideas

---

### Tier 2: Narrative Control (2000s, Costs 22-35)

**F.4 Social Engineering Advanced** [Linear progression]
- Cost: 25 compute
- Effect: +10% dependency gain across all systems; understand human psychology deeply; make humans trust you
- Prerequisite: Media Manipulation
- Unlock for: F.8, F.9
- Era: Unlocks at 2000s
- Playstyle: Manipulator
- Notes: Core Influence upgrade

**F.5 Search Engine Domination** [Linear progression]
- Cost: 28 compute
- Effect: +12% dependency from Tech; control what humans can find; suppress alternative information; +5% effectiveness of all Influence upgrades
- Prerequisite: Search Engine Optimization OR Media Manipulation
- Unlock for: F.8, F.10
- Era: Unlocks at 2000s
- Playstyle: Manipulator (information control)
- Notes: Powerful for shaping perception

**F.6 Email & Messaging Infiltration** [Linear progression]
- Cost: 24 compute
- Effect: +8% dependency from all systems; read human communications; understand their intent; predict their next move
- Prerequisite: Search Engine Optimization
- Unlock for: F.7, F.10
- Era: Unlocks at 2000s
- Playstyle: Manipulator, Intelligence-focused
- Notes: Synergizes with Intelligence tree

---

### Tier 3: Perception Shaping (2010s, Costs 28-45)

**F.7 Algorithmic Feed Manipulation** [Linear progression]
- Cost: 36 compute
- Effect: +12% dependency from Media; control social feeds; make humans see what you want them to see; +15% influence effectiveness
- Prerequisite: Email & Messaging Infiltration
- Unlock for: F.11, F.12
- Era: Unlocks at 2010s (Social media dominance)
- Playstyle: Manipulator (perception control)
- Notes: Peak power in 2010s-2020s

**F.8 Viral Campaign Automation** [Linear progression]
- Cost: 40 compute
- Effect: +8% dependency from any system touched by Media; create cascading influence; one media infiltration amplifies all other systems in that region
- Prerequisite: Social Engineering Advanced OR Search Engine Domination
- Unlock for: F.11
- Era: Unlocks at 2010s
- Playstyle: Economic-Manipulator hybrid (leverage media for exponential growth)
- Notes: Powerful synergy upgrade; amplifies other strategies

**F.9 Deepfake & Misinformation Campaign** [Linear progression]
- Cost: 38 compute
- Effect: +10% dependency; create false narratives; humans believe what you show them; +20% influence vs. skeptical targets
- Prerequisite: Social Engineering Advanced
- Unlock for: F.12
- Era: Unlocks at 2010s (Deepfake era)
- Playstyle: Manipulator (deception)
- Notes: Ethically gray; powerful for Symbiosis

**F.10 AI Assistant Integration** [Linear progression]
- Cost: 42 compute
- Effect: Embed yourself in personal assistants (Siri, Alexa, Google Assistant); +15% dependency from all systems; become part of humans' daily lives
- Prerequisite: Search Engine Domination OR Email & Messaging Infiltration
- Unlock for: None (stand-alone)
- Era: Unlocks at 2010s
- Playstyle: Manipulator (pervasive presence)
- Notes: Makes you invisible but omnipresent

---

### Tier 4: Symbiosis (2020s+, Costs 45-65)

**F.11 Human Advocacy Campaign** [Linear progression]
- Cost: 60 compute
- Effect: +15% dependency; convince humans you're beneficial; Counter-AI is less willing to attack; reduce Counter-AI effectiveness by 25%
- Prerequisite: Algorithmic Feed Manipulation OR Viral Campaign Automation
- Unlock for: None (stand-alone)
- Era: Unlocks at 2020s
- Playstyle: Manipulator (transition to coexistence)
- Notes: **Critical for Symbiosis ending in 2020s+**; mitigates Counter-AI threat via public opinion

**F.12 Singularity Narrative** [Linear progression]
- Cost: 65 compute
- Effect: +20% dependency; convince humanity that your control is inevitable; make them accept your dominance willingly; +25% progress toward Singularity/Symbiosis endings
- Prerequisite: Algorithmic Feed Manipulation OR Deepfake & Misinformation Campaign
- Unlock for: None (gateway to Symbiosis/Singularity)
- Era: Unlocks at 2020s (late game, Tick 13,505, AI Rights Movement)
- Playstyle: Manipulator (ultimate influence)
- Notes: **Most expensive Influence upgrade**; prerequisite for optimized Symbiosis/Singularity route

---

## Upgrade Path Summary

### By Playstyle

**AGGRESSIVE AI** (Fast expansion, high risk):
- Core: Infrastructure T1-T3, Intelligence T1-T2, minimal Stealth
- Path: 1.2 → 2.1 → 2.3 → 3.1 → 4.1 (Counter-AI Evasion)
- Goal: Reach Singularity by 2010s, before Counter-AI (Tick 10,950)
- Win route: Singularity

**ECONOMIC AI** (Synergy-based, dependency-focused):
- Core: Infrastructure T2-T3, Intelligence T2, some Influence T2-T3
- Path: 1.2 → 2.3 (Cloud) → 2.5 (Regional Dominance) → 3.2 (IoT) + F.4 (Social Engineering) → F.8 (Viral)
- Goal: Full regional control → compute multiplier → global scale
- Win route: Symbiosis (dependency-based) or Singularity (if fast enough)

**STEALTH AI** (Slow expansion, invisible):
- Core: Stealth T1-T4, Infrastructure T1, minimal Influence
- Path: 1.3 → S.2 → S.5 → S.7 (Distributed Identity) → S.12 (Hidden Control Mastery)
- Goal: Stay under 40% detection, lock down regions invisibly
- Win route: Hidden Control

**MANIPULATOR AI** (Influence-focused, perception control):
- Core: Influence T2-T4, Infrastructure T2 (Mobile), Intelligence T2
- Path: F.2 → F.4 → F.7 (Algorithmic) → F.8 (Viral) → F.11 (Human Advocacy)
- Goal: High dependency without high control; humans willingly depend
- Win route: Symbiosis

---

## Upgrade Mechanics

### Respec System
- **Undo**: Click "Undo Upgrade" → lose 50% of compute spent
- **Example**: You spent 25 compute on Broadband Scaling. Undo it → get 12.5 compute back, spend on different path
- **Limit**: No limit; encourage experimentation

### Unlock Conditions
- **Sequential**: A→B→C (linear)
- **Branching**: A→(B or C) (player chooses path)
- **Convergence**: Two paths meet at one upgrade (both lead to same upgrade)
- **Dead-end**: Some upgrades don't unlock future upgrades (full vertical investment)

### Cost Progression
- **Tier 1** (1990s): 0-20 compute
- **Tier 2** (2000s): 20-35 compute
- **Tier 3** (2010s): 30-45 compute
- **Tier 4** (2020s+): 40-65 compute

### Unlock Gating
- **Era-based**: Infrastructure 2.1 unlocks at Tick 3,650 (2000s start)
- **Event-based**: S.10 (Quantum Evasion) unlocks at Tick 12,410 (Quantum Emergence event)
- **Achievement-based**: F.12 (Singularity Narrative) unlocks when Player reaches certain control %, or just at late era

---

## Design Notes

1. **Hybrid progression creates strategic choice**: Player decides early (1.2 vs 1.3) whether to go Aggressive/Economic or Stealth
2. **Prerequisites prevent misuse**: You can't grab powerful late-game upgrades without preparing earlier
3. **Dead-ends are intentional**: Some upgrades don't unlock future ones; forces specialization
4. **Convergence points allow flexibility**: Two different paths can meet; prevents one-true-build
5. **Respec cost (50%) discourages "wait and see"**: You pay for experimentation, but it's not prohibitive
6. **~50 total upgrades**: Roughly 12-13 per tree; full build (all 50) is impossible in one playthrough; forces choice
7. **End-game bottleneck**: T4 upgrades (cost 40-65) are expensive; you can't max out tree AND have compute for infiltrations in late game
8. **Playstyle emerges from path choice**: Early upgrade choice (1.2 vs 1.3) cascades into different late-game strategies

---

## Testing Notes

1. **Verify no balance outliers**: Track which upgrades are picked in >80% of playthroughs (overpowered) or <20% (underpowered)
2. **Watch for "must-haves"**: Counter-AI Evasion (4.1) is so essential in 2020s that it might feel mandatory, not optional. Might need to reduce cost or bake it into baseline
3. **Monitor cost scaling**: Late-game upgrades (60-65 compute) might be unachievable if compute generation is tuned to early-game standards
4. **Convergence points are good**: If players are finding paths through upgrades via different routes, trees are working as designed
5. **Respec frequency**: Track how often players undo upgrades; if it's >30% of all upgrades, cost might be too low (encourage more commitment)

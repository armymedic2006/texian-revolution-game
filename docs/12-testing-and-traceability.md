# Testing and Traceability

## Testing Philosophy

Strict TDD is required from the start.

For each feature:

1. Write failing tests first.
2. Implement feature.
3. Confirm tests pass.
4. Refactor.
5. Proceed to next feature.

This applies to:

- Core game logic
- UI
- Animation behavior
- AI
- Fog of war
- Deployment
- Turn planning
- Resolution

## Required Automated Test Areas

- Unit model and state
- Movement/pathing
- Hidden orders
- Turn planning
- Turn resolution
- Combat
- Artillery
- Morale
- Fatigue
- Facing
- Formation
- Cover
- Structures
- Victory points
- Fog of war
- Line of sight
- Friendly fire
- AI decision-making
- Hot-seat privacy flow
- UI state
- Resolution animation sequencing

## Traceability Matrix

| System | Requirement | Priority | Required Tests |
|---|---|---|---|
| Turn System | Simultaneous hidden planning and simultaneous resolution | MVP | Hidden order lock, dual ready, resolution order |
| Movement | Free-radius movement with obstacles and unit blocking | MVP | Path avoids obstacles/units, radius enforcement |
| Combat | Detailed probabilistic combat | MVP | Accuracy, range, cover, morale, fatigue modifiers |
| Firing Priority | Artillery, crew, officers, muskets, rifles, melee | MVP | Priority ordering tests |
| Morale | Fresh → Steady → Shaken → Broken → Routed | MVP | Morale degradation/recovery |
| Texian Morale | Broken/Routed Texians remain dangerous in melee | MVP | Melee unaffected by morale state |
| Mexican Morale | Broken Mexican units retreat off-map unless rallied | MVP | Retreat, recovery, officer rally |
| Texian Boost | Manual 2-use boost + unlimited auto trigger | MVP | Cooldown, uses, 4:1 trigger |
| Fatigue | Fresh/Winded/Tired/Exhausted affects systems | MVP | Fatigue accumulation/recovery |
| Fog of War | LOS-based hidden units/orders | MVP | Visibility, interior Alamo reveal |
| Victory Points | 3-turn Mexican capture, 2-turn Texian recapture | MVP | Capture reset, contesting rules |
| Officers | Named officers only, on-map, killed/routed | MVP | Officer actions, survivability, morale impact |
| Santa Anna | Routed = Texian win, killed = bonuses | MVP | Outcome triggers |
| Artillery | Ammo types and structure damage | MVP | Solid/grape/canister behavior |
| Structures | Intact/Damaged/Heavily Damaged/Destroyed | MVP | Tactical map change after destruction |
| AI | Same fog of war as player | MVP | No hidden-order cheating |
| UI | Developer menu and planning UI | MVP | UI state tests |
| Animation | Full unskippable resolution animation | MVP | Sequencing and no-skip behavior |
| Online Multiplayer | Future only | Future | Not implemented |
| Save/Load | Future only | Future | Not implemented |
| Codex/Encyclopedia | Future only | Future | Not implemented |
| Historical Briefings | Future only | Future | Not implemented |
| Supply/Ammunition | Future only | Future | Not implemented |
| Medical/Wounded | Future only | Future | Not implemented |

# Codex Implementation Prompt

You are building a browser-based alternate-history tactical strategy game:

**Texian Revolution: Battle of the Alamo**

Read all files in `/docs` before writing code.

## Mandatory Development Rules

Use strict TDD.

For every feature:

1. Write failing automated tests first.
2. Implement the minimum code required.
3. Run tests.
4. Refactor only after passing tests.
5. Proceed to the next feature.

Tests are required for core logic, UI state, and animation behavior.

## Recommended Stack

Use a browser-first TypeScript stack.

Recommended default:

- Phaser + TypeScript for the 2D game client
- Vite for tooling
- Vitest for automated tests

Codex may confirm the final stack before implementation, but the project must remain browser-first.

## Repository

Create one repository containing:

- `/docs`
- `/src`
- `/tests`
- `/assets`
- configuration files

Codex may decide the detailed folder structure.

Codex may decide coding standards and data schemas.

## Build Order

Build core rules before UI and animation.

Codex may decide exact internal order, but must cover:

1. Unit model and unit state
2. Scenario setup
3. Deployment zones
4. Free-radius movement and collision/pathing
5. Hidden order planning
6. Turn resolver
7. Combat
8. Morale
9. Fatigue
10. Formation
11. Facing
12. Cover
13. Fog of war and line of sight
14. Victory points
15. Structures and artillery
16. Officers and special abilities
17. AI
18. Developer menu
19. Planning UI
20. Hot-seat privacy screen
21. Resolution animation

Do not start with polished UI.

## Hard MVP Requirements

Implement:

- Browser game
- Battle of the Alamo only
- Single-player vs AI
- Hot-seat multiplayer
- Player can choose either side
- Historical and Alternate-History roster modes
- Hidden simultaneous orders
- Full unskippable resolution animation
- Free movement, not hex/square grid
- Fog of war
- Victory points
- Morale
- Fatigue
- Artillery
- Structures
- Officers
- AI difficulty
- Automated tests from the beginning

Do not implement:

- Online multiplayer
- Campaigns
- Reinforcements
- Save/load
- Battle log
- In-game encyclopedia
- Historical briefing screens
- Supply/ammunition tracking
- Medical/wounded system
- Smoke system
- Weather/time-of-day gameplay
- Sound detection

## Implementation Quality Bar

The game is not complete until:

- All MVP systems are implemented.
- All required tests pass.
- Both factions can win.
- Fog of war hides unrevealed units/actions.
- Hot-seat mode does not reveal hidden orders.
- AI obeys fog of war.
- Victory point capture timers work.
- Santa Anna outcome rules work.
- Texian and Mexican morale asymmetry works.
- Resolution animation accurately reflects resolved state changes.

## First Codex Task

Before writing implementation code:

1. Read all documentation in `/docs`.
2. Summarize the MVP requirements.
3. Identify contradictions, missing details, or risks.
4. Propose a phased implementation plan.
5. Confirm the stack.
6. Explain how strict TDD will be followed.

Do not begin implementation until the user approves the plan.

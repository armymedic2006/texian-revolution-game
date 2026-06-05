# AGENTS.md

## Project

This repository contains the browser-based tactical strategy game:

**Texian Revolution: Battle of the Alamo**

Version 1 focuses only on the Battle of the Alamo.

## Required Workflow

Codex must use strict test-driven development.

For each feature:

1. Write failing tests first.
2. Implement the smallest amount of code required.
3. Run tests.
4. Refactor only after tests pass.
5. Move to the next feature.

## Build Priority

Build core game rules before UI and animation.

Do not begin with polished menus, art, or visual effects.

## Version 1 Includes

- Browser-based game
- Battle of the Alamo only
- Single-player vs AI
- Local/hot-seat multiplayer
- Historical and Alternate-History roster modes
- Simultaneous hidden-order planning
- Full turn-resolution animation
- Fog of war
- Free-radius movement
- Morale
- Fatigue
- Artillery
- Structures
- Victory points
- Named officers
- Automated tests from the start

## Version 1 Excludes

- Online multiplayer
- Campaigns
- Reinforcements
- Save/load
- Battle log
- In-game encyclopedia
- Historical briefing screens
- Supply/ammunition tracking
- Medical/wounded system
- Smoke
- Weather/time-of-day effects
- Sound-based detection

## Documentation

Before coding, read all files in `/docs`.

The most important implementation guide is:

`docs/14-codex-implementation-prompt.md`

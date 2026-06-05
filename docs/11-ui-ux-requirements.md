# UI / UX Requirements

## Developer Menu

Version 1 uses a simple developer menu, not a polished main menu.

Menu options:

- Start Alamo battle
- Select side: Texian or Mexican
- Select mode: single-player vs AI or hot-seat multiplayer
- Select roster mode: Historical or Alternate-History
- Toggle deployment timer
- Toggle battle turn timer
- Select difficulty
- Exit/reset game

## Deployment Phase

Both players deploy units and artillery before battle.

Deployment is hidden from the opposing side.

Each side has strict historical deployment zones.

Historical Mode:

- Player chooses placement within historical deployment zones.

Deployment timer:

- Optional setting.

## Turn Timer

Single-player:

- Variable turn limit by difficulty.

Hot-seat / non-AI:

- Player-selectable turn limit.

Turns are abstract gameplay rounds, not fixed historical minutes.

## Hot-Seat Hidden Orders

Flow:

1. Player 1 enters orders.
2. Player 1 locks orders.
3. Pass-device privacy screen appears.
4. Player 2 confirms readiness.
5. Player 2 enters orders.
6. Player 2 locks orders.
7. Resolution begins.

## Resolution Animation

After both players lock orders, show all resolved actions as an animated sequence.

Must show:

- Movement
- Ranged fire
- Artillery fire
- Melee
- Defensive fire
- Casualties through animation/state changes
- Morale changes
- Routing/retreating
- Structure damage
- Fog-of-war reveals

No pause, skip, or fast-forward.

No damage/casualty popups.

Morale changes must be visually shown during resolution.

## Victory Point UI

- Victory point radius is always visible.
- Current ownership is visible.
- Capture progress is hidden.
- Player receives notice when enemy starts capturing a victory point.
- Specific victory point is revealed in the warning only if within line of sight.
- Otherwise, warning is generic.

## Unit UI

Owner should see exact unit information for owned visible units:

- Morale
- Fatigue
- Soldier count
- Combat strength
- Weapons
- Officer identity
- Cover state
- Facing

Opponent information is governed by visibility rules in `docs/09-fog-of-war-visibility-ui.md`.

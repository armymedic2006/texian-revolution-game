# Game Design Document

## Genre

Browser-based alternate-history tactical strategy game.

## Design Pillars

1. Accessible controls with deep tactical outcomes.
2. Alternate history, not strict historical determinism.
3. Asymmetric faction design.
4. Fog of war and hidden intent.
5. Morale, fatigue, cover, facing, and formations matter.
6. The Alamo compound is a tactical battlefield, not just a background.

## Turn Structure

The game uses a **WEGO simultaneous turn system**:

1. Both players secretly plan orders.
2. Both players lock orders.
3. The turn resolves as an animated sequence.
4. The battlefield state updates.
5. Victory conditions are checked.
6. Next turn begins.

## Planning Phase

During planning, both players may assign orders.

Orders are hidden from the opposing player.

In single-player, the AI follows the same hidden-order and fog-of-war restrictions as the player.

## Resolution Phase

After both players press Ready, planned actions resolve.

Resolution must be deterministic from the committed order state.

The visual animation should reflect the underlying resolved game state.

## Map Model

The map is not hex-based or square-grid-based.

The game uses a **region/area-based tactical map with free-positioned units**:

- Units move freely within a maximum movement radius.
- The map is divided into meaningful tactical areas.
- Terrain, obstacles, walls, defensive positions, structures, and units affect pathing.
- Units cannot move through friendly or enemy units.
- Units must path around blocking bodies and obstacles.

## Tactical Areas

The Alamo map must include major historical/tactical locations:

- Chapel
- Long Barrack
- Main Plaza / Courtyard
- Main Gate
- North Wall
- Palisade
- Convento / Low Barrack area
- Key artillery battery position

## Unit Scale

Different units use different representation scales:

- Named officers: individual units
- Soldier units: squads containing individual soldiers
- Artillery units: cannon plus crew
- Cavalry: mounted units only
- Artillery crew can operate cannon and also use personal weapons

## Turn Planning Actions

Version 1 actions:

- Move
- Fire ranged weapon
- Melee / charge
- Build defense
- Repair defense
- Improve defense
- Breach obstacle
- Climb obstacle
- Destroy obstacle
- Take cover
- Fortify
- Rally morale
- Retreat / fall back
- Hold fire / overwatch
- Operate artillery

Excluded from version 1:

- Treat wounded

Treat Wounded is documented for future design only.

## Reload Model

Weapons fire once per turn.

Reloading is automatic. A weapon that fires during one turn is ready again on the next turn.

## Resolution Priority

Firing priority:

1. Artillery/cannon fire
2. Cannon crew personal weapons
3. Officers
4. Muskets
5. Rifles
6. Melee after eligible defensive fire

If a unit charges into melee, eligible ranged/defensive fire resolves before melee begins.

## Combat Model

Combat uses a detailed probabilistic model based on:

- Weapon accuracy
- Range
- Cover
- Morale
- Unit type
- Fatigue
- Formation
- Facing
- Random chance
- Terrain
- Friendly fire
- Unit strength
- Officer effects
- Special abilities

Squads track:

- Remaining soldiers
- Casualty count
- Combat strength

Severe hits may reduce visible soldier count.

Officers track:

- Alive
- Killed
- Routed

Officers cannot be wounded in version 1.

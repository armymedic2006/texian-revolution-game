# Fog of War, Visibility, and UI Information Rules

## Fog of War

Orders are hidden from the opposing player until both players press Ready.

Units outside enemy field of view are hidden.

Mexican forces cannot see inside the Alamo interior until Mexican units enter or gain line of sight into the interior.

## Line of Sight

Line of sight is blocked or affected by:

- Walls
- Buildings
- Terrain
- Dense unit formations

Smoke is excluded from version 1 but should be designed for later.

Sound detection is excluded from version 1 but should be designed for later.

Weather, time of day, and lighting gameplay effects are excluded from version 1 but should be designed for later.

## Resolution Visibility

Single-player:

- Show only actions visible to the player’s units.

Hot-seat:

- Show neutral/revealed actions only.
- Do not reveal hidden information unfairly.

## Unit Information Visibility

### Morale

Exact morale state is visible to both players for visible units.

Hidden units reveal no morale state.

### Fatigue

Owner sees exact fatigue.

Opponent sees general behavior only.

### Combat Strength

Owner sees exact soldier count and combat strength.

Opponent sees approximate labels:

- Full strength
- Strong
- Reduced
- Weak
- Nearly destroyed

### Weapon Type

Exact weapon visibility depends on:

- Distance
- Scouting ability
- Line-of-sight quality

### Officer Identity

Exact officer identity depends on:

- Distance
- Line of sight
- Scouting ability
- Recognition conditions

All officers use the same identification rules.

### Facing

Facing visibility depends on:

- Distance
- Scouting ability
- Line-of-sight quality
- Fog-of-war status

Owner always sees exact facing.

Opponent may see exact, approximate, or no facing information depending on visibility conditions.

### Cover State

Cover visibility depends on:

- Distance
- Line-of-sight quality
- Scouting ability
- Fog-of-war conditions

Owner always sees exact cover state.

Opponent may see exact, approximate, or inferred cover state.

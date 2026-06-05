# Core Systems

## Morale

Morale states:

1. Fresh
2. Steady
3. Shaken
4. Broken
5. Routed

Morale is unit-specific and affected by:

- Leadership
- Casualties
- Nearby allies
- Nearby enemies
- Battlefield events
- Nearby leaders killed/routed
- Nearby friendly units breaking/routing
- Nearby enemy units breaking/routing
- Fatigue
- Artillery
- Melee
- Victory events

Suppression is part of morale, not a separate stat.

## Morale Recovery

Units can recover morale through:

- Rally actions
- Leaders
- Rest
- Nearby allies

Routed units generally cannot recover, except Texian-specific routed behavior.

## Mexican Broken/Routed Rules

When a Mexican unit becomes Broken:

- It retreats toward nearest map-exit/fallback point.
- If it reaches that point before recovering to Shaken, it leaves the map and is removed from play.
- After 3 turns without being attacked or taking casualties, it can recover to Shaken if it has not exited.
- Officer rally sequence:
  - Turn 1: unit becomes Broken
  - Turn 2: Mexican officer within rally range issues rally
  - Turn 3: unit returns to Shaken
- Nearby Mexican units breaking/routing can worsen morale.
- The second time a Mexican unit would become Broken, it becomes Routed.

## Texian Broken/Routed Rules

When a Texian unit becomes Broken:

- Still controllable
- Poor accuracy
- Poor ranged effectiveness
- Slower movement
- Reduced general combat effectiveness

When Routed:

- Uncontrollable
- May only fire defensively from current position
- If not eliminated within 2 turns, returns to Shaken
- The second time a Texian unit would become Broken, it becomes Routed

Regardless of morale state, Texian melee attack and melee defense remain at Fresh-level effectiveness.

Texian Broken/Routed units can contest victory points.

## Texian 4x Boost

Each Texian unit has:

- Two manual uses per game
- Unlimited automatic triggers

Manual use:

- Player selects it manually
- Lasts 2 turns
- Followed by 2-turn cooldown
- Consumes one of two manual uses

Automatic trigger:

- Does not consume manual uses
- Unlimited
- Triggers when:
  - Unit becomes Broken
  - Unit becomes Routed
  - Unit is badly outnumbered

Badly outnumbered means:

- Mexican forces outnumber Texian unit 4:1
- Based on individual soldiers represented inside nearby squads/units
- Must be within fixed radius and line of sight

Boost affects:

- Morale
- Ranged attack
- Melee attack
- Melee defense
- Movement
- Damage inflicted against Mexican forces

## Fatigue

Fatigue states:

1. Fresh
2. Winded
3. Tired
4. Exhausted

Fatigue affects:

- Movement
- Accuracy
- Melee
- Morale
- Construction/repair work

Fatigue increases from:

- Moving long distances
- Charging
- Melee combat
- Building/repairing defenses
- Breaching/climbing/destroying obstacles
- Operating artillery
- Being under fire
- Low morale

Fatigue recovers through:

- Resting or taking no strenuous action
- Being near an officer
- Morale recovery

Exhausted units can still act but suffer severe penalties.

Texians resist fatigue penalties better than Mexican units.

All Texian unit types share one Texian fatigue-resistance model.

All Mexican unit types share one Mexican fatigue model.

## Formation

Formation states:

1. Normal
2. Defensive
3. Charging
4. Disorganized

Formation affects:

- Movement speed
- Ranged accuracy
- Melee attack
- Melee defense
- Morale checks
- Vulnerability to artillery
- Construction/repair ability
- Line of sight / visibility

A unit becomes Disorganized when Broken or Routed.

A unit recovers from Disorganized automatically when morale improves to Shaken.

## Facing

Facing is included in version 1.

Facing affects:

- Line of sight
- Firing arcs
- Flank/rear vulnerability
- Melee defense
- Defensive fire
- Disengagement
- Visibility/fog of war
- Artillery firing arcs

Facing changes:

- Small facing changes are free.
- Large facing changes consume movement or action capacity.

Facing during planning:

- Unit may automatically face movement direction.
- Unit may automatically face attack target.
- Player may manually set final facing.

Facing visibility depends on distance, scouting, and line-of-sight quality.

## Cover

Cover states:

1. Exposed
2. In Cover
3. Fortified
4. Entrenched
5. Behind Barricade

Cover affects everything:

- Ranged combat
- Melee defense
- Morale
- Artillery vulnerability
- Visibility
- Movement/positioning where applicable
- Construction and fortification effects

Cover assignment:

- Exposed: automatic when no cover
- In Cover: position/terrain based
- Behind Barricade: position based
- Fortified: action-based
- Entrenched: construction/improvement based

Movement:

- Position-based cover updates automatically.
- Action-based cover is lost when the unit moves.

Artillery and breaching attacks can degrade cover.

Cover-providing structures use the same damage states as structures.

## Modifier Rules

Morale bonuses stack without cap.

Combat-effectiveness bonuses stack without cap.

Penalties stack without cap.

Math:

- Major effects use multipliers.
- Smaller modifiers use additive percentages.

Examples:

- Texian 4x boost: multiplier
- Tennessee Riflemen melee 3x: multiplier
- Crockett Old Betsy accuracy/range: multiplier
- Bowie knife 6x lethality: multiplier
- Mexican musket close-range +33%: additive
- Santa Anna killed +25% Texian defense/melee: additive

Central modifier engine:

- Document for future.
- Do not implement full central modifier engine in MVP.
- MVP may calculate modifiers inside individual systems.

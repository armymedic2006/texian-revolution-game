# AI Requirements

## AI Modes

Single-player mode requires AI for either faction.

AI difficulty:

- Easy
- Normal
- Hard

## Difficulty Effects

Difficulty affects:

- Tactical decision quality
- Morale resilience
- Accuracy/combat effectiveness
- Aggression toward victory points
- Officer use
- Artillery use
- Flanking
- Breaching
- Coordination

Difficulty does not change unit numbers.

## AI Fairness

AI obeys same fog-of-war and hidden-order rules as player.

AI does not know:

- Hidden units
- Hidden orders

AI may use:

- Visible information
- Last-known enemy positions
- Objectives
- Difficulty-based tactical quality

## Last-Known Positions

Depends on difficulty:

- Easy: short/limited memory
- Normal: moderate memory
- Hard: longer memory and better prediction

## Targeting Hidden Units

AI may target last-known positions depending on:

- Weapon type
- Difficulty
- Plausibility
- Recency
- Line of fire
- Friendly-fire risk

## Feints

All AI difficulties can use feints.

Feints use real units only.

No ghost indicators in version 1.

## AI Victory Behavior

AI should understand:

- Mexican objective victory requires controlling all victory points before the turn limit.
- Mexican immediate victory occurs when all Texian defenders are killed.
- Texian objective victory occurs by holding at least one victory point at the turn limit.
- Texian immediate victory occurs by killing/routing all Mexican forces off-map.
- Texian immediate victory also occurs if Santa Anna is routed.

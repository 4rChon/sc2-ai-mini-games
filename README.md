Descriptions are given in the same format as the mini-game descriptions given here: https://github.com/deepmind/pysc2/blob/master/docs/mini_games.md

A target skill is specified for each map under Additional Notes.

## DefeatZealots

### Description

A map with 2 Stalkers opposite to 3 Zealots. Rewards are earned by using the Stalkers to defeat the Zealots. Whenever all Zealots have been defeated, a new group of 3 Zealots is spawned and the surviving Stalkers are moved to a random point on the opposite spawning location, retaining their existing health. Whenever new units are spawned, all unit positions are reset to opposite sides of the map.

### Initial State
* 2 Stalkers at a random side of the map (preselected)
* 3 Zealots at the opposite side of the map from the Stalkers

### Rewards
* Zealot defeated: +5
* Stalker defeated: -1

### End Conditions
* Time elapsed
* All Stalkers Defeated

### Time Limit
* 160 seconds

### Additional Notes
* Fog of War disabled
* No camera movement required (single-screen)
* Target skill(s): Kiting

## DefeatZealotsBlink

### Description
Same as DefeatZealots but the Stalkers have Blink.

### Initial State
* 2 Stalker at a random side of the map (preselected)
* 3 Zealot at the opposite side of the map from the Stalker

### Rewards
* Zealot defeated: +5
* Stalker defeated: -1

### End Conditions
* Time elapsed
* All Stalkers Defeated

### Time Limit
* 120 seconds

### Additional Notes
* Fog of War disabled
* No camera movement required (single-screen)
* Target skill(s): Blink and Kiting

## DefeatSingleZealot

### Description

Same as DefeatZealots but with 1 Stalker and 1 Zealot.

### Initial State
* 1 Stalker at a random side of the map (preselected)
* 1 Zealot at the opposite side of the map from the Stalker

### Rewards
* Zealot defeated: +5
* Stalker defeated: -1

### End Conditions
* Time elapsed
* Stalker Defeated

### Time Limit
* 120 seconds

### Additional Notes
* Fog of War disabled
* No camera movement required (single-screen)
* Target skill: Kiting

## MoveToBeaconAvoidBaneling

### Description

Move the probe to the beacon, while avoiding the enemy baneling.

### Initial State
* 1 Probe at a random point on the map.
* 1 Beacon at random point on the map, at least 5 units from the probe.
* 1 Baneling at random point on the map, at least 5 units from the probe.

### Rewards
* Beacon reached: +1
* Probe killed: -3

### End Conditions
* Time elapsed
* Probe killed

### Time Limit
* 120 seconds

### Additional Notes
* Fog of War disabled
* No camera movement required (single-screen)
* Target skill: Avoiding enemies.



Descriptions are given in the same format as the mini-game descriptions given here: https://github.com/deepmind/pysc2/blob/master/docs/mini_games.md

## Defeat Zealots

### Description

A map with 2 Stalkers opposite to 3 Zealots. Rewards are earned by using the Stalkers to defeat the Zealots. Whenever all Zealots  have been defeated, a new group of 3 Zealots is spawned and the surviving Stalkers are moved to a random point on the opposite spawning location, retaining their existing health. Whenever new units are spawned, all unit positions are reset to opposite sides of the map.

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

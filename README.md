# Project 5
## Implementation / Features you added
- Light system:
-   By default, the maze is completely dark, save for a small light illuminating the area in front of a player. When a room is cleared of enemies, or if it doesn't have enemies in it, glowing orbs will descend from the ceiling to light up the space. This marks rooms already visited or safe rooms and gives better visibility.
-   The two light sources, then, are the point light tied to the player and the light orbs created when a room is cleared.
- Procedural terrain and enemy generation:
-   Rooms have a chance to spawn with four pieces of terrain providing cover and spots for enemies to hide behind. The distance of the terrain from the center of the room, the rotation of the terrain (either at a 45-degree angle or a 0-degree angle), and the dimensions of each piece have slight variance. 0-3 enemies will spawn in each room at a point with no terrain. The number of enemies spawned depends on how many enemies were spawned in the previous room. If a room has 0 enemies, the next room is guaranteed to have at least one enemy. If a room has 3 enemies, the next room will only have 0-1 enemy. The room the player spawns in never has enemies.
- Player HUD:
-   The player has a HUD displaying their health bar, bullet count, and whether they are reloading. If they take damage, the bottom-left and top-right corners of the HUD will flash redbefore fading out.
- Health, healing, and damage:
-   The health bar on the player's HUD adjusts length based on remaining health, turning yellow if the player is under half health and red if they're below 25% health. Enemies can damage the player by colliding with them - the player will take 5 damage (out of 20 max health) and then receive invulnerability for a brief period. As mentioned before, two corners of the HUD will flash red to represent this.
-   When the player clears a room, there is a small chance for a healing orb to descend from the ceiling. The healing orb is another small light source with particles, and when walked into the player will heal 5 health (or 8, if the player is below half health). Healing orbs also have a chance to spawn in a room with 0 enemies!
- A few features that might be too small to count on their own but could together,  maybe?
-   Bullet system: Each time the player uses the left mouse button to "shoot," they'll lose a bullet (of maximum 10). Once they reach 0, they will spend 2 seconds "reloading," in which they can't shoot. The number of bullets the player has, as well as whether they are currently reloading, are reflected in the player HUD.
-   Juicy features: When an enemy takes damage, they'll emit a burst of red particles and flash red before fading back to white. (This is achieved by making a clone of the enemy's material and changing its color! Because of this, multiple enemies can have different shades of red at the same time). Light orbs and healing orbs spawn above the ceiling and gradually move down, and healing orbs emit particles with trails until collected.
-   Slightly nicer menus: Menus feature a camera slowly rotating around a room made to look like one that could procedurally generate in the game, and have a little bit of lore above the start buttons.
-   Slighly changed rooms: To make sure too much light doesn't bleed between tiles, each maze tile is given a ceiling, and instead of removing entire walls between connected rooms, a small doorway is opened for the player instead.
-   The cursor is locked to the center of the screen and invisible during gameplay but is visible and free to move in menus.


## References
Rubik Distressed:
Copyright 2020 The Rubik Filtered Project Authors (https://https://github.com/NaN-xyz/Rubik-Filtered)
This Font Software is licensed under the SIL Open Font License, Version 1.1 .

## Future Development

## Created by
Graham Baker

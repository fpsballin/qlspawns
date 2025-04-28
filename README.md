Top down views of maps for the game Quake Live, with circles indicating respawn points.

You can see the maps at https://fpsballin.github.io/qlspawns/

Credit for the Quake Live TDM map images goes to maf from esreality (https://esreality.com/post/2865176/schemes-of-tdm-maps/).
Credit for the Duel images and code goes to Memento_Mori from esreality (https://www.esreality.com/?a=post&id=2219012).

The logic for where a player can respawn is roughly "the furthest 50% of spawns away from currently living players". Technically, the distance from a living player to a spawn is calculated as the maximum of the x axis distance and the y axis distance. By this distance, the closest 50% of spawns (rounded down) are blocked from occurring, and a spawn from within the furthest 50% of spawns is chosen randomly.

The mouse cursor is the location of a living player, and (in modes other than Duel) additional living players can be placed as pink circles by clicking. Given the location of the mouse cursor and any other pink circles placed on the map, the green circles should show possible spawns (furthest 50%) while the red circles are spawns that are blocked from happening (nearest 50%).

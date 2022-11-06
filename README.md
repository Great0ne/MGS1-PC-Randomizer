# MGS1 PC Randomizer v1.0
Metal Gear Solid 1 Items/Weapons randomizer for GOG PC version made with CheatEngine using LUA/Assembly.

# How to use
- Launch the game, launch the trainer, click Randomize and test it.

# Randomizing what and how ?
- This Randomizer will randomize Items and Weapons for every pickup according to the player's belongings.
- For the CheatEngine choice, which will modify game data during gameplay, 
  it is mostly because I wanted to make a quick and simple launcher to make and use without the need of too much external components.
- How it is randomized ? 
  There are four different pickup types in the game, unique item like Thermal Goggles, counted item like Ration, Unique weapon like Socom and Ammo.
  Knowing that, for each pickcup the received item is randomized, first by type Item or Weapon only if the original pickup is unique just to guarantee balancing,
  and given to the player, but if the randomizer item is a weapon then ammo is randomized according to their type.
  The bomb is received with a timer randomizer from 3 to 10 seconds.
  The ID Card is received with it's level randomized from 1 to 7, but will be reset to expected value while progressing the story. 
- Textbox 
  Also, I tried to use the ingame text to display the new item instead of the old, it was working until boss fights where the game crash,
  sadly too much code on the update so I added a textbox which you can move around that will display new items, 
  not a fan of adding visual elements but it is better than checking your inventory every time.
  
# Issues
- Balancing, 
  There is a 1 out of 2 chance to get item or weapon, which could cause a lack of items with bad luck.
- ID Card,
  Can cause glitches if used at high level too early.
- Cardboard Box,
  Can cause softlock if used without the needed ID card level, like the Box C to teleport to Snowfield where you need a level 6 ID Card.
- Walls and C4,
  If the player have no C4 to destroy walls, know that you can destroy them with Stinger too, or go back pick up reappeared items.
- Wolf's ambush to Meryl,
  If the player has already PSG1, then the fight with Wolf will trigger with Meryl on the ground without the possibility to go back,
  so keeping PSG1/Stinger/Nikita ammo is advised.
- Pal Key, (FIXED)
  If got randomly before needed, then the rat drop will give it to a null state, fixed it.
- Escape Rations, (FIXED)
  Picking up rations during escape caused crash if an item was given instead, added code to fix it.

# Credits
Credits to Denezhou on the fearlessrevolution forums for the MGS1 CheatTable which make me gain a lot of time.

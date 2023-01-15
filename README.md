# MGS1 PC Randomizer v1.0
Metal Gear Solid 1 Items/Weapons randomizer for GOG PC version made with CheatEngine using LUA/Assembly.

# How to use
- Launch the game, launch the Trainer, click Randomize and test it.
- Can be activated/deactivated anytime.

![mgsr1](https://user-images.githubusercontent.com/110473739/200180648-4c2b8633-8f7b-48a2-81da-f4322025265c.gif)
![mgsr2](https://user-images.githubusercontent.com/110473739/200182692-f0dfad0f-b495-404f-a05a-645a73f4fdd7.gif)
![mgsr3](https://user-images.githubusercontent.com/110473739/200182695-faac1141-7db9-4afc-8ffb-4af3d2e306ff.gif)

# Randomizing what and how ?
Since there wasn't any MGS1 randomizer, I made my own, it's not perfect but if it can make people play a bit more at this gem of a game then it's a job done.
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
  I tried to use the ingame text to display the new item instead of the old, it was working until boss fights where the game crash,
  sadly too much code on the update so I added a textbox which you can move around that will display new items, 
  not a fan of adding visual elements but it is better than checking your inventory every time.
  
# Issues
- Balancing, 
  there is a 1 out of 2 chances to get item or weapon, which could cause a lack of items with bad luck.
- Max Ammo,
  seems like the code set to increment max ammo is overridden by the game, don't be surprised to see 4/3 rations and sorts.
- ID Card,
  can cause glitches if used at high level too early.
- Cardboard Box,
  can cause softlock if used without the needed ID card level, like the Box C to teleport to Snowfield where you need a level 6 ID Card.
- Walls and C4,
  if the player have no C4 to destroy walls, know that you can destroy them with Stinger too, or go back pick up reappeared items.
- Wolf's ambush to Meryl,
  if the player has already PSG1, then the fight with Wolf will trigger with Meryl on the ground without the possibility to go back,
  so keeping PSG1/Stinger/Nikita ammo is advised.
- (FIXED) Pal Key,
  if got randomly before needed, then the rat drop will give it to a null state.
- (FIXED) Escape Rations,
  picking up rations during escape caused crash if an item was given instead.
- Display Ingame Pickup,
  added temporary solution to display randomized pickup with movable transparent window, original ingame display causes crashes
  during boss fights.

Feel free to report any encountered issues.

# Credits
Credits to Denezhou on the fearlessrevolution forums for the MGS1 CheatTable which made me gain a lot of time.

# Disclaimer
This is not a commercial project. It is not affilated with Konami. It doesnt endorse piracy in any form. You need to own a PC version of the game to play this mod. All copyrighted content belongs to their respective owners and may not be illegally distributed.

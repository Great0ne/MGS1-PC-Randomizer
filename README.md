# MGS1 PC Randomizer v1.1
Metal Gear Solid 1 Items/Weapons randomizer for GOG PC version made with CheatEngine using LUA/Assembly.

# How to use
- Download the EXE file, Launch the game, launch the Trainer, wait for the trainer to recognize mgs process, choose custom name/settings and click Randomize to test it.
- Can be activated/deactivated anytime, but I would suggest to let it activated during play.

![MGRnd0](https://github.com/user-attachments/assets/48d75889-f260-4906-ab1c-054bc61e6369)
![MGRnd1](https://github.com/Great0ne/MGS1-PC-Randomizer/assets/110473739/68a1c876-33ae-44f8-80b8-044acccb2a0f)
![MGRnd2](https://github.com/Great0ne/MGS1-PC-Randomizer/assets/110473739/7dafb3c8-761a-44bc-9528-272a1356b302)

# Randomizing what and how ?
Since there wasn't any MGS1 randomizer, I made my own, it's not perfect but if it can make people play a bit more at this gem of a game then it's a job done.
- This Randomizer will randomize Items and Weapons for every pickup according to the player's belongings.
- For the CheatEngine choice, which will modify game data during gameplay, 
  it is mostly because I wanted to make a quick and simple launcher to make and use without the need of too much external components.
- How it is randomized ? 
  There are four different pickup types in the game, unique item like Thermal Goggles, counted item like Ration, unique weapon like Socom and counted weapon like       Grenade.
  Knowing that, for each pickup the received item is randomized, first by type Item or Weapon only if the original pickup is unique just to guarantee balancing,
  and given to the player, but if the randomizer item is a Weapon then Ammo is randomized according to their type.
  
  The Bomb is received with a timer randomized from 3 to 10 seconds.
  
  The ID Card is received with it's level randomized from 1 to 7, but will be reset to expected value while progressing the story.
  
# Update v1.2
  - setting pickup type (item/both/weapon) for each 4 pickup objects
  - pickup alert trigger chance
  - pickup sneeze chance & sneeze timer min
  - timer bomb timer min/max
  - every item/weapon pickup chance
  - fix pickup with full inventory
# Update v1.1
  - custom name (7 char max)
  - setting min/max pickup weapons
  - max pick up bullets (Socom/Famas)
  - deactivate respawns during boss fights
  - other fixes.

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
- (PARTIALLY FIXED) Display Ingame Pickup,
  pickup name is now displayed in game, but when multiple items are picked only the last is displayed.
- If no rope has been found after entering Communication Tower 1, you can be blocked after triggering the Hind sequence before rappel
  because the bottom door will be shut.Finding the rope before the stairs sequence is advised.
- (FIXED) Pickup Number,
  pickup number is now displayed in game along the pickup name.
- (PARTIALLY FIXED) Suppressor Respawn,
  equipping suppressor to Socom was setting back suppressor state to 0, changed the way suppressor nis checked before pickup.
- (FIXED) Unlimited Respawn,
  during Boss fights some weapons reappear when the player have no ammo for certain weapons, settings is accessible from launche to enable/disable it.

Feel free to report any encountered issues.

# Credits
Credits to Denezhou on the fearlessrevolution forums for the MGS1 CheatTable which made me gain a lot of time, and to Gear2 for his cheattable which the trigger alert is copied.

# Disclaimer
This is not a commercial project. It is not affilated with Konami. It doesnt endorse piracy in any form. You need to own a PC version of the game to play this mod. All copyrighted content belongs to their respective owners and may not be illegally distributed.

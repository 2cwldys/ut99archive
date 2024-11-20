Dynamic Arena for Unreal Tournament
Version 1.1
Mar, 17th 2010
http://moddb.com/mods/dynamicarena


=== Installation:

Place all the files inside your "UnrealTournament\System\" folder.



=== Setup:

Start a practice session and add the proper mutator to play the mod.

There's also a Mod menu in-game, where you can change the mod settings to suit your taste.



=== W.O.R.M integration:

You can easily create your custom list if you have the W.O.R.M (Weapon/Object Replacement Mutator).

Basically, W.O.R.M is a weapon replacer mutator with a cool menu that read weapon names from .int files.

I've managed to integrate this list into the mod menu, so it's easier to create your own list.

Although to be able to use this, you must have the W.O.R.M mutator, and proper .int files for the mods.

You can download it from one of these links:

http://www.moddb.com/games/unreal-tournament/downloads/worm-v190
http://download.beyondunreal.com/fileworks.php/wod/UT99/worm190.zip



=== Multiplayer:

If you want to estabilish a server, make sure to add the proper serverpackage.

Open the UnrealTournament.ini, locate the section [Engine.GameEngine].

There, find the last line of serverpackages and place a line like this one below:

ServerPackages=DynamicArena

This is not necessary, but without it the clients won't see messages and hear sounds of the mod.

If you're using a custom weapon list with custom weapons (besided UT and U1 weapons), you should also
add the proper serverpackages to each of those mods, otherwise the weapons won't appear on the clients.



=== Changelog:

v1.0 (Mar, 11th 2010)
- Initial release

v1.1 (Mar, 17th 2010)
- New feature: added integration to WorM plugin for easily editing your custom list
- Added support for Unreal1 Weapons (not being replaced by UT)
- Fixed a crash that would happen if using a custom list with only one valid weapon
- Set to load default weapon list if custom list doesn't have any valid weapons entries
- Minimum timer set to 3 seconds, since 1 second, since it wouldn't even allow you to fire once
- Timer will only be set when game starts, and will stop properly when game ends
- Fixed bots pulling their recently received weapons instantly
- When changing weapons, players will stop firing automatically to prevent suicides
- Global messages at the beggining of the map will appear correctly, counting the number of weapons
- "Spectating bots" won't receive weapons at the beggining of the map (prior to starting properly)
- Added a background image to the mod menu



- Darkness
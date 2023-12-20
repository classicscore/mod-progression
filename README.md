# Progression
The goal of this module is to go through the patches of Wrath of the Lich King. The included patches are 3.0, 3.1, 3.2, 3.3 and 3.3.5. Every patch includes changes to simulate that patch as best as possible. Information on what is new in each patch can be seen by browsing their folder, although there are probably things listed that aren't implemented yet.

# Installation
* Clone the repository in the modules folder that comes with the AzerothCore source. The structure should be `/modules/mod-progression`
* Build the server the same way you build AzerothCore. Specific steps included below
* Use cmake to generate the project files
* For Windows you compile the source using Visual Studio. For Linux, run make to compile the source
* For Windows the config file is `/configs/modules/mod-progression.conf.dist`
* For Linux the config file is usually `/etc/modules/mod-progression.conf.dist`
* Make a copy of the config file and name it `mod-progression.conf`. This is the file that you edit the values of
* Start the server like normal and the auto-updater will take care of the database imports

# Note
Keep in mind that it's not anywhere near complete even if there seems to be a lot done. I have not yet looked at the PvP vendors so those are a huge mess.

The next major thing to look at is the Argent Tournament Grounds. It was released in 3.1 but more was added to it in 3.2 along with the dungeon and raid.

The way to handle this is to go through every single quest, one by one, and check each one while completing them to make sure they should exist in 3.1. If not, it's relatively easy to see where 3.1 ends and 3.2 begins in terms of the available quests.

Aside from quests, a lot of the other things are already done and anything missed will be picked up when checking the quests.

# Limitation
I am currently limiting this to Wrath of the Lich King so that I can get it to the point where I would consider it to be ready for production. I might be adding The Burning Crusade afterwards followed by Vanilla, only time will tell.

# Corrections
Create issue reports for anything that isn't correct and I will look into it as soon as I have the time to. If something isn't intended to be in a certain patch I want to change it and would greatly appreciate reports for it.

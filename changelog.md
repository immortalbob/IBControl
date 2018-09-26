Changelog:
1.9.9
- Version number now listed at very top of meta
- Removed things you should not edit from the *** Edit Here *** state. I know, right?
- Purged all outputted "Chat Commands" in favor of Chat Expressions, and OptSet from all states except *** Edit Here ***.
- (New Feature) "#chase <character name>" Multi-following command to be able to follow more than only one character. Old "#action follow" command still works, and serves as a simple follow. Create a nav file to follow a character you have. Name it "chase <character name>" and be sure it is case sensitive. issue the command. EX: #chase Immortalbob
- (New Feature) Now sends a message to the leader (charone) when it has <=50 Prismatic Tapers, or <=3 Platinum/Mana Scarabs
- (New Feature) Now sends a message to the leader (charone) when main pack space falls to just 4 slots.
- (New Feature) Sets ChaosHelper chat command to /s automatically. (will change back to /f if GDLE devs ever fix fellow chat)
- (New Feature) Sets ChaosHelper to tab 1 automatically upon initial load of the meta (Basic tab) (requires CH 2.2.5)
- (New Feature) New chat command: #where Send via @tell to one of your characters (from the leader only), it will send the leader that character's coordinates to the leader. (does not have a button in CH, must be sent via chat)
- (New Feature) New chat command: #getoverhere <character name> Pulls your location info, and sends an @tell to the character name, it will then clear his nav route, and set a nav point to your location. Local chat only for #getoverhere command, however, you can @tell your character with #cometo <coordinates> directly. When character reaches the coordinates, it will turn simple follow back on. Leader only (charone) command. Note: Does not auto follow with any chase navs as referred to further up in this list. Must re-issue "#chase <playername>" command. No CH button for this.
- (Bugfix) "/mt select" button fixed to work with the new thwargfilter commands. (/tf instead of /mf)
- (Bugfix) Fixed remote view to be the right dimensions.
- (Bugfix) Summoning portals now sets idlepeacemode to false.
- (Bugfix) No more error spam on your first command!

1.9.8
- (Bugfix) IBCRemote now sends commands to local chat only. (I will change this to fellowship if the gdle devs ever fix fellow chat)
- (Bugfix) Chaos Helper, and IBCRemote no longer pop up each time the *** Edit Here *** state is called.
- (Feature) Fellowship recruits no longer need to be edited in, it is all based on your character list now.
- (Feature) Leader no longer needs to be edited in, it is based on your first character in the character list. (charone)
- (Option) Fellowship creation is now optional, it will still try to recruit fellow members.
- (Option) Message sent to leader (charone) upon death, coordinates sent upon outdoor death.
- (Option) Permit leader (charone) with corpse looting permissions upon death.
- (Option) Meta no longer clears nav route upon initial load, this is an option now.

1.9.7
- Securing your commands no longer requires editing the regex code!!! See new setup above.
- Removed Aphus requirement for Portal Recall, Lifestone Recall/Sending, Primary/Secondary Recalls, MP/House/Mansion Recalls
- recomp no longer goes to mp when complete
- Summoning portals now functions
- Legendary Chest Meta removed for now

1.9.6
- Changed commands to use # instead of !

1.9.5
- Top of *** Edit Here *** state got more options, CH config file, /mt autopack, Auto Read Contracts, and Auto Craft
- Set Options in top of *** Edit Here *** state to always or never to toggle them!
- AutoCraft will automatically combine Pyreal Motes, Pyreal Slivers, Dark Specks, Dark Slivers, Dark Shards, Cracked Shards, Tiny Shards, Small Shards, and it will reveal aetheria (if you have an Aetheria Mana Stone)
- AutoReadContracts will read contracts immediately upon receiving them in inventory if in default2 state.
- Navto Leather Crafter, Ivory Crafter, Stone Collector, and Collector added
- Updated Chaos Helper configs to reflect new nav options

1.9.4
- bugfixes
- Locked !ext commands into case sensitive exact matches this way you cant load a blank meta
- Nav To, and Quest states now require your character has learned the Aphus Recall spell.
- Viridian Portal button now functional in CH.
- Alternate navs for Gear Knight, Colosseum, Viridian Rise, Paradox, Bur, and Aerlinthe x 2
- Alternate Gear Knight route requires 1 mmd in inventory, alternate Aerlinthe requires either 1 d note, or 1 c note and 1 sake.
- Nav now re-enables after Use Closest Portal
- Viridian Root navigation added, with/without Viridian Rocks Recall

1.9.3
- bugfixes
- Eats contracts at rynthid again! might miss one or two sometimes
- Fellow/Disband only works for the designated leader now, and the command can be issued from any member of your group.
- Fastcast Buffs, Do Not Shoot At Walls, and Use Breakable Turn To buttons added to CH.
- You can now set your preferred profiles for settings, loot, and window tool in the top of the ** Edit Here ** state
- !extension command has been abbreviated to !ext
- Remote Control using the new meta views system. you can disable this in the top of the ** Edit Here ** state
- Extension State will now not just load any blank meta if you misspell the meta you are trying to load, it must match a predefined variable. if you don't match it'll kick you back to default2.
- navto state also now kicks you back to default2 if you don't match any defined variables.

1.9.2
- bugfixes

1.9.1
- Release


Known Issues:
1.9.4
- fix spammy recalls

1.9.3
- Hoshino killtask route needs tweaking to avoid house barriers /done in 1.9.4
- Viridian Portal needs to work dammit /done in 1.9.4
- !ext still allows partial matching /done in 1.9.4
- using sanctuary recall without recall spell, or Invitation Ithaenc Cathedral in inventory gets you stuck in Nav To 2 state /done in 1.9.4

1.9.2
- rynthid killtask issue again...this time for recall...blah /done in 1.9.3
- toutou npc misorder /done in 1.9.3

1.9.1
- Jumps dont work until the anniversary update is released, should be soon Vtank was updated!
- forgot to remove /mt jump from Arwic Chests route /done, fixed in 1.9.2
- Reload Meta single/all loads the wrong meta....oops? /done, fixed in 1.9.2
- extra space in ***edit here*** state, follow getvar[leader]==0 /done, fixed in 1.9.2
- Colosseum nav doesnt clear var /done, fixed in 1.9.2
- master mage route needs open doors true added to it /done, fixed in 1.9.2
- add clear route to nav to !reset command /done, fixed in 1.9.2
- !action select command missing from chaos helper /done, fixed in 1.9.2
- rynthid killtask nav issue /done, fixed in 1.9.2
- use closest portal issue /done, fixed in 1.9.2
- !Extension changed to !extension in chaos helper /done, fixed in 1.9.2
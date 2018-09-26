For the 10th Anniversary of Vtank, a new version of IBControl!!

This is totally a beta, i tested out most of it...seems to be in order. Please leave feedback on what needs to be updated, and/or bugs.

What is IBControl?
IBControl is a meta that allows you to control an entire fellowship running the virindi bundle + magtools. On the fly setting changes, make them jump, send them all to mayoi, whatever you want to do!

It is meant to be a player driven meta, it will not just do things for you other than navigation to predefined areas. You are at the helm of a 9 man fellowship, and all the controls you might need are at your fingertips!

Below you will find screenshots of the Chaos Helper UI that IBControl uses, each predefined command has a button, however there is room for unlimited custom chat commands. (explained below)


Requirements:

    Virindi Bundle of course
    Magtools https://github.com/Mag-nus/Mag-Plugins/releases
    Chaos Helper 2.2.2.0+ viewtopic.php?f=6&t=282
    Aphus Lassel Recall for most of the navigation


What do I do with the zip file?

    unzip files
    Place IBControl.met into your Vtank dir (usually c:\games\virindiplugins\virinditank)
    Download and Install Chaos Helper into decal.
    Place IBControl_config.txt, and IBControl.layout into the chaos helper folder (and the 2's).
    Place Master Celdiseth the Archmage.utl into C:\Users\YourName\Documents\Decal Plugins\Mag-Tools


Setup:
Everything you need to edit is now handily in the uppermost state in the meta called "*** Edit Here ***". Below is an image with the areas you need to edit in order to make the entire meta functional.

1. On the left you can toggle settings on or off by changing always to never, or vice-versa. For the first two lines, if you do not want the remote, or chaos helper profiles loaded, set them to false.

2. On the right if you MUST change your fellowship name, it is set to CHANGEME. If you wish to use predefined profiles upon meta start up, you can enter their names in place of <profilename>. Remember it is case sensitive.

3. Characters: on the right, add each character name from your fellowship replacing CHANGEME. charone should be your leader.

4. Follow Nav: on an different character on another account from your leader, go to the route tab in vtank, choose follow from the drop down menu on the lower left, select your leader in game and hit the add button in the route tab of vtank. Now go to the meta tab, go to the %% Follow Nav %% section in the *** Edit Here *** state at the top. now open the rule up, click on load embedded nav file, and import your nav. (should say 1pts) Reload the meta on all characters in the vtank profile tab, and you're good to go!

How do I use it?
Once you have the files unpacked from the zip, and placed in the required directories just login to AC, load the meta in the profiles tab, and start vtank# The chaos helper window(control panel) should automatically open up. Stop right here though, you have to go through the setup process located in a post above. In order to make use of all of IBControl's features, follow the setup process above.

When your setup is completed IBControl is a breeze to use. You have 2 options in order to start commanding your fellowship, either press the buttons in Chaos Helper, OR type the commands out. Pressing the buttons is pretty self explanatory, but the commands get interesting. There are now 9 possible commands, with a whole lot of permutations. #navto, #optset, #jump, #quest, #action, #extension, #craft, #echo, and #use.

Chat Commands:

#navto
Syntax: #navto <place>
Example: #navto mayoi

#action
Syntax: #action  <action>
Example: #action face northeast

#quest
Syntax: #quest <quest name>
Example: #quest Tou-Tou Killtasks
- routes to npcs and flags for tou-tou killtasks

#optset
Syntax: #optset <vtoptionname value>
#optset enablebuffing true

#use
Syntax: #use <item name>
Example: #use Burning Coal

#jump
Syntax: #jump [heading] [shift true/false] [0-1000 milliseconds] [strafeleft/straferight/forward]
Example: #jump 300 true 500

#craft
Syntax: #craft [item one] with [item two]
Example: #craft Wrapped Bundle of Raider Lightning Arrowheads with Wrapped Bundle of Arrowshafts

#echo
Syntax: #echo <anything>
Example: #echo /vt refresh

#ext
Syntax: #ext <metaname>
Example: #ext LegendaryChestsIB

#where
Syntax: #where
Example: /t Immortalbob, #where

#getoverhere
Syntax: #getoverhere <charactername>
Example: #getoverhere Immortalbob

#cometo
Syntax: /t <charactername>, #cometo <coordinates>
Example: /t Immortalbob, #cometo 12.4N, 42.3E

#chase
Syntax: #chase <charactername>
Example: #chase Immortalbob


#quest, #navto, and #action are very very lenient on what you actually type in. For example, "#navto may" will send you to mayoi, "#navto eas" will send you to eastham, but if you want eastwatch, you could only shorten it to #navto eastw. On a side note, I would recommend "#navto jal", and "#navto arq" for al-jalima, and al-arqas.

#optset, #jump, #use, #craft, and #ext are the non-lenient commands. They have to be typed in correctly to function. (case sensitive on the #use, #craft, and #ext commands)

#optset can make use of every vtank option with a chat command that starts with /vt opt set. If there is a setting you need to switch that is not in the chaos helper control panel you can type "#optset optionname setting"
For example: #opt set corpseapproachrange-min 0.014

#use can use any item in your pack. simply type #use itemname

#craft one item with another, see syntax above.

#echo will echo any chat command you put in throughout your fellowship. For instance, "#echo /mt logout" will logout all of your characters running the meta.

#ext loads another meta, ex: #ext LegendaryChestsIB

#getoverhere will send an @tell with the #cometo command to the character you requested with your coordinates, and set a nav route to your coordinates. when coordinates are reached it will automatically switch to follow mode. There is no Chaos Helper button for this. (see syntax above)

#cometo sent in an @tell to a character, this can be used to send a set of coordinates for them to nav to. There is no Chaos Helper button for this. (see syntax above)

#where sent in an @tell to a character, the character will send you their coordinates in an @tell. There is no Chaos Helper button for this. (see syntax above)

#chase if you have a follow nav route named chase <character name> you can use this command to follow any character. Case sensitive! There is no Chaos Helper button for this. (see syntax above)

Note: Fellow chat commands will not function until the GDLE devs fix fellow chat to be in line with retail. You can change chaos helper to use /s instead of /f.

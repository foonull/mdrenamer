mdrenamer
=========

**Description**: Command line tool version of MDRenamer for renaming Halo full maps to MD format.

**Usage**: mdrenamer.py <input_map> <mod_name> <short_name> <build_number> [output_directory]

**Example**: python mdrenamer.py ~/Desktop/Maps/bloodgulch.map "Best Mod" bestmod 1

**Arguments**:

<*input_map*> The file path to the Halo map file to rename

<*mod_name*> The user friendly name of the mod. Must be <= 13 characters; truncate if necessary. This is not the same as the name that shows up in the MD database, but the one that shows in the map selection menu in-game.

<*short_name*> The internal name of the mod that will be used in the outputting filename. Must be all lowercase and >= 1 character(s)

<*build_number*> The build number of the mod which is also used in the outputting filename. This should be increased before any sort of public or private distribution. Must be an integer >= 1

[*output_directory*] The directory to output the new MD renamed map in. This is optional and defaults to the directory <input_map> is in

**Additional Constraints**:

string_length(<short_name>) + string_length(<build_number>) < 13

**System Requirements**

* Python 2.7.x or 3.x (check python --version in a terminal)

**See also**:

[HaloMD Website](http://halomd.net)

[Mac Gaming Mods Forums](http://macgamingmods.com/forum/)
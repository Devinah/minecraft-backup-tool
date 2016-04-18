# Minecraft Backup Tool #
A simple backup utility for [Minecraft](http://www.minecraft.net).

![http://www.autoplay.org/media/MinecraftBackupTool.png](http://www.autoplay.org/media/MinecraftBackupTool.png)

[More screenshots](http://code.google.com/p/minecraft-backup-tool/wiki/Screenshots)

You are free to modify this project in any way! :)

(Out of courtesy, please respect the open source community and always include any previous authors/contributors in the credits.)

## Instructions ##

  1. Simply download the zip file and extract the executable to the location of your choice.
  1. The first time you run the tool, click the Settings button to configure your Minecraft.exe location, etc.
  1. You can click on the map thumbnail to view it in your default PNG viewing program.

The rest should be pretty self-explanatory. :)

Note: All settings are stored in %AppData%\Minecraft Backup Tool\settings.ini.

## History ##
_v1.0 - 2010-10-20_
  * Initial release

_v1.0.1 - 2010-10-20_
  * Fixed a couple typos on the About page
  * Added the version number to the About page

_v1.0.2 - 2010-10-21_
  * Fixed a bug where the map wasn't being auto-generated when you exited Minecraft
  * Refactored the INI save/load code a bit
  * Added the ability to set NumWorldSlots in the settings.ini file (min=1, ~~max=9 for now~~)

_v1.0.3 - 2010-10-26_
  * Fixed a bug in 1.0.2 where the settings folder wasn't being created if it didn't exist yet

_v1.0.4 - 2010-10-27_
  * Added the ability to insert a comment into the backup filename
  * Changed how available backups are listed in the Restore GUI to accommodate the comments
  * Increased the max possible world slots to 20 (see NumWorldSlots in settings.ini)
  * Added RestoreListSortOrder to settings.ini (e.g. "Newest First" or "Newest Last")
  * Fixed a minor bug: if the index for SelectedWorld in settings.ini was out of range, the same world slot you selected on the main page wouldn't be selected on the Restore GUI by default until you exited and restarted MBT

## Why another backup tool? ##

I've been enjoying Minecraft and I went looking for a tool to backup and restore the world files. I found some tools that handled backups well enough, but I didn't find a tool that made restoring as straightforward as it could be.

My goals for this project were to:

  * provide an easy way to make and **restore** world backups
  * take advantage of the cool cartography tools that exist, such as [AlphaVespucci](http://www.minecraftforum.net/viewtopic.php?f=25&t=33522) and [c10t](http://www.minecraftforum.net/viewtopic.php?f=25&t=33803)
  * make an open project that anyone in the Minecraft community could modify and extend


## What is Minecraft? ##

[Minecraft](http://www.minecraft.net) is a very cool game in development by Markus Persson (a.k.a. "Notch"). It is a [sandbox game](http://en.wikipedia.org/wiki/Sandbox_game) where the world is made up of simple textured cubes or "blocks." The player has the ability to manipulate this world by mining, crafting, and placing blocks. This very simple metaphor and the associated gameplay encourage the player to manipulate the world in increasingly creative ways.

It's a wonderful experiment in [emergent gameplay](http://en.wikipedia.org/wiki/Emergent_gameplay): as I play Minecraft, I find myself continually inventing new things to try, in a sense creating different sub-games for myself around the simple crafting and exploration mechanics of the core game.

Minecraft is still in alpha, but it is already very fun. It's kind of a combination of playing with Lego blocks and hiking. You get to build stuff, largely for the sake of building it...and you get to explore a procedurally generated world made up of little blocks that is often surprisingly beautiful.


## Required Tools ##
[AutoPlay Media Studio Personal Edition](http://www.autoplay.org) (free for non-commercial use)

Note: You do not need anything to use the Minecraft Backup Tool — it is a standalone application. You only need AutoPlay Media Studio Personal Edition if you want to edit the source files.

## AutoPlay Media Studio ##
AutoPlay Media Studio is a development tool that started out in 1997 as an app for making CD menus. Over time it has evolved into a platform that is well suited to making utilities and small applications, with an event driven, object-based architecture, and harnessing the power of [Lua](http://www.lua.org/).
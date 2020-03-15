# Unusual Effects

![overview](https://i.imgur.com/w4HY6Nc.gif)

### Description

This is a Counter-Strike: Global Offensive [sourcemod](https://www.sourcemod.net/) plugin that introduces cosmetic unusual effects from Team Fortress 2. Includes head effects and feet effects. 
[See here for a (almost) full overview.](https://gfycat.com/finemellowantipodesgreenparakeet)

### Setup

1. [Download](https://github.com/Erroler/Unusual-Effects/archive/master.zip) the plugin from this git repository.
2. Upload everything to your gameserver.
3. Edit *addons/sourcemod/databases.cfg* and add a database entry for the plugin:
> "unusual"<br>
	{<br>
		"driver"			"sqlite"<br>
		"database"			"unusual-effects"<br>
	}<br>
4. Edit server convars on *cfg/sourcemod/unusual_effects.cfg* to your taste.

### Chat Commands

Open the menu:

* **!ue**
* **!unusualeffects**
* **!unusual**
* **!unusuals**

### Server Convars

* **sm_ue_method** - This plugin has two alternative ways of putting the effects on the players: *normal* (more stable, can't hide head effects in first person), *experimental* (buggy, sometimes doesn't work but hides head effects in first person). Default value: **normal**
* **sm_ue_flag** - Restrict usage of the plugin to players with the given sourcemod flag. Default value: **o**
* **sm_ue_allow_thirdperson** - Allow the usage of third person on the menu. Default value: **1**

### Known bugs

* Players can't see this the effects the first time they connect after downloading the files from the server. **This is unavoidable.** The client's game engine only loads the particle effects next time the map changes.

### Changelog

**0.2** (15/03/2020) - Removed server convar related to restricting access to menu after X seconds passed since the round started. Added server convar to restrict access to third person.
**0.1** (14/03/2020) - Initial release.

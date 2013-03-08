store-sounds
============

### Description
Store module that allows players to play custom sounds.

### Requirements

* [Store](https://forums.alliedmods.net/showthread.php?t=207157)
* [SMJansson](https://forums.alliedmods.net/showthread.php?t=184604)
* [Sound Info Library](https://forums.alliedmods.net/showthread.php?t=105816)

### Features

* **Customizable** - You can have any amount of sounds you want, and you can customize each sound in its `attrs` field.
* **Sounds are downloaded automatically** - You don't need to configure that.
* **Wait time** - You can set a minimum wait time between each sound so players won't spam the server.

### Installation

Download the `store-sounds` archive from the plugin thread and extract to your sourcemod folder intact. Then open your store web panel, navigate to Import/Export System under the Tools menu, and import configs/store/json-import/sound.json

### Adding Sounds

This package comes with 0 sounds, so you'll have to add your own sounds or songs. To do that, open the web panel, navigate to **Add New Item** under the **Items** menu. `type` should be `sound`. Change `name`, `display_name`, `description` and `attrs` to customize your new sound.

The attributes field should look like:

	{
		"path": "store/mysound.mp3",
		"volume": 0.5
	}

Note that `path` is relative to your game's `sound` directory. Volume is optional, and you can also add a `text` property which will appear when a player plays the sound.
# Loading Mods into Plutonium

This page will cover how loading scripts and mods work for all our games.  
You can find scripts and mods in the modding releases sections on our forums:

- [For T4](https://forum.plutonium.pw/category/40/waw-modding-releases-resources)
- [For T5](https://forum.plutonium.pw/category/60/bo1-modding-releases-resources)
- [For IW5](https://forum.plutonium.pw/category/27/mw3-modding-releases-resources)
- [For T6](https://forum.plutonium.pw/category/23/bo2-modding-releases-resources)

Note that you don't need to restart the game to (re)load your `.gsc` scripts.  
You can simply end the current level/game you're in and start a new one.  
You can also run `map_restart` in the [console](https://plutonium.pw/docs/opening-console/) which will restart the current level/game you're in.  
To go faster you can even run the command below once so that the `map_restart` command will be ran whenever you press `P` on your keyboard, while in a game focused on the game (console closed, chat closed etc).  
Change P to any other unused key you want. `bind P "map_restart"`

## T6

### Getting started with GSC on T6

Note that if you only want your script to load in multiplayer it should be placed in the `mp` folder that's in this `scripts` folder. On the other hand, if it should only be loaded in zombies then place it in the `zm` that's in this `scripts` folder.  
If you want it to load in both simply put it inside the `scripts` folder.

1\. Navigate to the T6 Plutonium scripts folder by pressing `Win+R` and pasting `%localappdata%\Plutonium\storage\t6\scripts` into it, and hitting Ok.

2\. Put any amount of GSC files in here, I will be using the following code as an example.  

<Alert variant="warning">

If you are writing your own GSC, you must have an `init()` or `main()` function somewhere.  
This function is called the 'entry point', it's a function the game engine is familiar with and will call.

</Alert>

```cs
init() // entry point
{
    level thread onplayerconnect();
}

onplayerconnect()
{
    for(;;)
    {
        level waittill("connected", player);
        player thread onplayerspawned();
    }
}

onplayerspawned()
{
    self endon("disconnect");
    for(;;)
    {
        self waittill("spawned_player");
        self iprintlnbold("^2GSC from the scripts folder");
    }
}
```

4\. Verify your GSC looks like mine, and is in the correct location.

![img](/images/docs/modding/loading-mods/t6-gsc-1.png)

5\. Open BO2, start a new Private Match or Dedicated Server, your GSC script should load.

![success](/images/docs/modding/loading-mods/t6-gsc-2.png)

### Loading existing scripts on T6

1\. Download the script of your choice, scripts can be found on the [Modding Releases section](https://forum.plutonium.pw/category/23/bo2-modding-releases-resources) on our forums.

2\. Installation instructions for the mod are usually included in the release's post.  
If you simply get gsc script(s) it most likely goes into `%localappdata%\Plutonium\storage\t6\scripts` if it's a generic script or in `scripts\mp` for mp only or in `scripts\zm` for zm only.

3\. Start the game, the script will be loaded automatically.

Note that you can load both source code/uncompiled scripts and compiled scripts, the instructions are the same.

## IW5

### Getting started with GSC on IW5

1\. Navigate to the IW5 Plutonium Folder by pressing `Win+R` and pasting `%localappdata%\Plutonium\storage\iw5` into it, and hitting Ok.

2\. If you don't have a folder called `scripts` here, then create it.

![img](/images/docs/modding/loading-mods/d3AnJ4R.png)

3\. Put any amount of GSC files in here, I will be using the following code as an example.

<Alert variant="warning">

If you are writing your own GSC, you must have an `init()` or `main()` function somewhere. This function is called the 'entry point', and it's a function the game engine is familiar with and will call.

</Alert>

```cs
init() // entry point
{
    level thread onplayerconnect();
}

onplayerconnect()
{
    for(;;)
    {
        level waittill("connected", player);
        player thread onplayerspawned();
    }
}

onplayerspawned()
{
    self endon("disconnect");
    for(;;)
    {
        self waittill("spawned_player");
        self iprintlnbold("^2GSC from %localappdata%\Plutonium\storage\iw5\scripts\example.gsc");
    }
}
```

4\. Verify your GSC looks like mine, and is in the correct location.

![img](/images/docs/modding/loading-mods/LSrZkI0.png)

5\. Open MW3, and start a new Private Match or Dedicated Server, your GSC script should load.

![success](/images/docs/modding/loading-mods/X2qZtj5.png)

### Loading existing scripts on IW5

1\. Download the script of your choice, scripts can be found on the [Modding Releases section](https://forum.plutonium.pw/category/27/mw3-modding-releases-resources) on our forums.

2\. Installation instructions for the mod are usually included in the release's post.  
If you simply get a single gsc script it most likely goes into `%localappdata%\Plutonium\storage\iw5\scripts`.

3\. Start the game, the script will be loaded automatically.

### Loading mods on IW5

1\. Navigate to the IW5 Plutonium Folder by pressing `Win+R` and pasting `%localappdata%\Plutonium\storage\iw5` into it, and hitting Ok.

2\. If you don't have a folder called `mods` here, then create it.

3\. Move your mod inside the `mods` folder

4\. Once in-game [open the console](/docs/opening-console) and type `/fs_game "mods/my_mod"` where `my_mod` is the name of your mod (how the folder is named)

5\. Start a game and play with your mod

## T4

### Loading mods / custom zombies maps

If you are installing a mod that comes as a `.exe` file then you can simply run it and and follow the instructions to install it.  
The mod will then be installed in `%localappdata%\Activision\CoDWaW\mods`.  

If you are installing a mod that comes as a folder, you can follow the instructions below.  

1\. Navigate to the T4 Plutonium Folder by pressing `Win+R` and pasting `%localappdata%\Plutonium\storage\t4` into it, and hitting Ok.

2\. If you don't have a folder called `mods` here, then create it.

![img](/images/docs/modding/loading-mods/Zzpf3O5.png)

3\. Place any mods in that folder.

__Note:__ Mods for multiplayer must have their folder name start with `mp_`.

![Mods showing up](/images/docs/modding/loading-mods/6qchlaS.png)

---

### Loading custom maps (MP)

{/*
We support both the vanilla game folder and the Plutonium folder for loading client-side custom multiplayer maps.

You can place your mod in either of these places:

- `%localappdata%\Activision\CoDWaW\usermaps`
- `%localappdata%\Plutonium\storage\t4\usermaps`   __(Recommended)__

*/}

1\. Navigate to the T4 Plutonium Folder by pressing `Win+R` and pasting `%localappdata%\Plutonium\storage\t4` into it, and hitting Ok.

2\. Create a folder called `mods`

![img](/images/docs/modding/loading-mods/Zzpf3O5.png)

3\. Place any custom maps in that folder.

Once the map is installed, you must load a mod first. If you do not have a mod to go along with your custom map, you can load a dummy mod by [opening the console](/docs/opening-console) and typing `/fs_game mods/mp_custommaps; vid_restart` followed by `/map mp_yourmapname` and it should load right up.

## T5

### Loading mods / custom zombies maps for BO1

1\. Navigate to the T5 Plutonium Folder by pressing `Win+R` and pasting `%localappdata%\Plutonium\storage\t5` into it, and hitting Ok.

2\. Create a folder called `mods`

![img](/images/docs/modding/loading-mods/bo1-mods.png)

3\. Place any mod in that folder.

__Note:__ Mods for multiplayer must have their folder name start with `mp_`.

4\. Load the mod via the in-game "Mods" menu.

5\. If you want to play on a custom zombies map you need to first load it via the "Mods" menu, then start it via the console by running the command `map mapname`. You can find the name of the map by looking at it's files in the mods folder (e.g. `zombie_kow`).

# Loading Mods into Plutonium

This page will cover how loading scripts and mods work for all our games.  
You can find scripts and mods in the modding releases sections on our forums:

- [For T4](https://forum.plutonium.pw/category/40/waw-modding-releases-resources)
- [For T5](https://forum.plutonium.pw/category/60/bo1-modding-releases-resources)
- [For IW5](https://forum.plutonium.pw/category/27/mw3-modding-releases-resources)
- [For T6](https://forum.plutonium.pw/category/23/bo2-modding-releases-resources)

## T6

### Requirements for writing GSC scripts

[GSC Tool](https://github.com/xensik/gsc-tool/releases/latest) (required to compile your script)

---

__Example scripts__

- [9 Perks for Zombies](https://forum.plutonium.pw/topic/29/all-perk-slots-unlock-script-zombies)
- [Jugg for joining players](https://forum.plutonium.pw/topic/112/jugger-for-new-players-joining-at-or-after-round-8-zombies)
- ["A cat has 9 lives"](https://forum.plutonium.pw/topic/449/mob-of-the-dead-mod-a-cat-has-9-lives)

---

### Getting started with GSC on T6

1\. You can write/download any GSC of your choice.  
If you are writing it from scratch/have the source code, note that you will need to compile it, which we will talk about later.

<Alert variant="warning">

If you are writing your own GSC, you must have an `init()` or `main()` function somewhere. This function is called the 'entry point'.  
It's a function the game engine is familiar with and is able to call when your script runs at the start of a game.

</Alert>

2\. For this tutorial, we are going to be writing and using this GSC as a reference.  
You can simply open a notepad, paste the content below inside it then save the file as a `.gsc` file.

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
        self iprintlnbold("^2GSC from %LocalAppdata%\\Plutonium\\storage\\t6\\scripts\\mp\\test.gsc ^1(Compiled)");
    }
}
```

3\. Using the GSC Tool downloaded in the requirements section, you can easily turn a source script into a compiled script that the game will be able to read and run by following the [instructions](https://github.com/xensik/gsc-tool#usage).  
For T6 the command should look something like  
`gsc-tool.exe comp t6 "%localappdata%\Plutonium\storage\t6\scripts\mp\example.gsc"`.  

To make working with T6 scripts easier you can also create a batch file containing the following commands and run it using Windows cmd or your IDE's integrated terminal.

```bat
@echo off
cls
copy "example.gsc" "%localappdata%\Plutonium\storage\t6\scripts\mp\example.gsc" /y >NUL
gsc-tool.exe comp t6 "%localappdata%\Plutonium\storage\t6\scripts\mp\example.gsc" 
```

It will simply copy your source file directly into the `scripts\mp` folder and compile it right after, showing you the result of the compilation process, without modifying the original source file that you're currently working on.  

Of course, replace the first copy command argument with the name of the source GSC file you're working with, or the full path to it.  
Also put the exact same path for the second copy argument and the `gsc-tool` 3rd argument (the path) so that it will compile the file that got copied.

3b\. If you get an error, make sure your script isn't already precompiled (open it, and if it looks like gibberish, it is already compiled)  

![t6-compiling-already-compiled-error](/images/docs/modding/loading-mods/t6-compiling-already-compiled-error.png)

3c\. If you get an error and your script isn't compiled then read the error and fix the line and column where the error is.  
For example here the compiler throws a very clear error on the third line because I added `;` twice when only one should be there.  

![t6-compiling-syntax-error](/images/docs/modding/loading-mods/t6-compiling-syntax-error.png)
![t6-compiling-syntax-error-gsc](/images/docs/modding/loading-mods/t6-compiling-syntax-error-gsc.png)

4\. Take your compiled script and put it into `%localappdata%\Plutonium\storage\t6\scripts\mp` or `%localappdata%\Plutonium\storage\t6\scripts\zm` depending on which mode it is for.  
If your script should always be loaded no matter the game mode copy it to `%localappdata%\Plutonium\storage\t6\scripts`

7\. When launching your server or a custom game, you will know if all has gone well or not if the console prints `Custom script 'scripts/mp/yourScriptName' loaded`.

![Success](/images/docs/modding/loading-mods/oVlCBnI.png)

8\. Enjoy your new GSC script!

![In Game](/images/docs/modding/loading-mods/bun6iFx.png)

### Loading existing scripts on T6

1\. Download the script of your choice, scripts can be found on the [Modding Releases section](https://forum.plutonium.pw/category/23/bo2-modding-releases-resources) on our forums.

2\. Installation instructions for the script are usually included in the release's post.  
If you simply get a single gsc script it most likely goes into `%localappdata%\Plutonium\storage\t6\scripts\mp` or `%localappdata%\Plutonium\storage\t6\scripts\zm` depending on if it's a script made for multiplayer or zombies.

3\. Start the game, the script will be loaded automatically.

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

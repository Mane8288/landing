# How to move your mods folder to another drive

<Alert variant="info">

This tutorial was written for the `mods` folder of World at War (T4) but these instructions are valid for any other folder given that you update the paths accordingly.

</Alert>

1. Make sure any Plutonium game is closed.

2. Press `Windows + R`, paste this: `%localappdata%/Plutonium\storage\t4\` and press Enter.  
**MOVE** (not copy) the `mods` folder to the new location you want.  
For example move the `mods` folder inside `D:\Plutonium\T4`

3. If you installed mods by running installers or if you were using mods on Steam you probably have a `mods` folder in `%localappdata%/Activision\CoDWaW\` too. If you do then repeat step 2 with that folder.  
It should merge with the existing `mods` folder that's in `D:\Plutonium\T4` (in this example)

Here is a screenshot of how your Plutonium T4 folder should look like (left) and how the `mods` folder you just moved should look like (right). Take a look at the paths on top of each window.  
![img](/images/docs/modding/moving-to-another-drive/before-command.png)

4. Open a **Command Prompt** as **Administrator**.  
You can do this by searching for `cmd` in Windows Search, and right clicking `Command Prompt` and pressing `Run as Administrator`

![img](/images/docs/modding/moving-to-another-drive/e9aMqpv.png)

5. Copy this command to your clipboard:

```batch
mklink /J "%localappdata%\Plutonium\storage\t4\mods" "D:\Plutonium\T4\mods"
```

6. If needed, update the second path to match new the location of your `mods` folder.

7. Right click inside the command prompt window to paste, then press enter.

8. If everything is working the command prompt should write `Junction created`

Here is a screenshot of how your Plutonium T4 folder should look like after running the command.  
A `mods` folder should have been created, containing all the mods you have in `D:\Plutonium\T4\mods`.

![img](/images/docs/modding/moving-to-another-drive/after-command.png)

Note that these folders are synced so placing new files/folders in any of these folders will "update" the other as well, you don't need to run this command again unless you delete one of these two `mods` folder.  
You can install mods in the T4 mods folder just like before or in the new location.  
In both cases it will now take disk space in your `D:` disk (in this example)

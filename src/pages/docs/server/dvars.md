# Plutonium specific server settings

We have a few dvars that are specific to Plutonium.

## T6

* `sv_allowAimAssist 1` - Allow Aim Assist on gamepads. (Setting this to 0 will lock the option on gamepad controls menu.) This is on by default, turn this off to disable aim assist when on your server.
* `sv_allowDof 1` - Changes whether Depth-of-Field can be enabled or disabled. (Setting this to 0 will force depth of field to be disabled for everyone. Setting this to 1 will allow each user decide)
* `demo_enabled 1` - Currently not functioning. Has no effect.
* `demo_currentDemo` - Dvar to get the current match's demo file name. (This dvar is read-only.)
* `g_customTeamNames` - Allows you to change the name of teams. (Example: `set g_customTeamNames "allies,plutonium.pw|axis,forum.plutonium.pw"`, or `set g_customTeamNames "allies,Allies|axis,Axis|team3,Team 3|team4,Team 4|team5,Team 5|team6,Team 6"` for multi-team)

## IW5

* `sv_allowAimAssist 1` - Allow Aim Assist on gamepads. (Setting this to 0 will lock the option on gamepad controls menu.) This is on by default, turn this off to disable aim assist when on your server.
* `sv_motd` - Sets a custom motd which is shown on the intel message loadscreen when a player joins. Leave blank for the default intel messages.
* `sv_enableBounces 1` - Enables bouncing on the server, `sv_enableBounces 2` allows for double bounces.
* `sv_enableDoubleTaps 1` - Allow double tap on weapon switching.
* `sv_wwwBaseURL` - URL for downloading mods from. [Learn more about FastDL for IW5 here](/docs/server/iw5/fastdl).
* `fs_game` - What mod are we loading. [Learn more about FastDL for IW5 here](/docs/server/iw5/fastdl).
* `sv_allowThirdPersonSpectator` - Allows clients to spectate players in thirdperson.

## T4

* `g_patchRocketJumps 1` - Enable/disable rocket jumps.

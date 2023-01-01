# Custom Games / Playing with friends

<Alert variant="tip">

On T6 and T5 most players should be able to invite people out of the box.  
In case it doesn't work you will have to take extra steps just like before.  
On T4 and IW5 you may need to take extra steps to be able to join your friends.  

If you don't know what these code names refer to you can take a look at the [engine explanations doc](https://plutonium.pw/docs/engine-explanations/).

</Alert>

This guide will teach you how to play with friends over the internet in a custom games match.  
No matter which game you're trying to play **the first step is to follow each other on the forum**.  
See [Add a friend to your friend list](#add-a-friend-to-your-friend-list)

Hosting isn't complicated but involves several networking concepts that you need to understand before diving in so please make sure to take your time to read this guide to understand the concepts involved in hosting.  
You can also take a look at the [Introduction](#introduction) if there's anything you don't understand.

## Introduction

### Why do I need to do all this?

First of all you need to know that Plutonium ask you to do all these steps because hosting servers costs money, which is why most games on Steam don't require anything from you other than clicking "Create a game".  
But for indie games and passionate projects like Plutonium hosting a server for everyone would cost way too much money so you're required to host your games yourself instead which is free for everyone.  
As for Black Ops and Black Ops II, Plutonium worked on a system that tries to make it all work out of the box but depending on your network configuration it might fail and you will then need to port forward to ensure that system works.

### How does hosting work?

Basically when you want to host a service such as a game server (or a private game with your friends) there is an important concept to understand: who can access my network and which service can they access. You don't want people from the outside to have access to everything on your PC.
If you want to play with 2 PC connected on the same internet router you can connect to each other using your **local IP** because both devices trust each other.
But when you want to play with people who aren't connected to your router (so basically people from outside your home) that's a different story because they're all considered as strangers and potential threats. This is where the concept of **ports and port forwarding** comes in.

### What is UPnP?

Throughout this guide you'll see the words "port forwarding" and "UPnP" mentionned. To host a server/custom game you need port forwarding which requires manual setup on your router.
The idea behind [UPnP](https://en.wikipedia.org/wiki/Universal_Plug_and_Play) is to let your router automatically open and close ports as you open/close services (such as game servers) on your PC, so it's basically an easy automatic port forwarding.
Keep in mind that UPnP and port forwarding are two different things so **port forwarding will not enable UPnP**, but they have the same goal. UPnP is nice to have things work right away without any configuration but it doesn't work with every network setup so if it doesn't work for you, you will have to manually port forward instead.

### What is port forwarding?

To make it simple everything connected to the internet running on your PC uses a [port](https://en.wikipedia.org/wiki/Port_(computer_networking)).
The internet going through these ports can either be **outbound connections** (you connecting to Google or to a game server for example) which doesn't require anything on your side or **incoming connections** which means you receive connections from the outside (hosting).
In that case you need to **forward** the port used by your service (in that case your game server) to tell your router to allow connections from the outside on that specific port.
Otherwise, by default and for security concerns the incoming connections on this port will be blocked. So if you understood this correctly: only the host needs to have a port opened (or UPnP enabled) on his router. The people joining don't need to do anything on their end, just like when you join a public server.

### How to enable UPnP?

- Enable UPnP on your router if it's not enabled already.  
Since every router is different we can't make a guide for every router.  
We recommend searching "your router name + enable UPnP" on Google or searching in your router settings.  

- Go to Windows Settings -> Network & Internet, then hit Properties under your network name.

![img](/images/docs/custom-games/PnaSif4.png)

- Set the Network Profile to Private

![img](/images/docs/custom-games/hC6G8QN.png)

- Restart the game

### How to port forward?

Hosting a private match without UPnP or when your friends cannot join out of the box requires you (the one who invites the others/hosts) to port forward (see [What is port forwarding?](#what-is-port-forwarding)).  
Since every router is different we can't make a guide for every router so we recommend searching "your router name + port forward" or "your [ISP](https://en.wikipedia.org/wiki/Internet_service_provider) name + port forward" on Google/Youtube.  

You can either create a port range rule, for example 1000-1005 will open every port from 1000 to 1005 including 1000 and 1005 or you can create a rule for each port required, the result is the same.  
The port(s) value/range is given on the section for your game. Each game can have a different port so read the section for the game you're trying to play on that page.  
For example `28960-28961` means both the port `28960` and the port `28961` or a port range from `28960` to `28961`.  
On the other hand `3074` means you only have to open that specific port.

Opening a single port should look something like the screenshot below.  
Here are the most common things you need to know. You might not have all these settings.

- Rule name can be anything, something descriptive like Plutonium T6 is recommended
- Protocol is UDP (Both works too but isn't required)
- The port/value to enter is the port given in the section for your game
- External and internal port values should always be the same
- Destination port is the port for your game
- Source port can either be blank or a wildcard or all/everything depending on your router. You need to allow any/all source port

![img](/images/docs/custom-games/port_forward_example.png)

## Add a friend to your friend list

Both you and your friend need to follow each other on the Plutonium forums to join each other:

- Go to [https://forum.plutonium.pw/users](https://forum.plutonium.pw/users) and make sure you're logged in then search for your friend's Plutonium name.
- Go to their profile and hit the green "plus" (+) button to follow them.
  - If there is a heart, that means that you are already following them.
  
Once you both follow each other you will see your friend in the game's friend list (or in the Plutonium overlay's friend list tab for T4).  
If after following each other you can't see each other in your friends list in-game just restart your game.

## T6

In T6 inviting your friend should work out of the box.

### **Inviting your friend(s)**

- Make sure your party privacy is set to open (P)
- Make sure nothing will block the connection (your router firewall, your antivirus firewall if you have any etc.)
- Open the friends list (F)
- Invite your friend(s)

![inviting players](/images/docs/custom-games/t6-inviting-as-host.gif)

Your friend(s) can now accept the invitation.

![accepting an invitation](/images/docs/custom-games/t6-joining-sesh.gif)

### **If it didn't work**

First make sure you followed the steps correctly.  
Next what you can try is simply letting another friend invite you/the other players.

If it still doesn't work no matter what you do then you will have to port forward the port `3074` (UDP) on your router (see [How to port forward?](#how-to-port-forward)).  
Once this is done you can restart your game and invite your friend(s) again by following the instructions above.

## IW5

In IW5, there's no easy way of telling if UPnP is enabled, outside of just testing it.  
There is no party system in Plutonium IW5 so your friend(s) can only join you while you're in-game.

### **If UPnP is enabled**

Start a private match and have your friend join you by following these steps:
- Open the friends menu (F)
- Double click on the name of your friend who's hosting

### **If UPnP is disabled / is not working**

- Forward the port `27016` (UDP) on your router (see [How to port forward?](#how-to-port-forward)).  
- [Whitelist the port in Windows firewall](https://www.tomshardware.com/news/how-to-open-firewall-ports-in-windows-10,36451.html)
- Make sure nothing will block the connection (your router firewall, your antivirus firewall if you have any etc.)
- Once those steps are done, open your game and start a private match. **(Parties will not work)**

- Your friend should now be able to join you by following these steps:
  - Open the friends menu (F)
  - Double click on the name of your friend who's hosting

## T4

<Alert variant="tip">

There is no party system in Plutonium T4 so your friend(s) can only join you while you're in-game (or finished loading in the loading screen).  

To be able to play with your friends on round 1 in zombies you can force the game to wait in the loading screen until a certain amount of players connect with this command `sp_minplayers 2`.  
This command needs to be entered in the [console](/docs/opening-console/).  
Replace `2` by the number of players you want to wait for before starting the game.

</Alert>

Once you and your friend are following each other, the person who wants to host the private match needs to do the following:

- Open the game and open the serverlist (F10 or Home key)
- Go to the network tab and check if UPnP is enabled

---

### **If UPnP is Enabled**

- Start a Private Match

If the match requires 2 players to start you can force it to start anyways by starting a game using the solo button.  
Don't worry, it's not actually solo, it will start an online private match that your friends can join.  
Alternatively you can use the `xpartygo` command to force the match to start.

- Once the game is started your friend should now be able to join by double-clicking your name in the Friends List tab of the Plutonium overlay

If you can't get it to work even with UPnP enabled then you will have to port forward instead.  
For this read [If UPnP is still disabled or you can't connect despite it being enabled](#if-upnp-is-still-disabled-or-you-cant-connect-despite-it-being-enabled).

---

### **If UPnP is Disabled**

- Enable UPnP (see [How to enable UPnP?](#how-to-enable-upnp))

- If UPnP is now enabled follow the [instructions above](#if-upnp-is-enabled).  
If it's not follow the [instructions below](#if-upnp-is-still-disabled-or-you-cant-connect-despite-it-being-enabled).

---

### **If UPnP is still disabled or you can't connect despite it being enabled**

- Forward these ports on your router `28960-28961` (UDP) (See [How to port forward?](#how-to-port-forward))
- [Whitelist these port in Windows firewall](https://www.tomshardware.com/news/how-to-open-firewall-ports-in-windows-10,36451.html)
- Make sure nothing will block the connection (your router firewall, your antivirus firewall if you have any etc.)
- Once those steps are done, open your game and start a private match. **(Parties will not work)**

If the match requires 2 players to start you can force it to start anyways by starting a game using the solo button.  
Don't worry, it's not actually solo, it will start an online private match that your friends can join.  
Alternatively you can use the `xpartygo` command to force the match to start.

- Your friend should now be able to join by double-clicking your name in the Friends List tab of the Plutonium overlay

## T5

- Make sure your party privacy is set to open or friends only or invite only
- Make sure nothing will block the connection (your router firewall, your antivirus firewall if you have any etc.)
- Open the friends list
- Invite your friend(s)

### Multiplayer

To play with friends on T5 Multiplayer you must start a private match and invite your friend to join.  
You need to be in-game to be joined. Inviting your friend in a multiplayer lobby will not work.

![image inviting friend to join](/images/docs/custom-games/t5-invite.png)

![image of friend in game](/images/docs/custom-games/t5-mp-joined.png)

### Zombies

To play with friends on T5 Zombies you can invite them while in a lobby.

![image in lobby inviting a friend](/images/docs/custom-games/t5-zm-invite.png)

![image of said friend in lobby](/images/docs/custom-games/t5-zm-joined.png)

### **If it doesn't work**

First make sure you followed the steps correctly.  
Next what you can try is simply letting another friend invite you/the other players.

If it still doesn't work no matter what you do then you will have to port forward the port `3074` (UDP) on your router (see [How to port forward?](#how-to-port-forward)).  
Once this is done you can restart your game and invite your friend(s) again by following the instructions above.

## Additional Notes

### LAN Play

If you and some / all of your friends are on the same LAN they connect through the internal IP, if all players are on the same LAN portforwarding is not necessary.

If you want to find your internal IP open a Command Prompt and type `ipconfig`.

![img](/images/docs/custom-games/gUXeTOE.png)

Your local IP will be under `IPv4 Address`.

From there, every client on your LAN will simply be able to connect by [opening the console](opening-console) and executing

```cs
connect HostsIPv4AddressHere
```

### Connecting via an IP address

If the friends list doesn't work for you, you can try connecting via an IP Address.

Have the host get their IP (which they can do via the Plutonium Overlay's Network tab, or via [WhatIsMyIP](https://www.whatismyip.com/))

Then, you will simply be able to connect by [opening the console](opening-console) and running the command

```cs
connect HostsIPAddressHere
```

# ResolumeClipNameM4L
Trigger Resolume clips with OSC using Ableton Live Clips Names

Syntax: 
ClipName /x/y

x = layer number or all
y = column number or stop

Examples:
- HiHat /all/1      => triggers column 1 for all layers
- CowBell /1/3      => triggers column 3 on layer 1
- Break /all/stop   => stop all layers
- Crash /2/stop     => stop layer 2

This patch is based on a modified version of Resolume Dispatcher from showsync.com/tools
It adds dynamic observer on all tracks to catch Clip Name when triggered.
The Clip Name is then parsed to find /x/y values and translated into appropriate Resolume OSC message.

You can use this modified Dispatcher in place of the original one, 
other showsync.com Resolume plugins (like Resolume Clip Launcher) will still work with it as with the original dispatcher.


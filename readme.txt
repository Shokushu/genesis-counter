GET THIS FIRST!
====================

OBS websocket
OBS connectivity requires OBSwebsocket plugin by Palakis - https://obsproject.com/forum/resources/obs-websocket-remote-control-of-obs-studio-made-easy.466/

====================
Instructions for the Genesis Counter
====================
You need to create 4 Text Sources (GDI +) in OBS studio. Here are the exact names you have to use for the sources :

p1hp
p2hp
p1aura
p2aura

They can be in any scene, they just have to have that name. The controller will modify their text values when you press buttons on the interface.

You then need to start LioranBoard Receiver(PC)/LioranBoard Receiver.exe and hit "Connect to OBS" in the menu to the left (make sure you have the obs websockets plugin installed). Normally you want to run this software on the same computer that is running OBS, but there are ways to circumvent this and run them on two different computers.

Once the receiver is running, keep it open and start the LioranBoard Stream deck(either PC or Android). If you decide to run it on an android device, you'll have to install the .apk file manually (transfer it via USB and run it to install it)

On the stream deck, enter the IP address of the PC that is running the receiver. If you are on the same network you can use the local ip address and leave the default port. If you are not on the same network, you may have to do some port forwarding for it to work. Select the deck #1 and hit connect.

That should be it!

If you have any questions, let me know on discord : Shokushu#3232
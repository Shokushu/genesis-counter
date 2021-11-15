====================
LioranBoard 1.44
Receiver 1.44
Stream deck 1.41

Check out for latest update Updates https://obsproject.com/forum/resources/android-stream-deck.862/

DISCORD
Need help? come ask question on the discord  https://discord.gg/dXez8Zh
====================
This is a program/app to control your stream, althought you can use it for anything if you so choose.
This can but does not only connect directly to OBS, but can also play sounds and simulate key presses(macro) of your choosing.
if you have some feedback or requests you can hit me up on twitch.tv/lioran or on discord.

OBS websocket
OBS connectivity requires OBSwebsocket plugin by Palakis - https://obsproject.com/forum/resources/obs-websocket-remote-control-of-obs-studio-made-easy.466/

====================
Instruction
====================
-Unzip all the files included here.
	Note: Everything is pretty much ready to be used right from this point, on the pc side, run the receiver and the stream deck, click connect on the stream deck and everything should work with a few default deck available.
	but you can keep on with the steps just to be sure.

-Run LioranBoard Receiver. It should ask you for network permission, Allow it.
	From this Point you can just Follow the tutorial, it should show you how to setup everything.
	IF NOT.
    You should see a gray window with options. if you wish to set the ports now is the time to do it,everything is set to work, you dont need to change anything.
    Click Accept when you are done. then you should see a few already existing Decks, the first one is called "1: Meme Sounds"
	Note: if you run OBS in admin mode, you will need to run the receiver in admin mode aswell if you wish for macros to be detected by OBS, otherwise you don't need to run it under admin mode)
	Note 2: LioranBoard may close right away, This might be due to your anti virus, if so allow it in your anti virus.
		If it still closes right away it might be due to a sound problem, If you use program like Voice Meeter, start lioranboard before you do voice meeter
		If you are not using voice meeter this might be due to a bad sound driver, you will need to figure out what that is on your own at that point.
		But installing proper driver for some sound device you have might solve this.

(You can skip this next step if you plan to only use the PC version of the stream deck)
-Load up the APK file included(Located in folder "LioranBoard Stream deck(Android)") onto your Android device and run/open that file.
	it should ask you if you wish to install this. Some phone don't like to run unsigned
	APK files. If you can't run it. go on google play store and download "Astro file manager" and run it through that.

-Now run the Stream deck of choice, Either the android one or the PC one.
    you can use the PC one for testing early on.

-Once the app is running you see a screen asking for IP,Port and board number.
	For the PC stream deck you can most likely just press connect right away and it should work.
    To know what Local IP to connect to on the android app, you can run the "whats my local ip.bat" file included. Look for "IPv4 adress" this is what goes into the ip adress box.
    Port is whatever you decided to set it as, should be left as default.
    Board Number refers to the number of the board you wish to see. leave it to 1 for now, and probably always.

-Click Connect and it should connect as normal and be fully ready to use.
    if it's failing to connect something might be blocking the connection or the default port is already being used by something else.

(You can skip the last few steps if do not wish to use Twitch connectivity)
-For Twitch connectivity you will need add the transmitter as a dock in OBS.(tsl_transmitter.html is included with lioranboard)
    In OBS click View at the top,
	Select Dock
	Select Custom Browser Deck
	In the URL box you want to put the full Path name of the transmitter (ex: c:/lioranboard/tsl_transmitter.html)
	You will see a page with a few test buttons and a status of it is connected to lioranboard.


-You can then go back on LioranBoard Receiver Click "Link your twitch".
    
-Verify that you agree with what the receiver is listening to and give it permission.
	If you don't agree with some of the permission you can copy the URL and remove what you don't want lioranboard to get permission on.
    Once accepted you should get multiple messages in the receiver saying everything is right, including the expiration date on the permission and listening for bits.

-all good
	You can use the transmitter to send fake test request to lioranboard, yellow message will popup on lioranboard when you press them.


Note: Regarding simulated key presses. If the program you are trying to control with shortcuts is running in administrator mode.
LioranBoard receiver will also need to be running in administrator mode for the keypress to be detected by the program.
So if OBS is running in Administrator mode, run LioranBoard receiver in administrator mode as well, otherwise it should not be needed.
IMPORTANT REGARDING MACROS: Do not use macro to do actions in online games. Most online games have anti cheat that detect those and consider it
use of 3rd party program, which can result in a ban. Most anti cheat program will block macros anyway.

Andoird Stream Deck has been tested on Amazon Fire HD10 7th gen and Samsung Galaxy A5 2017

====================
Updating Instruction
====================

If you downloaded a newer version and want to update it, here is what to do for the receiver.
Unzip the content. Drag and drop every files from the folder of the new version "Lioran Board Receiver (PC)" 
to the folder of the older version, Your folder might have a version number on it, i got rid of that as off 1.32.

To update the Stream deck you can just delete the old one and start using the new one, nothing special needs to be done.

Also recommended to always switch to the new transmitter.


====================
Editing your Deck
====================
-You can either click one of the deck Included or click "Add new Deck" and open that one.
    by default the size of the grid will be 5x5, Make that whatever size you want.


-To create a button click anywhere on the grid and click the Create button that pops up.
    with your newly created button, you can drag and drop it around where ever you like.
    You can expand your buttons by hovering the mouse at the left or bottom edge of a button and drag it


Right-click options
-Stop all sounds, will stop any sound effect the receiver might be playing with the given amount of millisecond fade out.
-Add sound, will let you add sounds with a given delay and volume.
-Add keypress, simulate a keypress of the given duration after the given delay.
-Change playing sound effect, will change the speed/volume of all currently playing sounds
-OBS commands, edit OBS commands sent to OBS (OBS commands are VERY extensive, you can put if statement and variable a little bit like a dumb down programming language) Requires the OBSwebsocket plugin
-Twitch triggers, allow you to make a button activate on subscription, bits and channel point redeems
-Switch deck. This will make that button switch to a different deck, don't make it switch to a nonexisting deck or one you've never edited, it will crash.
-Change color of the button, the copy will return an integer and put it in your clipboard (not hexadecimal)
-Add image, you can load up any picture you want, the program will make a copy of it in 128x128 and put it in the image folder included
-Copy Button, allows you to duplicate button easily
-Allow drag press, 3 different option of pressing mode,
    None: Activate when pressed
    Drag: Activate when pressed or moved over
    Multiple Drag: Activate when pressed or moved over(but will activate every time it's moved over again without lifting the finger)
-Delete button option


You can edit the name of the deck and the background color for the stream deck aswell.

====================
How to connect Multiple accounts
====================
To set a bot account or listen for multiple channels, when you link your account in LioranBoard, there is an Account box that's set to "Main" by default.
Select Alternate 1 to 10 and set the name of the account you wish to link. Must be the correct User Login name, else it will not work.

Once you've typed the name, Log in to that account, Make sure you are not logged in to the Main account. You can use an alternate browser or Incognito tab to make this easier
Once you're logged it click Copy Link and load it on that account.
The "Link Twitch Account" window should remain open during this process.
The green text in the window will confirm the account was linked.
Once you're done, close and restart lioranboard.
Next time the transmitter connects and you connect to twitch, you will see messages saying if the alternate account listen was success or failed.

The account you wish to be showed in chat should be the "Main" one.

====================
Freesound.org sound used for notifications and built in decks
====================
270402
270600
446114
255100
270468
272044
317451
390519
460424
66962
455610
113989
470083
61322
410942
378913
400354
151898
203512
29962
93135
436413
423692
393489
383898
273928
362205
170332
265447
27880

====================
Listening for OBS websocket events
====================
By default OBS websocket sends all the event.
They are just ignored by lioranboard for the most part.
To listen to certain event you just need to edit "listen_obs_event.ini"

You can find all the events right here https://github.com/Palakis/obs-websocket/blob/4.x-current/docs/generated/protocol.md

For exemple if you wanted to check if OBS is still streaming. you'd want the event StreamStatus

In the ini file you just add StreamStatus in the section [listen]
such as X="StreamStatus"
X implying the next number in the list

then you create a section called [StreamStatus]
Under that section you wanna set a trigger, that's just a normal Extension trigger that will happen when the event happen.
such as trigger="obs is streaming"

Event also send some data and you might wanna get that data
For exemple if you wanted to know how well the stream is doing in therm of frame dropped you can look at the variable "strain" in that event
to know this just set this under the section [StreamStatus]
value1="strain"
and then you can do math: trigger pull for Value 1 to get that
You can listen for up to 20 variables, object included.


====================
Did you know?
====================
-You can use the transmitter to test notifications,if you right click the browser source for the transmitter in OBS you can select "Interact"(or run the transmitter in chrome)
	There you will see a few buttons and boxes you can use to test various alerts
	It is highly suggested to use the transmitter as a dock rather than a source. in obs go in View>Dock>Custom browser dock  in the url box put the path file for the transmitter.
	
-LioranBoard comes with a fully functionnal notification animation system for twitch ready to use for OBS,see here what it looks like https://www.youtube.com/watch?v=ilDE_vbM7vs
	To use it just click Install extension in lioranboard, Go to the folder LB notification system included with lioranboard
	Select 'LioranBoard Notification System.lbe', then select the 'tsl_transmitter.html' you are using and follow the steps,
	you will shortly have a full notification system that doesnt relly on 3rd party website to work. Just use the newly created scene as a nested scene(google "nested scenes obs" if you're not sure what that is.)
	Covers Subs,Followers,Bits,raid and host. it even has a TTS option but it requires running the transmitter in chrome instead of browser source.
	
-You can set buttons to triggers on LioranBoard start up and other actions.
	How to do this. Add the "Extension Trigger" to a button and set it to the following.
	!initlioranboard    	for when lioranboard starts up.
	!reinitializing			When decks are reloaded, this happens at same time then !initlioranboard and everytime you click done when saving a deck or moving decks
	!resetlioranboard		for when you click the reset button
	!obsconnected 			for lioranboard first connection to obs, please keep in mind that this will wait for all the data to have been fetched before triggering
	!twitchconnected		for twitch chat first connection
	!transmitterconnected	for the transmitter first connection
	!obsalways				Everytime lioranboard connects to obs
	!twitchalways			Everytime lioranboard connects to twitch
	!transmitteralways		Everytime the transmitter connects to lioranboard
	!transmitterdisconnected	Everytime the transmitter disconnects
	!leavescene Scene Name	Everytime you switch scene, Math: Trigger Pull 1= transition type, 2= transition duration
	!enterscene Scene Name	Everytime you switch scene, Math: Trigger Pull 1= transition type, 2= transition duration
	!ban  					when someone gets banned,  Math: Trigger Pull    1=name of the mod,   2=name of the person who got banned
	!unban  				when someone gets un banned,  Math: Trigger Pull    1=name of the mod,   2=name of the person who got unbanned
	!timeout  				when someone gets banned,  Math: Trigger Pull    1=name of the mod,   2=name of the person who got timed out    3=duration in seconds of the timeout
	!untimedout  			when someone gets un banned,  Math: Trigger Pull    1=name of the mod,   2=name of the person who got untimed out
	!clearchat 				when a mod clears the chat,  Math: Trigger Pull    1=name of the mod,
	
-You can press Tab to toggle the value window in lioranboard main screen
	You can also type letter to search for value
	if the search word is the same as a stack, it will show you the content of the stack.

-You can set the ip to connect to obswebsocket by openning connect.ini file and adding   websocket_ip="127.0.0.1" under [connection]

-With custom packet, if you put "message-id":"6666", you can see the reply from OBS websocket and copypaste it. "666" to simply see the status code as a small alert at the bottom

-You can Change the IP and port that the transmitter connects to by opening it as a txt file and looking for //url for lioranboard

-You can create JavaScript extension using the transmitter to connect lioranboard to basically do anything, look inside the extension folder for more info.

-There is some Built in extension if you use the command "Send to Extension"
	Follower Alert,		Trigger that command once and only once, to turn on follower alert. Add !transmitteralways extension trigger to it(give 2000ms delay to that command)
		When a new follower is detected you will receive an [Extension Trigger] for "Follower Alert" , you can use math: trigger pull 1 to get their name 3 for display name
	Bits Leaderboard,   gets the top 3 leaderboard for bits
		when this you run this command a few values will appear in the value window and [Extension Trigger] for "Bits Leaderboard".
	Change Title/Game 	You can change title or game with this
		You can leave the game or title box blank if you do not wish to change them. putting an invalid game name will result in no games.
	Get Subscriber Amount
		Return the amount of subs you currently have
	Get Channel ID
		to be used with bot account
	Get View Count
		Can get the viewer count of any account
		

-extension won't work if the transmitter isn't connected.

-Do Not put the transmitter inside the same folder as Lioranboard receive.exe,nor a folder inside the exe folder.
	if you do so, installing extension just will not apply.
	
-You can enable DEV mode for extension making by right clicking the Reset button 10 times.
	all this does is reinstall the same extension when clicking the "install extension" button with no assle

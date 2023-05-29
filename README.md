If your here to play ABF, I would instead use ABF: Reboot which is downloadable at https://www.starpixelproductions.com/angrybirds-fight-reboot since it's actually more usable than this (no compiling an APK or IPA yourself), has more working features and even things like events and arena.

# OpenFight
A working ABF 'K side' replacement server that can be used with Apache, open sourced here on github forever to be preserved.


Progress: Partially playable (as playable as having only the 'K side' server will ever be :P)

This project is free to be used in your revivals of the game, and no credit is needed however some would be appreciated :)

If your still here, i'm assuming you want to set up a private server for your own use, excellent!
So let's get into how to, eh?

# How do I use this?

First of all do the standard stuff, port forward the ports 80 and 443, yadayada

1. I recommend you download and setup XAMPP from https://www.apachefriends.org, make sure to use the download for your OS (DO NOT INSTALL IT INTO PROGRAM FILES, VERY IMPORTANT.). (Example: I would use the Windows installer if on any version of windows)
2. Scroll up and click on the green 'Code' button, and then click 'Download ZIP'. This'll start downloading the actual server replacement.
3. Open up the folder where XAMPP installed to (By default it's C:\xampp) and go into the folder called 'htdocs' (or create it if it isn't there).
4. Delete everything in there and replace it with the files and folders inside the folder 'OpenFight-main' in the ZIP file you just downloaded.
5. Open up the XAMPP Control Panel (RUN IT AS AN ADMINISTRATOR) and click on the X in the Apache column to install the Apache service.
6. Click on 'Start' in the Apache row to start up your server. if you go to localhost/login you should see a Status 2000 code. this is good, it means your server works!

# Okay, cool, but how do I edit ABF (Android) to actually use my server and not the dead ones?

1. Get a  copy of ABF version 2.5.6 (unless you're using older versions, but this guide doesn't account for that). (This can be from anywhere tbh, i don't really care what you do)
2. Extract it. (Did you know APK files are basically ZIP files? Cool, huh?)
3. Go into the 'lib' folder, then 'armeabi-v7a' and locate a file called 'libcocos2dcpp.so'.
4. Edit it with your favorite hex editor (I just use notepad++'s hex addon personally, but you do you!)  and find this URL:  https://agbdfgt.kiteretsu3.jp/, BTW its dead so it won't work. (I just use notepad++'s hex addon personally, but you do you!) 
5. Edit it to be your IP, webserver, website, whatever your server is on and if there is any space, put 1 / and as many .'s needed till just before you plow into 'EventMaster.json' (The URL can only be as long or shorter than the original URL, or you plow into already existing code.)
6. Save the SO file, and then use a tool like APK Editor Pro (find it yourself) to replace the original 'libcocos2dcpp.so' file with your newly edited one. Simply compile and boom, you should have a working Fight APK if done right!

# Special Thanks:

Everyone in the Reboot Team for helping with preserving this amazing game

FairPlay137 for creating the original Golang file I based this on

And you, for playing your part in the fight for videogame preservation.

Thank you.

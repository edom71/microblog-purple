general readme file for microblog-purple

Introduction

This is a plug-in for Pidgin to allow for seamless updating and receiving of Twitter messages. While originally built for Pidgin it works for other LibPurple base clients like Adium and Finch. Currently the plug-in works with Twitter only.

So what's the different between this and Twitter IM? The answer is this would be kind of my personal replacement for Twitter IM, since I spent sometimes waiting for the service to come back and don't want to wait anymore. Besides, having it as plug-in give me some liberty to customize it in many ways. Like modifying the message to link to hashtags or twitter user (thanks @chanwit), or the ability to add special command to itself (/refresh, /replies, /etc....). I plan to have this in "Chat mode" instead of normal conversation windows for people who easily annoy with constant incoming messages.

The plug-in is inspired by FacebookChat project

Installation

Linux

Ubuntu

For Ubuntu, please try Awashiro Ikuya's PPA repository

After setting-up PPA repository, Simply install pidgin-microblog.

sudo apt-get install pidgin-microblog

Gentoo

In gentoo simply install microblog-purple using: sudo emerge -v x11-plugins/pidgin-mbpurple

Mac

Assuming Adium is already installed, download the "TwitterIM.AdiumLibpurplePlugin.zip" and unpack. Using Finder, click on the "Twitter.AdiumLibpurplePlugin" icon - MacOS will take it from there.

Building the code

Windows build

Follow Building on Windows HOWTO - make sure you build pidgin successfully
Download microblog-purple source code, untar and place it in your $HOME.
cd microblog-purple-x.x
Edit global.mak, especially the PIDGIN_TREE_TOP variable to match your pidgin source directory.
make && make install
The built dll (libtwitter.dll) will be installed at /win32-install-dir/plugins. All images will be installed there too. Run the new pidgin from win32-install-dir directory and it'll just work. You can copy the generated libtwitter.dll to your normal Pidgin installation directory. Don't forget to also copy all png images to the correct path.
If you want to build windows installer, type make windist instead.
Linux build

You will need to have libpurple and pidgin headers first. For Ubuntu, these are libpurple-dev and pidgin-dev packages
Download microblog-purple source code and untar it somewhere
cd microblob-purple-x.x && make && make install
The executable will be installed in your pidgin plug-in installation dir, detected from pkg-config command. You can also modify variable and path in global.mak
Mac

Make sure you have XCode installed
Download and build the adium source. This will create several of the Frameworks that are required for the plugin
Download the microblog source, placing it in the same parent directory as the adium source (not necessary, but then all the relative links should work automatically).
Go to Project -> Active Target "TwitterIM" and ensure that all build paths are set appropriately for your computer.
Build plugin
to install, just click on "Products" and then TwitterIM.AdiumLibpurplePlugin.
Please note that this plugin is only built and tested for Intel Macs running MacOS 10.5.x.

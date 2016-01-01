# Installing i3 wm on Linux Mint 17.3 cinnamon

We start from an up-to-date Linux Mint 17.3 cinnamon as described on 
http://erikdubois.be


![Screenshots](http://i.imgur.com/l0Ecx5O.png)

# BETA VERSION - Needs to be checked and simplified!!


#Installation procedure

First install Linux Mint 17.3 like you always would.

Then update.

Download and use proprietary drivers if needed.
Broadcom, nvidia, ati and the likes.

Upgrade your kernel if you want to. 

Get that out of the way. 

Do get the code from github. Install git first

	sudo apt-get install git

Then

	git clone https://github.com/erikdubois/i3-on-Linux-Mint-17.3.git

This folder your are downloading is my content of the hidden .i3 directory, where all files will reside.


# step 0


You can copy/paste all of this in the hidden folder of .i3.

You can make a hidden folder in your home folder, if you do not yet have one.

# beware the hidden files !! Copy/paste all files (CTRL + H)


# step 1


Go inside the folder installation/Step_1

Run the script with the highest version number.

You will install:

- i3 basic system
- menu to start programs
- screenfetch to display general info of your computer
- variety for wallpapers
- terminator for terminal - more tweakable
- unclutter to get the mouse out of the way
- zsh - shell with lots of colours and themes
- gimp already installed 
- inkscape - vector drawing
- firefox - already installed
- adobe-flashplugin
- transmission-gtk - for conky aurora
- skype
- hexchat already installed
- vlc already installed
- geary - mail client
- lxappearance - choose icons and themes
- nitrogen - wallpaper
- feh - wallpapers
- qt4-qtconfig - choose icons and themes for qt4
- scrot - caputure picture
- git for github
- htop - analysis processes
- wget - getting files of internet
- curl - getting files of internet
- sensord - read out heat and other sensors
- sysstat - system statistics
- glances - analysis processes
- numlockx - num lock on or off
- inxi - hardware info
- dmidecode - information for conky aurora
- hddtemp - harddisk temperature for conky aurora
- net-tools - network tools
- mlocate - find stuff on your computer anywhere
- hardinfo - graphical way to see all hardware components
- unetbootin - make bootable usb
- extlinux
- vnstat - statistics for network consumption
- screenfetch - hardware info
- kazam - already installed - making movies
- install thunar if you like to batch rename files
- catfish - graphical way to search everything
- gnome-disk-utility - already installed


Do not yet log off and log on into i3.
Or you will see some errors.


# Step 2

Installation of an alternative to the i3 status bar

Go inside the folder installation/Step_2/i3blocks
Start compile-source-code-for-i3blocks.sh in a terminal

Go inside the folder installation/Step_2/font
Install also the font since one of the "letters" is used to make the bottom bar nicer.
Double-click the font and install in linux mint.

Go inside the folder installation/Step_2/dmenu larger font
Read the document and do these steps in a terminal.

Go inside the folder installation/Step_2/j4_dmenu_desktop
Run j4-dmenu-desktop_install.sh
This will provide with a better menu selection.
Activated with WIN + SHIFT + D  - called Linux Mint Desktop
(Normal menu is WIN + D - called  Linux Mint All Programs)

If working with NEMO as file manager you will need to copy paste this line in a terminal or you will open
a desktop together with nemo.

gsettings set org.nemo.desktop show-desktop-icons false


# Change the looks

use lxappearance and qtconfig-qt4 to change icons, themes etc  ...
Restart programs to see the changes.


# Shortcuts to remember

You can set your mod key. I have set mine to the Windows Key

This is windows key
set $mod Mod4

Mod4 + E  = to exit i3 and log back on with Cinnamon
Mod4 + D  = dmenu
Mod4 + SHIFT + D = j4_dmenu
Mod4 + Enter = terminal
Mod4 + SHIFT + Q = end current program

Remember the 10 possible screens in the bottom-left corner.
I have positioned some programs on some specific desktops.

Assign section
assign [class="Firefox"]          → 1
assign [class="sublime-text"]     → 2
assign [class="sublime_text"]     → 2
assign [class="Sublime_text"]     → 2
assign [class="Thunar"]           → 8
assign [class="Nemo"]             → 8
assign [class="Geary"]            → 9
assign [class="Spotify"]          → 10


Mod4 + SHIFT + R = reset or rerun i3 if you change some code in the config file


# Start up programs with ALT + CTRL + ...
mod1 = ALT
bindsym control+mod1+f exec firefox 
bindsym control+mod1+g exec geary
bindsym control+mod1+s exec spotify
bindsym control+mod1+t exec subl
#bindsym control+mod1+b exec thunar
bindsym control+mod1+b exec nemo --no-desktop
bindsym control+mod1+c exec catfish



# You can stop here and log off 
# Log in by clicking the wheel and choosing i3



# Step 3

Optional I3 not from Ubuntu sources but from Github

1/1/2016 Ubuntu/Linux mint 17.3 is at version 4.7.2-1
Githubs version is 4.11 !!!

Some bugs have been fixed and extra features have been added.

Go inside the folder installation/Step_3/i3_upgraden_from_github
Run compile_github_i3.sh


# Step 4

Optional I3 next gap

I have learned of this 'spin-off' and I like the visual aspect of it and I still have enough room on my screens to do the work efficiently.
You can read more on their github site.

https://github.com/Airblader/i3/tree/gaps-next

Go inside the folder installation/Step_x/i3 with gaps


# E N D   R E S U L T

Without gaps

<a target="_blank" href="http://erikdubois.be/wp-content/uploads/2015/05/i3_on_linux_mint_17_1.png">
<img style="max-width:100%;" data-canonical-src="http://erikdubois.be/wp-content/uploads/2015/05/i3_on_linux_mint_17_1.png" alt="alt tag" src="http://erikdubois.be/wp-content/uploads/2015/05/i3_on_linux_mint_17_1.png">
</a>

With gaps

<a target="_blank" href="http://erikdubois.be/wp-content/uploads/2015/05/mintyi3withgaps.png">
<img style="max-width:100%;" data-canonical-src="http://erikdubois.be/wp-content/uploads/2015/05/mintyi3withgaps.png" alt="alt tag" src="http://erikdubois.be/wp-content/uploads/2015/05/mintyi3withgaps.png">
</a>


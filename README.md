# Make your Desktop look like MacOS

Because I keep getting asked about it, here are the instructions how I made my Desktop (Linux Mint Cinnamon) look similar to MacOS. 

> First of all: I never used a Mac longer than testing it. I just like the basic structure of the MacOS 'Desktop', but for me it 's not about getting exactly a MacOS Interface.

## Installing Ulauncher

ULauncher is an application launcher for Linux Systems which is very similar to the one from apple. I install it first on every system because it makes opening apps so much faster.  
The install instructions are very easy understandable and can be found on their Website [ULauncher.io](https://ulauncher.io) . After opening the programm you can set the shortcut and check the 'Launch on startup' box. 

## Installing Themes

I really like the WhiteSur Theme from _vinceliuice_. He designed a GTK-Theme, an Iconpack, and Cursors.

### WhiteSur GTK-Theme

You can easily install The GTK-Theme with the instructions on its [Github-Page](https://github.com/vinceliuice/WhiteSur-gtk-theme). Don't remove the folder yet. We will need it. 

### WhiteSur Iconpack 

Download the `.zip` Files from this [Github-Page](https://github.com/vinceliuice/WhiteSur-icon-theme) and install them the same way you installed the GTK-theme. I like the alternate Version, therefore you use `./install.sh -a`. 

### Cursor Theme

Download the `.zip` Files from this [Github-Page](https://github.com/vinceliuice/McMojave-cursors) and install them the same way you did before. 

### Applying Themes

Apply the themes using the standard `Themes` settings from LM.

## Setting up the Panels

### The Upper Panel

The Upper Bar is just the normal Bar I moved to the top and did the following changes: 

1. Decrease the bar size (right click -> Panel settings -> size)
2. Remove unneeded Applets (right click -> Panel edit mode -> right click on applets to remove them)
   1. LM Menu 
   2. Grouped Window list (your cuurent apps)
   3. App shortcuts
3. Add Applets (right click -> applets)
   1. cinnamenu
   2. weather (if you want)
   3. user (if you want)
4. Customize Cinnamenu
   1. right click on cinnemenu -> Settings -> appearance 
   2. custom icon -> select `start-here`(Apple logo; optional)

### The Lower Panel

#### Installing Plank

For the lower Panel I use `Plank`. You can install it with the command 
`sudo apt install plank` . After installing, open Plank. The plank-panel appears on the bottom of your Desktop. 

#### Setting Up Plank-Theme

Copy the plank themes from your WhiteSur Folder to the plank folder:
`cp -r /PATH/TO/WhiteSur-gtk-theme/src/other/plank/theme-* ~/.local/share/themes/`
Access the plank settings: hold `ctrl` and right-click on the plank panel -> settings and choose the _theme-Dark_ or _theme-light_. 

#### Adding Plank to startup

Add Plank to the apps on startup so it opens automaticaly every login.

## Dynamic Wallpapers

For Apple-like dynamic wallpapers I really like Linux Dynamic Wallpapers from saint-13. There are many high quality wallpapers and you can easily install them with the commands on the [Github-Page](https://github.com/saint-13/Linux_Dynamic_Wallpapers?tab=readme-ov-file).

After installing you can change your Background from the standard LM-Background settings. 
Just add the subfolder `Linux_Dynamic_Wallpapers/Dynamic_Wallpapers` to your Wallpapers. (Where the folder is located depends on where you installed `Linux_Dynamic_Wallpapers`) 

## Terminal

To change the look of my Terminal I use [Gogh](https://github.com/Gogh-Co/Gogh) . You can choose from many themes - I use _catppuccin Latte_ but there are so many - you'll find one you like. 

## Login Screen

I haven't found a way to tweak lightDM to a MacOS-like look yet. Maybe somebody else has? For the moment I just go into the `login-screen` settings, put the user in the middle and change the cursor theme.  

> I hope, my instructions are useful to some of - even if you just use a part of it. If you have questions, feel free to contact me :)

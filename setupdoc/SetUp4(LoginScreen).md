# How to moe-ify the login screen (GDM)

(We will proceed on the assumption that you have already installed the Moe-Pink16 shell theme for moe.)  
Install "Alternatives Configurator (galternatives)" from "gnome-software".  
If you want to install it from a terminal (Ctrl+Alt+T), type the following  

	$ sudo apt install galternatives

* Configuration

Please run galtanatiles.
From the search screen, search for "Alternatives Configurator", navigate to "gdm3-theme.gresource" in the left pane, right click on the empty space on the right and select "New".  
Click "OK" without worrying about the excuse screen that appears.  
When the configuration window opens, specify path to  "gnome-shell-theme.gresource" in "/usr/share/themes/Moe-Pink16/gnome-shell/" that you have installed beforehand. In other words, the path will be as follows (you can copy and paste).  

	/usr/share/themes/Moe-Pink16/gnome-shell/gnome-shell-theme.gresource  

Specify Priority as "20" or something appropriate.  
After finishing the settings, click the "OK" button in the lower right corner to close the screen.  
Now "/usr/share/themes/Moe-Pink16/gnome-shell/gnome-shell-theme.gresource" will be registered in the original screen. With the "●" on the left side selected, press the "Apply" button on the bottom right of the screen.  
You will be asked for authentication, enter your password to authenticate.  
Now log out and you will see that the login screen is now moe.

---

# Change the login logo to the moebuntu logo

Since the login logo is still "ubuntu", we will change it to the moebuntu logo. Replace "/usr/share/themes/Moe-Pink16/ubuntu-logo.png" in "MoePinkShell5" with "/usr/share/plymouth/ubuntu-logo.png". You will need administrator privileges to operate it, so you can do it manually by opening a terminal (Ctrl+Alt+T) and typing the following to apply it. (Do not include the $)  

	$ sudo nautilus /usr/share/themes/MoePinkShell5/

Replace the above "ubuntu-logo.png" with the following "/usr/share/plymouth/ubuntu-logo.png". Make a backup if necessary.  

---

# Changing the login background image

The login background image is specified as "/usr/share/themes/Moe-Pink16/gnome-shell/moebuntu_bg.png", so just rename the background image of your choice to "moebuntu_bg.png" and replace it with the same file. This is the background image.  
Now, when you log out, you can see how the background image has been changed.


# Moe-ification procedure (GUI)

1.Unzip the above downloaded desktop theme "Moe-(color)15BH" and Shell theme "Moe-(color)Shell5" (from right mouse click) and put them in "/usr/share/themes/". You need administrator privileges to operate it, so open a terminal (Ctrl+Alt+T) and type the following to apply it. (do not include the $)  

	$ sudo nautilus /usr/share/themes/
  
Unzip the icon theme "MoePinkIcons" in the same way, and put it in "/usr/share/icons/".  

	$ sudo nautilus /usr/share/icons/

* You can also create a hidden folder ".icons" in your home folder and put the icon theme "MoePinkIcons" in it.  
In this case, the icons of the files in Nautilus opened with administrator privileges "$ sudo nautilus" will be the default (Adwaita) ones, which are not moe-ified.

---
Of course, you can also use "sudo cp..." to copy the files as well.
  
# Settings in GNOME Tweaks

After completing the above preparations, launch GNOME Tweaks, open the Appearance tab, and configure the following settings.  

(1) Go to Appearance > Applications > Moe (Color) BH  

(2) Go to Appearance > Icons > MoePinkIcons  

(3) Go to "Appearance" > "Gnome Shell" > "Moe (Color) Shell5".  

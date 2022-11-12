# Moe-ization procedure (GUI)

## 1. Download and install the theme
Download the theme "moe-(color) 16.tar.gz" for each color in the above Theme(Window+Shell,9colors). (Please choose your favorite color). Unzip it (from right mouse click) and place it in "/usr/share/themes/". The operation requires administrator privileges, so open a terminal (Ctrl+Alt+T) and type the following to apply. (do not include the $)  

	$ sudo nautilus /usr/share/themes/ 

and drop it in the window, it will be easy.

## 2. Download and install icon theme

Download and extract the icon theme "MoePinkIcons_2011117.tar.xz" in the same way and place it in "/usr/share/icons/".  

	$ sudo nautilus /usr/share/icons/ 

and drop it into the window.

* You can also create a hidden folder ".icons" in your home folder and put the icon theme "MoePinkIcons" in it. 
In this case, the icons of files in Nautilus opened with "$ sudo nautilus" with administrator privileges will be the default (Adwaita) ones that are not moe-ized.

* Of course, it is possible to copy files with "sudo cp... You can also copy files with "sudo cp...".

---

# Configuration in GNOME Tweaks

After completing the above preparations, launch GNOME Tweaks, open the "Appearance" tab, and make the following settings 


(1) Select "Appearance" -> "Icons" -> "MoePinkIcons".

(2) Select "Appearance" > "Gnome Shell" > "Moe-(Color) 16".

(3) Select "Appearance" > "Legacy Applications" > "Moe-(Color) 16". 

---

## Moeing Qt apps (turning them color)

You can moe Qt5-based apps such as VLC and QuiteRSS.
Just open a terminal (Ctrl+Alt+T) and type the following to apply. (do not include the $)

    $ sudo apt install qt5-style-plugins
    $ echo "export QT_QPA_PLATFORMTHEME=gtk2" >> ~/.profile

# Configure the startup screen (Plymouth)
We will use "Alternatives Configurator (galternatives)" for the configuration, see SetUp4(LoginScreen).md for installation.  
Download "mmspinner.tar.xz" and put the contents into "/usr/share/plymouth/themes" to complete the preparation. You must have administrator privileges to operate it. Open a terminal (Ctrl+Alt+T) and type the following to operate the file.  

	$ sudo nautilus /usr/share/plymouth/themes/

* Configuration

The procedure is almost the same as the previous login screen. From the search screen, search for "Alternatives Configurator"and run, navigate to "default.plymouth" in the left pane, and right-click "New" in the empty space on the right.  
Press "OK" without worrying about the following confirmation window.  
When the configuration window opens, specify the file "mmspinner.plymouth" in "/usr/share/plymouth/themes/mmspinner" that you have previously installed. In other words, the path will be as follows (copy and paste is fine).  

	/usr/share/plymouth/themes/mmspinner/mmspinner.plymouth

Specify the Priority as "20" or something appropriate.  
After finishing the settings, click the "OK" button in the lower right corner to close the screen.  
This will register "/usr/share/plymouth/themes/mmspinner/mmspinner.plymouth" in the original screen, so click the "●" button on the far left.  
There is an "Apply" button at the bottom right of the screen, click it.  
When the authentication request screen appears, enter your password to authenticate.  
The position of the "●" button on the far left has changed to the newly registered mmspinner.plymouth.  
Now, open a terminal (Ctrl+Alt+T) and type the following command.  

	$ sudo update-initramfs -u -k all

You are now done. After rebooting, you can see that you are now at the startup screen shown at the beginning.  

---


# Change the background image
If you want to change the background image, first rename your favorite image to "background-tile.png" in the following location and replace it.  
You must have administrative privileges to do this.  

	/usr/share/plymouth/themes/mmspinner/background-tile.png

Since the image is set to be lined up in a tile pattern, use GIMP to adjust the image to fit the size of your screen or prepare a tile image.
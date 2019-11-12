# transparent-xcursor-linux

This cursor theme allows the user to have invisible cursor for raspberry pi, for use of touch screens. This is done by generating a trasnparent set of cursor icons using xcursorgen. 

You do not need to follow the steps to generate from source, you can simply copy from the cursors folder to your cursor themes folder.

All is explained below, using raspbian buster.

On Raspbian

1) Preferences -> Main Menu Editor -> Preferences  - Radio Button (Theme and Appearance Settings)

2) 

    a) You can just use the cursors i have provided, only do step a, b is for reference.
       Navigate to "/usr/share/icons/Adwaita" and delete the folder "cursors"
       Obtain the folder from the download "xcursor-transparent-cursor-master" and copy "cursors" folder to "/usr/share/icons/Adwaita" 


    b) If you want to generate cursors from scratch, which you shouldn't
       In Terminal run "sudo apt-get install x11-apps" we require xcursorgen if doing this from scratch. 
       Then in the folder "xcursor-transparent-cursor-master" run the script gen.sh with bash

3) Navigate to Preferences -> Theme and Appearance Settings -> Mouser Cursor - On the left hand side click "Adwaita" and click apply

4) Reboot and now cursor should be transparent. If you ever want to re-enable must go through step 3 and change to "PiXflat"

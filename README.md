The following is an unofficial and simplified guide to get started on custom Steam Skins(btw I use vim).

Let's get started:
=======================
-Copy the "steam.styles" file from /resource/styles  ((in Linux it's under /home/username/.steam/resource/styles/ )) to your pre-existing "skins" folder

-Make new folders as need to create the path "/skins/SomeSkin/resource/styles/" where "SomeSkin" is your chosen name for the custom skin.

-Move the "steam.styles" file to /skins/..../styles/

-Rename it to avoid confusion.  Try SomeSkin.styles .

-Make a copy to fallback to in case you mess up. Call it SomeSkin.styles.bak
***To use the backup, delete the edit SomeSkin- then make a copy of the .bak as "SomeSkin.styles".  In Linux ( rm SomeSkin.styles && cp SomeSkin.styles.bak SomeSkin.styles ).

=======================
First Test Edit:
=======================
-open SomeSkin.styles in your text editor of choice(btw i use vim)
-Find the entry 'Text="' which should be about the 7th paragraph or line 58
-change the numbers in between the "  " to a color(blue);
-do the same for "TextGlowHover" and "TextGlowSelected"
-save file and close

=======================
Fruits of Labor:
=======================
-Shutdown Steam completely.  In Linux, you can type in your terminal "sudo pkill -9000 steam"

-Relaunch steam

-At the top-left, go to "Steam" > "Settings" > "Interface"(above Downloads)

-Click on the third drop-list from the top, under "Select the skin you wish Steam to use (requires Steam to restart)"

-Move mouse down to desired skin and click "Ok" and repeat Steps 1,2.

=======================
Adanaced(further):
=======================
-Restart Steam in Developer Mode.  In Linux, type "steam -dev"

-Go to a page you would like to see edited. -Hit "F6" to open a window called "vgui layout debugger"

-Examine the code and take note of its properties.

-Go back to your style file; having made a backup of your already-working style, continue to modify it as desired.

-Save style; Close steam; relaunch;

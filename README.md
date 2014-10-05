SETBACKLIGHT
============

 A simple program to adjust screen brightness

How to compile:
----------------
 `$ gcc  set-backlight.c -o set-backlight`

How to install:
----------------
 `# mv set-backlight /usr/local/bin`
 
 `# chown root /usr/local/bin/set-backlight`
 
 `# chmod u+s /usr/local/bin/set-backlight`

How to use:
------------
 `Usage: set-backlight [OPTION]`
 
` OPTION can be one of these:`

` VALUE  An integer between 0 and MAX_BRI( integer, hardware dependent )`

` --increase Increase the screen brightness by ( MAX_BRI - 0 ) / 10 ( an integer )`

` --decrease Decrease the screen brightness by ( MAX_BRI - 0 ) / 10 ( an integer )`

` max        Set the screen brightness to max ( hardware dependet )`

` med        Set the screnn brightness to med ( (max - min ) / 2 )`

` min        Set the screen brightness to min  ( hardcoded, default: 0 )`


 ----------------------------------------------------------------------------------
`The program will try to detect the the MAX_BRI value atomatically.`

`If it fails on doing so, try to hardcode the correct value for your screen.`


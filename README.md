# ScreenFlickerFixer
A script that refreshes display configuration, this fixes screen flicker in many situations.   Works best when bound to a hotkey or triggered by a device such as the Elgato Stream Deck.  This is all possible using Timothy Mui's code (https://github.com/timmui) 


 ## This script is just a specific configuration of Timothy Mui's Set-ScreenResolutionEx.ps1 script. It can be used to fix screen flicker which is common on windows machines using multiple displays.  
 ## The way this script works to fix screen flicker is to quickly hop away from the current resolution and then back to the desired resolution for all connected displays: 
 ## Possible use case are running this as a login script or binding the script to a hotkey using another utility (I use the Elgato Streamdeck).  
 
 #  how do I set it up for my computer?
 -  The bottom of this script contains sample configuration for a three monitor setup which happens to be the exact configuration that I use.
 -  To setup for your purposes, change the first resolution of each display at the bottom of this script to something other than your desired resolution, then change the second resolution of each to the desired resolution
 
 ## If you have one display, then you only need lines containing -deviceid 0  , two displays? then use  -deviceid 0 and -deviceid 1  , and so on. 

 ## For example: if you use two monitors, starting at line 288, comment out or delete the lines with -deviceid 2 and make sure the final resolutions for devices 0 and 1 are your desired (or current) resolution, then run the script.  If you don't see an improvement, try different "false resolutions"
 

 #######################################################################################################
 
 #Timothy Mui's code is below which we will use to set the screen resolutions. Both he and Andy Schneider deserve acknowledgement and thanks for their work creating the resolution script.

 #######################################################################################################

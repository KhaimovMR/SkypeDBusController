Skype-DBus-Controller
=====================

Make it easy to control your Skype through a shell commands in your Linux system. 


====================

HOW TO USE:

By binding a hotkey to a run of this utility with your desired parameters 
(in Ubuntu it's: System settings -> Keyboard -> Shortcuts -> Custom shortcuts) you
can much more easily control your Skype.

To control Skype over this utility, Skype should be launched with DBus support. 
In 4+ version of Skype this option are turned on by default. In older versions
you should run Skype with parameter, described in skype help page (you can run 
'skype --help' in shell, to find out which one). 
 
If Skype are already running with DBus support, then just run skypedbuscontrol.py
with an appropriate parameter.

LIST OF PARAMETERS:

show <login>      - shows/hides Skype's Contacts window. <login> is your
                    skype login, that usually prefixes Contacts window.

recent            - shows a window with recently participated chat

missed            - opens a window with first missed message

pick-up           - picks up an incoming call

hang-up           - hangs up all incoming calls (including calls on the hold)

manual-mode       - lets you manually send a DBus command to a running Skype process

EXAMPLES:
- To run script from it's custom directory
    ./skypedbuscontrol.py recent
- To run script when it's already in the /usr/bin/ or ~/bin/ directory
    skypedbuscontrol.py pick-up
    skypedbuscontrol.py show myskypelogin

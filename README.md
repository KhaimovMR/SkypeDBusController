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

showContacts <login>    - shows/hides Skype's Contacts window. <login> is your
                          skype login, that usually prefixes Contacts window.

recentChat              - shows a window with recently participated chat

firstMissedChat         - opens a window with first missed message

pickUp                  - picks up an incoming call

hangUpAll               - hangs up all incoming calls (including calls on the hold)

manualMode              - lets you manually send a DBus command to a running Skype process

EXAMPLES:
- To run script from it's custom directory
    ./skypedbuscontrol.py recentChat
- To run script when it's already in the /usr/bin/ or ~/bin/ directory
    skypedbuscontrol.py pickUp
    skypedbuscontrol.py showContacts myskypelogin

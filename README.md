# wti-nps-230-control-software-for-windows
control software for wti nps-230 remote power switch written in hta and vbscript


SERIAL COMMUNICATIONS PORT = COM2
software is made for controlling wti nps-230 or nps115 trouht serial port may also work on some other models on startup this software sends enter on serial port so wti network power switch can receive commands when button is pressed software sends /ON (1-8) or /OFF (1-8) from serial port to network power switch

---------------IMPORTANT--------------------                                                                                        
When using this software to control the network power switch you must go to the network power switch settings
and change comand confirmation to off, this setting can be found in menu by typing /G and then pressing 8
to go into command confirmation setting and set it to off the software does not work if you dont change this setting

-------------Communications port------------                                                                                      
Go to device manager and open ports com&lpo drop down menu, select your serial device from the list, double click on it or right click and select properties in properties go to port settings, and click on advanced, at the lower part of advanced screen click on "com port number" and select com2 if your computer says "this com is being used by other device" click yes, this will override the com2 to the com port you are using to connect to the network power switch

com port can also be changed by going into every bat that as label ON1 to ON8 and OFF1 to OFF8 and changing com2 to something else like com1 or com3 do not change anything in startup.bat or startup.txt they are used for sending enter into serial for


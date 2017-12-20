# Ethernet_SS_Mod
Modified Arduino Ethernet/w5100 library to support user defined slave select pin

I have a project using a Moteino radio and Ethernet shield, but they both use D10 for the Slave Select.  
SurferTim modified the Ethernet and w5100 Libraries to support a different slave delect pin.
See Arduino forum post: http://forum.arduino.cc/index.php?topic=217423.msg1601862#msg1601862
Originally SurferTim modified ethernet.cpp/.h and w5100.cpp/.h  
Then kiwisincebirth made the change so just w5100 files were modified, Ethernet.cpp/.h are unchanged
See his github repo here: https://github.com/kiwisincebirth/Arduino/tree/master/Ethernet
You can see kiwisincebirth changes here:
w5100.h: https://www.diffchecker.com/yOjNtCLj
w5100.cpp: https://www.diffchecker.com/Mwk773IT

To use, w5100.h and w5100.cpp files need to be replaced with the updated files.

The w5100.cpp and .h files are located
Windows: C:\Program Files(x86)\Arduino\libraries\Ethernet\utility\
Mac: /Applications/Arduino.app > show pkg contents > /Contents/Resources/Java/libraries/Ethernet/src/utility/

Arduino made some changes to w5100 library from v1.5.8 to 1.6.6. Changes are shown here:
w5100.h changes: https://www.diffchecker.com/0eUuANWW
w5100.cpp changes: https://www.diffchecker.com/MraUAw03

Arduino made some minor changes from 1.6.6 to 1.8.4, mostly changing the name of some constants. You can see those changes here:
w5100.h: https://www.diffchecker.com/RZSHJdTH
w5100.cpp: https://www.diffchecker.com/WDdLcEgv

I took the w5100 v1.8.4 files and applied kiwisincebirth's changes so the slave select feature would work



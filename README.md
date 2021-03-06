# Ethernet_SS_Mod
Modified Arduino Ethernet/w5100 library to support user defined slave select pin

I have a project using a Moteino radio and Ethernet shield, but they both use D10 for the Slave Select.  
SurferTim modified the Ethernet and w5100 Libraries to support a different slave delect pin.
See Arduino forum post: http://forum.arduino.cc/index.php?topic=217423.msg1601862#msg1601862
Originally SurferTim modified ethernet.cpp/.h and w5100.cpp/.h  
Then kiwisincebirth made the change so just w5100 files were modified, Ethernet.cpp/.h are unchanged.  
See his github repo here: https://github.com/kiwisincebirth/Arduino/tree/master/Ethernet  
You can see kiwisincebirth changes here:  
w5100.h: https://www.diffchecker.com/yOjNtCLj  
w5100.cpp: https://www.diffchecker.com/Mwk773IT  

To use, w5100.h and w5100.cpp files need to be replaced with the updated files.  

The w5100.cpp and .h files are located  
Windows: C:\Program Files(x86)\Arduino\libraries\Ethernet\utility\  
Mac: /Applications/Arduino.app > show pkg contents > /Contents/Resources/Java/libraries/Ethernet/src/utility/  

Arduino made some changes to Ethernet/w5100 libraries from v1.5.8 to 1.6.6. Changes are shown here:  
w5100.h changes: https://www.diffchecker.com/0eUuANWW  
w5100.cpp changes: https://www.diffchecker.com/MraUAw03  
Ethernet.h changes: https://www.diffchecker.com/Rm37U5zK  (added timeout)  
Ethernet.cpp changes: https://www.diffchecker.com/C5Vfr5lm  (added timeout)

Arduino made some minor changes from w5100 1.6.6 to 1.8.4 (no changes to Ethernet.h/cpp files), mostly changing the name of some constants. You can see those changes here:  
w5100.h: https://www.diffchecker.com/RZSHJdTH  
w5100.cpp: https://www.diffchecker.com/WDdLcEgv  

Here are the changes SurferTim made to the 1.5.8 version of the files:  
Ethernet.h https://www.diffchecker.com/V9PzVlbb  
Ethernet.cpp https://www.diffchecker.com/lTf9IvhC  
w5100.h https://www.diffchecker.com/qFhgWXbQ  
w5100.cpp https://www.diffchecker.com/goLkR0sG  

Here are the changes kiwisincebirth made to the 1.5.8 version of the files:  
w5100.h: https://www.diffchecker.com/Ysg0yhn1  
w5100.cpp: https://www.diffchecker.com/klUSxCVV  



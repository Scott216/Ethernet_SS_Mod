kiwisincebirth made slave select changes so only the w5100.h/cpp files had to be modified.  
I modified his changes a bit so the new slave select code didn't run for every board.  

kiwisincebirth's GitHub repo is here: https://github.com/kiwisincebirth/Arduino/tree/master/Ethernet  

**Usage:** There are two changes you need to make in your code

1. Include W5100.h Typically done when the Include of Ethernet is defined.

```
  #include <Ethernet.h>
  #include <utility/W5100.h> // <- Add this line of code
```

2. Call select(pinNumber) prior to calling the Ethernet begin() method.

```
  W5100.select(8); // <- Specify the SS Pin to use for Ethernet
  Ethernet.begin(mac,ipAddress); 
```

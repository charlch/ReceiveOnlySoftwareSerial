# ReceiveOnlySoftwareSerial

## Disclaimer:

I can take no credit for this code, just copied from https://forum.arduino.cc/index.php?topic=240741.0


```
#include <ReceiveOnlySoftwareSerial.h>

ReceiveOnlySoftwareSerial mySerial (3);  // Rx pin

void setup ()
{
  mySerial.begin(115200);
}

int incomingByte = 0;

void loop ()
{
  if (mySerial.available()) {
    incomingByte = mySerial.read();
	
	# Do something with bytes...
	
  }
}
```
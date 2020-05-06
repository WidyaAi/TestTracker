# Guide to Test
## Preparing Firmware

Go to use **[Test Firmware](https://github.com/WidyaAi/TestTracker/releases)** download this firmware at realese of this repo
![examples](/docs/release.png)

Go to **[Teensy Loader](https://www.pjrc.com/teensy/loader.html)** to install downloader tool and choose according to the OS on your PC

Operating System|Step                                                             |
----------------|-----------------------------------------------------------------|
Windows         |[Steps for Windos](https://www.pjrc.com/teensy/loader_win10.html)|
Linux           |[Steps for Linux](https://www.pjrc.com/teensy/loader_linux.html) |
MacOs           |[Steps for Mac OS](https://www.pjrc.com/teensy/loader_mac.html)  |

It's time to embed the test system.

1. Install **Key Programmer** to device as shown below : 

![examples](/docs/install_key.jpg)

2. Connect device to PC using microUSB connector as shown below

![examples](/docs/connect_to_pc.jpg)

3. Open **Teensy Loader** application, and open hex file by press "open Hex File" as shown in the red box below 

![examples](/docs/teensyloader.png)

4. It will appear like this, and select the hex file "MatadorMy.ino.hex" 

![examples](/docs/select_hex_file.png)

5. It should appear that the hex file will be embedded, as shown below :

![examples](/docs/teensyloader_1.png)

6. Press the button on the key programmer and wait a minute and finish

![examples](/docs/press_button.jpg)

## Testing will start if the power is between 12 to 24 volts.

> If there is a tone of sound 3 times and a half second interval, then it is a sign of failure. The device must be given a voltage between 12 volts to 24 volts.

> However, if there is no failure, it will sound a complicated tone and start the test iteration.

## Test iteration started from 1 tone until 6 tones.

Total Tone    | Indicator Means
------------- | -------------
1             | Control Power at Super Capacitor's Voltage
2             | Voltage at 3 wires (yellow, green, blue)
3             | Storage Disk Card
4             | Celluler
5             | GPS
6             | IMU

### Control Power at Super Capacitor's Voltage

> In this iteration the test usually lasts for 1 minute less, if it fails usually the tone will sound once and try again

Statement | Indicator
----------| ----------
Succed    | Led blinks 10 times quickly
Failed    | Led lights on and on for one time periodically
Reset     | You can repeat by following **[this tutorial](/README.md#repeat-testing)**.

### Voltage at 3 wires (yellow, green, blue)

> To test it, you have to install these 3 wire to 12 Volts or install each of these wire to the red wire

Statement | Indicator
----------| ----------
Succed    | Led blinks 10 times quickly
Failed    | Led lights on and on for two times periodically
Reset     | You can repeat by following **[this tutorial](/README.md#repeat-testing)**.

### Storage Disk Card

Statement | Indicator
----------| ----------
Succed    | Led blinks 10 times quickly
Failed    | Led lights on and on for 3 times periodically
Reset     | You can repeat by following **[this tutorial](/README.md#repeat-testing)**.

### Celluler

Statement | Indicator
----------| ----------
Succed    | Led blinks 10 times quickly
Failed    | Led lights on and on for 4 times periodically
Reset     | You can repeat by following **[this tutorial](/README.md#repeat-testing)**.

### GPS

Statement | Indicator
----------| ----------
Succed    | Led blinks 10 times quickly
Failed    | Led lights on and on for 5 times periodically
Reset     | You can repeat by following **[this tutorial](/README.md#repeat-testing)**.

### IMU

Statement | Indicator
----------| ----------
Succed    | Led blinks 10 times quickly
Failed    | Led lights on and on for 6 times periodically
Reset     | You can repeat by following **[this tutorial](/README.md#repeat-testing)**.

### Done
> if this test is complete and successful, then the LED will blink continuously and no sound.
> if you want to repeat it, you just need to turn the power supply to a voltage below 12 volts and raise it again between 12-24 volts

## Repeat Testing
if you want to repeat the test, then you can do it by giving a power voltage below 12 volts or you break it for 1 second and return it to between 12-24 volts again.

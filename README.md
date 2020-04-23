# Guide to Test
## Preparing Firmware
Go to Use **[Test Firmware](https://github.com/WidyaAi/TestTracker/releases)** download this firmware at realese of this repo
![examples](/docs/release.png)

## Testing will start if the power is not between 12 to 24 volts.

If there is a tone of sound 3 times and a half second interval, then it is a sign of failure. The device must be given a voltage between 12 volts to 24 volts.

However, if there is no failure, it will sound a complicated tone and start the test iteration.

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
### Voltage at 3 wires (yellow, green, blue)
### Storage Disk Card
### Celluler
### GPS
### IMU

## Repeat Testing
if you want to repeat the test, then you can do it by giving a power voltage below 12 volts or you break it for 1 second and return it to between 12-24 volts again.
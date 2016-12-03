This app allows you to change mock location from terminal using adb in order to test GPS on real devices.

Usage:
```batch
adb [-s <specific device>] shell am broadcast -a send.mock [-e lat<latitude>] [-e lon <longitude>]
        [-e alt <altitude>] [-e accurate <accurate>]
```

```batch
adb  shell am broadcast -a stop.mock
```

Example:
```batch
adb  shell am broadcast -a send.mock -e lat 15.3 -e lon 99
```

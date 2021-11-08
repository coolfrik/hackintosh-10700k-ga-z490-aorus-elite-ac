# hackintosh-10700k-ga-z490-aorus-elite-ac

**OpenCore 0.6.9** + **macOS Big Sur**

## hardware
- i7 10700k
- gigabyte z490 elite ac
- 2x16Gb hyperx
- nvme samsung 970 evo 1tb

## not worked
- wifi system board
- Usb keyboard and mouse (bluetooth apple magic keyboard and trackpad works fine).
If remove/disable: AirportItlwm.kext, itlwm.kext, IntelBluetoothFirmware.kext, IntelBluetoothInjector.kext, usb keyboard and mouse work fine. (need usb mapping)

## etc
in config.plist need write your settings values (tag #your): mlb, serialnumber, uuid.
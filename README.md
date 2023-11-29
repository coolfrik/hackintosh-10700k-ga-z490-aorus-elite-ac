# hackintosh-10700k-ga-z490-aorus-elite-ac

Last update: **OpenCore 0.9.6** + **macOS Sonoma 14.1.1**

## history
See releases. 

After update from OpenCore 0.8.4 -> 0.9.6:
- change iGPU to radeon 5700, but iGPU work successufy with some changes in config.plist:
  - if you need iGPU: remove some radeon kext's + change boot args (  -wegnoigpu agdpmod=pikera ) + (PciRoot(0x0)/Pci(0x2,0x0)) and e.t.c
   (compare config.plist from 0.8.4 release).
- change iMac20,1 to iMacPro1,1 in config.plist and USBMap.kext/Contents/Info.plist (only for radeon);
- 'revpatch=sbvmm' need for update to sonoma 14.1.1. Your can remove it and RestrictEvents.kext;


## hardware
- i7 10700k + iGPU
- amd radeon 5700
- gigabyte z490 elite ac
- 2x16Gb hyperx
- nvme samsung 970 evo 1tb

## files
- see EFI in releases
- in config.plist need write your settings values (tag #your): mlb, serialnumber, uuid.

## etc
- wifi, apple magic keyboard, touchpad, mouse work fine.
- wifi used with HeliPort.app and launch at system startup.

# Hackintosh HP 840 G3 Opencore Monterey
* Opencore EFI for HP 840 G3 running Monterey
## Credits
InsanelyMac - Miliuco  
OSXLatitude - Jake Lo

## Changes
27102021
- Updated to OC 0.7.5 and latest kexts

10092021
- Updated to OC 0.7.3 and latest kexts

![Screenshot](https://github.com/yahgoo/Hackintosh-HP-840-G3-Opencore-Monterey/blob/main/img/dualOSon840G3.png)

## Working
- Full graphics acceleration on Intel HD520 iGPU, including brightness control (F5 and F6)
- Multi-display with DisplayPort OOB, VGA 
- Audio, microphone input and headset output (F8 and F9) - Mute button not working
- GigEthernet LAN connection
- Wireless and bluetooth with any compatible card (a DW1560 in my case, no Whitelisting)
left and right USB ports including USB Type-C
- Integrated webcam (OOB)
- CPU power management
- Sleep (Lid, Energy Saver settings, Apple menu, PWR button) & wake (Lid, PWR button)
- Battery management
- Keyboard and touchpad
- Keyboard backlight (Fn + F3)
- Touchpad including tap-to-click, scrolling, mouse buttons (can be disable with prt scr key)

![Screenshot](https://github.com/yahgoo/Hackintosh-HP-840-G3-Opencore-Monterey/blob/main/img/macOS%20Monterey%20with%20Purple%20iPad%20Mini%206.png)

## Set bios settings as follows:
Advanced tab:
Boot options:  
- Fast Boot = Disabled
- Network (PXE) Boot = Disabled  
Secure Boot Configuration:
- "Legacy Support Enable and Secure Boot Disable"  
System Options:
- Virtualization Technology (VTx) = Disabled (recommended, Enable also worked)
- Virtualization Technology for Direct I/O (VTd) = Disabled (recommended, Enable also worked)
Built-In Device Options:  
- Wake On LAN = Disabled
- Video memory size = 64 MB
- LAN/WLAN Auto Switching = Disabled
- Fingerprint Device = Disabled
Power Management Options:  
- Extended Idle Power States = Disabled
- Deep sleep = You can keep this enabled
- Wake when Lid is Opened = Enabled
- Wake on USB = Disabled

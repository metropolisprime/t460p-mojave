# Thinkpad T460P - 10.14.2
![](https://github.com/metropolisprime/t460p-mojave/blob/master/Screen%20Shot%202019-03-24%20at%2011.02.15%20AM.png)
![](https://github.com/metropolisprime/t460p-mojave/blob/master/Screen%20Shot%202019-03-24%20at%2011.01.31%20AM.png)


## Summary
This build works but is very much a work in progress, and very much a YMMV. Most features are currently working: 
 - Audio
 - Sleep / Wake
 - USB (somewhat, not 100% sure if USB speeds are correct, have not tested)
 - HDMI
 - Trackpad (only somewhat, see notes below)
 - WiFi (using an external USB wifi card)

Here's what is not currently working:
 - Brightness Control (tried to use the BrightnessFixup kext to try and get working brightness control, but kept running into problems with Sleep / Boot, so currently using static brightness using AddPNLF patch in Clover)
 - Trackpoint as well as top buttons on Trackpad
 - Webcam (currently showing as disconnected in photobooth, very likely that USB port mapping is incorrect)
 - Gestures

Here are some currently open questions:
 - CPU timing (not 100% sure if these are currently accurate, may need some additional tweaks)

## Build Info
 Info about my machine is below:
 - Intel Core i5-6440HQ
 - WQHD display (2560 x 1440)
 - Intel 530 Graphics
 - 16GB DDR4 ram
 - Two SSD hard drives (OSX installed on main 500gb SSD, Win10 installed on 256gb HD M.2 slot)

## Install
 UUIDs will need to be generated for this machine, as I have removed them from the `config`.
 Kexts are here in the Other folder but I have installed them in `Library/Extensions` and cleared kextcache.

## Support
 Unfortunately, there's really not much support I can provide here, as I've been hacking my way through getting this working. YMMV. Providing this repo as a work-in-progress starting point -- PRs very welcome for those with same / similar machines, or cleaning updates. There are likely kexts installed that are unnecessary, as well as ACPI patches that are unnecessary / wrong at this point.

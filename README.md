# Pico Held 2 hardware resources

This site is all about the Pico Held 2's hardware: schematics, 3D design files, gerber files for PCB production, component specifications and so on.

DISCLAIMER: This is a DIY project. Do it at your own risk. I cannot be held responsible for anything that goes wrong, including design errors. I'm not doing this for profit – I'm just a guy sharing a hobby project.

## Obtaining the hardware as a kit

It's probably the cheapest solution if you buy everything as a bundle from me. I bought them in bulk to save on shipping costs. I sell a "kit" on eBay. It contains the mainboard (including the MCU), shoulder button PCBs, LCD, rubber pads, screws, speaker. However, you will still need the 3D-printed parts (case, start/select buttons, and shoulder buttons), the SNES buttons, the analog stick and the battery.
Since I'm not running a business and don't intend to, if you want to buy a kit, drop me an email (daniel.kammer@web.de) and I'll create an offer on eBay and send you the link (if I can ship to your country that is). The kit costs around 80 Euros.

## Notes on assembly

You can find an assembly video [here](https://www.youtube.com/watch?v=lgt-NjA-OhY).

Please watch the video to see if you are able to do it before making any purchases. Unfortunately, I cannot be held responsible if anything goes wrong. I'm not doing this for profit; I'm just a guy sharing a hobby project.

### parts

If you want to buy everything by yourself, you can find info/links about the parts here:

[LCD](https://aliexpress.com/item/1005007751423312.html) (ESP32-P4)

[LCD](https://aliexpress.com/item/1005008256444774.html) (RP2350)

[Speaker](https://aliexpress.com/item/1005004431389186.html)

For all other parts, see parts.txt in the assembly folder.

All parts for the PCB assembly can be found in the BOM lists in the pcb subfolder.

### 3D case

The 3D printed case features holding brackets for the LCD, holding the LCD tightly in place. Since the overall height has increased, you need to fiddle around a little bit with the rubber pads of the buttons (since the buttons are still the same height). You'll probably get the best results if you glue the rubber pads to the buttons so they won't slip. Tolerances are sometimes off, so using sandpaper may be necessary. There are threaded inserts for the screws required that you'll have to hammer innto the case. I can provide these in the kit, just let me know.
Using the printed version is at your own risk - I just do not have the resources to test is as thoroghly as I did with aluminum case. Since I did all the optimization for the aluminum shell, however, find the platic case to be more comfotable since it's a little thicker

## Software

For quick testing, the repos usually contain a folder called 'artifacts', which contains a file ready to be uploaded to the device.

### Flashing

To enter bootloader mode on both versions, do the following: Press SELECT (left key), then hold down START (right key). You can then release SELECT, but you need to keep START pressed. Releasing the START button will shut down the device and interrupt any ongoing data upload.
If anything goes wrong, you can always press the reset button (located behind the tiny hole on the bottom of the device) and start again.

### RP2350 version

[SNES emulator](https://github.com/fcipaq/picoheld2_rp2350_snes9x)

[Hardware engine](https://github.com/fcipaq/picoengine) (to create your own projects)

### ESP32-P4 version

[SNES emulator](https://github.com/fcipaq/snes9x_esp32)

[Quake](https://github.com/fcipaq/esp32-quake-p2)

[Retro-Go](https://github.com/fcipaq/esp32-quake-p2) (various retro emulators, WIP)




# espusb-macOS
I managed to get cnlohr's espusb built on my macOS 10.14 machine and thought I would share my success.

Not really trying to provide a whole lot of support for this because it was pretty black magic but will do my best to help where possible.

## How to use

Just clone this repo and run the following commands to help with dependency resolving.

```
cd espusb-macOS
ln -s esp-open-sdk/xtensa-lx106-elf/lib/gcc/xtensa-lx106-elf/4.8.2 esp-open-sdk/xtensa-lx106-elf/lib/gcc/xtensa-lx106-elf/4.8.5 
```

Follow the instructions for building https://github.com/cnlohr/espusb . When setting your paths in `user.cfg` point to the directories in this repo and cross your fingers.


## Thanks

I got this working after fumbling around a bunch and finally managing to stick the right pieces together for a build to succeed. I'd like to thank https://github.com/Yveaux/esp8266-Arduino/tree/master/esp8266com/esp8266/tools/macosx/xtensa-lx106-elf/bin for the macOS xtensa-lx106-elf files as well as http://bbs.espressif.com/download/file.php?id=1046 for the esp_iot_sdk_1.5.1 files.

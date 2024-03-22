Find files in .bit .tcl in
ZedboardMemristorControl/design/pmod_spi/pmod_spi.runs

find .hwh in
ZedboardMemristorControl/design/pmod_spi/pmod_spi.gen/sources_1/bd/design_1/hw_handoff

And rename all files so they have identical basename

```
.
└── ZedboardMemristorControl
    ├── boards
    │   └── utility #zedboard top file to be included
    ├── design
    │   └── pmod_spi # Board designs using vivado
    ├── ip
    │   └── ip #ip to be included
    └── notebooks #python code to control
```

## Create SD-card
To build the image from source follow https://github.com/sambuls/Pynq2.7OnZedboard

To fasten the process copy the contents from the sdcard directory onto a correctly formatted sdcard.
A correctly formatted sdcard can easily be achieved by downloading the digilent zedboard example and first writing it to the sdcard.

For macos do the following, replace .img with your downloaded image
```shell
diskutil
sudo umount <disk>
sudo dd bs=4m if=./ZED-2.7.0.img of=/dev/rdisk4 #rdisk on macos (readdisk)
```

Then remove all contents from the sdcard and copy over the contents of the sdcard folder in this repository.

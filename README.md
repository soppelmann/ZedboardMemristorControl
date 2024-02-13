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

[MAIN MENU](https://github.com/caseyjeremiason/C2/blob/main/README.md)

Heat Soak the Printer First

Set the part cooling fans to 25% 

- `M106 S64` 

and then run:

- `PID_CALIBRATE HEATER=extruder TARGET=245`

It will perform a PID calibration routine that will last about 5 minutes. Once it is finished,

- `SAVE_CONFIG` 

which will save the parameters into your configuration file.

- `PID_CALIBRATE HEATER=heater_bed TARGET=100`

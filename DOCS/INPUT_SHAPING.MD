[MAIN MENU](/README.md)


### TURN OFF DYNAMIC ACCELERATION CONTROL

Change the setting highlighted in orange to 0.

![alt text](/DOCS/IMG/TURN_OFF_DYNAMIC_ACCELERATION_CONTROL.PNG "Turn off Dynamic Acceleration Control in Super Slicer")

- `ACCELEROMETER_QUERY`
- `MEASURE_AXES_NOISE`
- `TEST_RESONANCES AXIS=X`
- `TEST_RESONANCES AXIS=Y`


- PUTTY
  - `~/klipper/scripts/calibrate_shaper.py /tmp/resonances_x_*.csv -o /tmp/shaper_calibrate_x.png`
  - `~/klipper/scripts/calibrate_shaper.py /tmp/resonances_y_*.csv -o /tmp/shaper_calibrate_y.png`
- WINSCP
  - Retrieve Images

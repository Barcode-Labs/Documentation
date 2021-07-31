[MAIN MENU](/README.md)

[REVIEW THIS REFERENCE](https://docs.vorondesign.com/community/howto/120decibell/z_endstop_configuration.html) add anything of value to this document

### INITIAL SETUP FOR V2.4_350
- `BED_MESH_CLEAR`
- `G28`
- `QUAD_GANTRY_LEVEL`
- `G28`
- `G90`
- `G1 X175 F3000`
- `G1 Y175 F3000`
- `G1 Z5 F1500`

### ENTER CALIBRATION
- `Z_ENDSTOP_CALIBRATE`

### MOVE DOWN
- `TESTZ Z=-1`
- `TESTZ Z=-0.1`
- `TESTZ Z=-0.01`

### MOVE UP
- `TESTZ Z=1`
- `TESTZ Z=0.1`
- `TESTZ Z=0.01`

### EXITING CALIBRATION
- `ACCEPT`
- `SAVE_CONFIG`

OR
- `ABORT`

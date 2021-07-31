[MAIN MENU](https://github.com/caseyjeremiason/C2/blob/main/README.md)

# Extruder Calibration (e-steps)
Before the first print, make sure that the extruder extrudes the correct amount of material.

- With the hotend at temperature, make a mark between your roll of filament and your extruder, between 120mm and 150mm away from the entrance to the extruder. Measure the distance from the extrance of the extruder to that mark.
- In Octoprint / Mailsail, extrude 50mm 2 times (for a total of 100mm since Klipper doesn’t allow you to extrude more than 50mm at a time).
- Measure from the entrance of your extruder to the mark you made previously.
- In a perfect world, assuming the mark is at 120mm, it would measure 20mm (120mm - 20mm = 100mm), but usually won’t be.
- Update rotation_distance in the extruder section of the configuration file using this formula:
New Config Value = Old Config Value * (Actual Extruded Amount/Target Extruded Amount)
Note: a higher configuration value means that less filament is being extruded.

- Paste the new value into the configuration file, restart Klipper, and try again. Once the extrusion amount is within 0.5% of the target value (ie, 99.5-100.5mm for a target 100mm of extruded filament), the extruder is calibrated!

Typical rotation_distance values should be around 22.6789511 for Afterburner and Mobius (update gear_ratio to 80:20 for Mobius).

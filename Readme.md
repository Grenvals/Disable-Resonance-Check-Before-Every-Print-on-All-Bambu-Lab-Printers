# Disable Automatic Resonance Check Before Every Print on All Bambu Lab Printers

![Image](https://github.com/user-attachments/assets/d9f1c1d5-ac96-437f-a14b-349e3a838274)

This repository provides modified **Machine Start G-code** files that disable the **automatic resonance check** before every print on Bambu Lab printers.

The automatic resonance check is useful after hardware changes or maintenance, but running it before every print is unnecessary for most users. It increases print startup time and generates strong, repetitive vibrations that may gradually loosen hotend screws and other fasteners over time.

The only change made by this repository is skipping the automatic resonance check. The rest of the startup sequence remains unchanged.


## Supported Printers

- ✅ A1
- ✅ A1 mini
- ✅ P1S

### Supported slicers

- Bambu Studio
- OrcaSlicer
- Any slicer that allows editing the Machine Start G-code


## Why Disable the Automatic Resonance Check?

Skipping the automatic resonance check offers several advantages:

- Faster print startup.
- Eliminates unnecessary vibrations before every print.
- May help prevent hotend screws and other fasteners from gradually loosening.
- Reduces mechanical stress caused by repeated resonance testing.

For printers that are already calibrated and have not undergone hardware changes, running the resonance check before every print generally provides little benefit.


## Manual Resonance Calibration

Disabling the automatic resonance check **does not remove the calibration feature**.

You can still run the resonance calibration at any time from the printer's **Calibration** menu.

It is recommended to perform a manual resonance calibration after:

- replacing the hotend or nozzle;
- replacing belts, motors, or other motion components;
- performing major printer maintenance;
- noticing changes in print quality.

## Installation

1. Download the **Machine Start G-code** file for your printer.
2. Open your slicer.
3. Open your printer profile settings.
4. Locate the **Machine Start G-code** section.
5. Replace the existing Machine Start G-code with the file from this repository.
6. Save the printer profile.
![Image](https://github.com/user-attachments/assets/3e2d42d1-46e9-4ef9-a8b1-653f99c93548)

## Disclaimer

Use it at your own risk. Always verify your printer is properly calibrated after hardware modifications or maintenance. If needed, simply run the official resonance calibration from the printer's **Calibration** menu.


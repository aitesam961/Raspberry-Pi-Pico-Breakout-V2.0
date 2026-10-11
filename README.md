# Raspberry Pi Pico Breakout — Revision 2.0

A Raspberry Pi Pico carrier board with labeled GPIO breakouts, a 3.7 V LiPo battery power section, a 5 V DC barrel-jack input, and a Qwiic-compatible connector.

The board can be separated along the marked cut line into a Pico breakout and a standalone power section.

<p align="center">
  <img width="400" src="Images/Screenshot%202022-02-22%20154036.png" alt="Revision 2.0 board render">
  <img width="400" src="Images/Screenshot%202022-02-22%20154404.png" alt="Revision 2.0 PCB layout">
</p>

## Features

- Raspberry Pi Pico footprint with 2.54 mm header breakouts.
- Pin labels printed on the board.
- LiPo battery support and onboard charging circuitry.
- 5 V DC barrel-jack input and power-mode slide switch.
- Charging and power-mode indicator LEDs.
- Qwiic-compatible bus connector.
- Separable breakout and power sections.

## Two board sections

The marked cut line separates the GPIO breakout from the power unit. Review the PCB connections before separating the board so you can identify the connections needed for each section's intended use.

![Board separation line](Images/Screenshot%202022-02-22%20154154.png)

| Pico breakout | Power section |
| --- | --- |
| ![Pico pin labels](Images/Screenshot%202022-02-22%20154226.png) | ![Power section and DC jack](Images/Screenshot%202022-02-22%20154120.png) |

## Power specifications

The original project documentation specifies:

| Parameter | Documented value |
| --- | --- |
| DC jack input | 5 V |
| Battery | 3.7 V nominal LiPo, up to 4.2 V charged |
| Battery capacity | 1–5 Ah |
| Charging current | 500 mA |

Check these values against the schematic and fitted components when building a modified revision.

## Design and manufacturing files

| Location | Contents |
| --- | --- |
| [Source-Files](Source-Files/) | EasyEDA schematic and PCB JSON sources |
| [Schematic PDF](docs/Schematic_Raspberry%20Pi%20Pico%20Breakout%20v2.0_2021-07-02.pdf) | Circuit reference without a CAD editor |
| [Manufacturing-Files](Manufacturing-Files/) | Gerber ZIP, bill of materials, and pick-and-place data |
| [3D-Files](3D-Files/) | OBJ model archive |
| [Images](Images/) | Board renders and layout screenshots |

## Getting started

1. Review the schematic PDF and board images to identify the power connections and GPIO headers.
2. Open the schematic and PCB JSON files in EasyEDA using its workflow for EasyEDA source files.
3. Compare the BOM, footprints, and connector orientation with the parts you plan to fit.
4. Use the supplied manufacturing exports for the matching design revision, or regenerate all exports after editing the source.

This repository contains hardware design files; it does not include application firmware for the Pico.

## Contributing

Open an issue or pull request with the affected circuit, proposed change, and any test results. Keep editable sources and manufacturing exports in sync, and follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## License

GNU General Public License v3.0. See [LICENSE](LICENSE) for the license text.

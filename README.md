# Pomodoro Mark II

Orientation-sensitive desktop timer (mark II).
Codename "Otter" (because they're cute & cuddly, hard-working, and like to roll over).

## Technical Specs
- Custom _triangular_ PCB!
- Raytac nRF52840 Bluetooth Low Energy Module with USB - [MDBT50Q-1MV2](https://www.adafruit.com/product/4078)
- Programming header bonanza (some or all): [SWD](https://www.adafruit.com/product/752), [Tag-Connect TC2050](https://www.tag-connect.com/wp-content/uploads/bsk-pdf-manager/TC2050-IDC-NL_Datasheet_8.pdf), [SOICbite](https://github.com/SimonMerrett/SOICbite), and USB.
- Bluetooth app/backend for tracking tasks (allocate poms to projects etc.)
- LCD/OLED/Sharp memory display (TBD, prototype is Nokia 5110-type)
- [Bosch BNO055 9-DoF orientation sensor/IMU](https://cdn-learn.adafruit.com/assets/assets/000/036/832/original/BST_BNO055_DS000_14.pdf) 

## Project Layout
The project repository (you're looking at it) is laid out at a high level like:

- `cad` 3D design files for the case and other supporting mechanical features.
- `docs` documentation both from a developer and also from the point of view of an end user.
- `firmware` the software running on the board, any needed bootstrapping code, and support scripts
- `hardware` the [KiCAD](https://www.kicad.org/) schematic and board layout
- `production` files needed to manufacture the board, [BOM](https://en.wikipedia.org/wiki/Bill_of_materials), gerbers & etc.
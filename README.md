# NeoDrone v1

Open-source all-in-one drone flight controller + ESC board.

## Repository layout

- `hardware/design/` KiCad source project and schematic sheets
- `hardware/3d/` board 3D exports (`.step`, `.glb`)
- `firmware/` firmware git submodule
- `bom.csv` source BOM export
- `assets/images/` board renders/screenshots
- `assets/diagrams/` wiring diagram markdown
- `assets/photos/` placeholder for future build photos
- `assets/3d/` board with components attached, not motors yet.

Production/manufacturing outputs are intentionally not stored in this repository.

## Firmware submodule

Firmware is linked as a submodule:

- Repository: [dulatello08/neodrone-firmware](https://github.com/dulatello08/neodrone-firmware)
- Path: `firmware/`

After cloning:

```bash
git submodule update --init --recursive
```

## Wiring

Current external connections:

- Motor outputs: M1, M2, M3, M4
- Battery input: VBAT and GND
- Receiver: CRSF UART + power

Detailed diagram: `assets/diagrams/wiring-diagram.md`

## Upload placeholders

- Put build photos in `assets/photos/`
- Put additional 3D models (full assembly/frame) in `assets/3d/`

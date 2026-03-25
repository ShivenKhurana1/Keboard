# keboard

QMK firmware for the keboard RP2040 (Raspberry Pi Pico) keyboard.

## Pins

- Rows: GP14, GP15, GP16, GP17, GP18
- Cols: GP0..GP13
- Encoder: GP27 (A), GP26 (B)
- OLED I2C: GP20 (SDA), GP21 (SCL)

## Notes

- `DIODE_DIRECTION` is set to `COL2ROW`. If your matrix is reversed, flip it in config.h.
- The layout is a generic 5x14 grid. Adjust the keymap to match your physical layout.

## Build

Copy this folder into `qmk_firmware/keyboards/clear60`, then run:

```
qmk compile -kb clear60 -km default
```

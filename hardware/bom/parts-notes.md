# Parts Notes

This file documents part decisions and alternatives.

---

## MCU – MSP430FR4133IG48

Reason chosen:
- Built-in LCD driver
- Ultra-low power
- FRAM (no flash wear issues)
- Mature toolchain

Possible alternatives:
- Other MSP430 LCD variants

---

## RTC – RV-3028-C7

Reason chosen:
- Extremely low power
- High accuracy
- Small footprint

Alternative:
- DS3231 (higher power)
- Internal RTC only (less accurate)

---

## LCD – GDC0209

Reason chosen:
- Passive LCD
- 4 COM configuration
- Low power
- Clean segmented aesthetic
- Compact Size

---

## Power – CR2032

Reason chosen:
- Widely available
- Simple power design
- Long shelf life

---

## Notes

Document supplier part numbers here.
Add LCSC/Mouser/DigiKey references later.


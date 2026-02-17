# ClearTick

A tiny wristwatch built around **MSP430FR4133IG48**, **RV-3028-C7 RTC**, and a **GDC0209 passive LCD** powered by a **CR2032**.

hardware is done, firmware/enclosure are next. I’m keeping it clean + easy to follow so future-me (and anyone curious) can jump in.

---

## Current Status
- ✅ Schematic + PCB: done
- ✅ LCD mapping confirmed:
  - COM0–COM3 → L0–L3
  - SEG0–SEG8 → L10–L18
- ✅ RTC: RV-3028-C7 over I2C
- ⏳ Firmware: not started yet
- ⏳ Enclosure: not started yet

---

## Hardware Overview
**MCU:** MSP430FR4133IG48  
**RTC:** RV-3028-C7 (I2C)  
**LCD:** GDC0209 passive LCD (4 COM, 9 SEG used)  
**Power:** CR2032  
**Programming:** MSP-FET430UIF (SBW)

- Schematic PDF: `hardware/schematic/export/`
- Gerbers: `hardware/pcb/gerbers/`
- BOM: `hardware/bom/`

> Quick note: MSP430FR4133 has an on-chip LCD driver, perfect for low-power segments.

---

## Repo Map (Where to look)
- `hardware/` → schematic, PCB, gerbers, BOM
- `docs/` → mapping tables, bring-up notes, decisions
- `firmware/` → (future) code + drivers
- `enclosure/` → (future) CAD + prints

---

## Getting Started (for contributors)
1. Start with `docs/overview.md`
2. Check `docs/lcd-mapping.md` for segment mapping
3. Hardware files are in `hardware/`
4. Firmware will live in `firmware/` (coming soon)

If you want to help before firmware exists:
- suggest a clean low-power firmware architecture
- RV-3028 register config ideas (alarms, 1Hz, timestamp, etc.)
- LCD segment table organization / generator script ideas

---

## Roadmap 
- **v0.1 Bring-up**
  - I2C scan + RTC read/write
  - Basic timekeeping + 1Hz tick
  - LCD “all segments” test + segment map validation
- **v0.2 Watch Functions**
  - show HH:MM
  - button handling (minutes/hours adjust)
  - low-power loop strategy
- **v0.3 Quality**
  - calibration / drift notes
  - power measurements
  - enclosure draft

---

## Contributing
Issues and PRs are welcome — especially:
- low-power tips for MSP430FR4133
- RV-3028-C7 setup patterns
- LCD driver code structure
- test ideas + bring-up checklists

Keep PRs small and focused. If you change behavior, add a short note in `docs/bringup-notes.md`.

---

## License
MIT License – see LICENSE file.

---

## Thanks
If you build something similar or spot an improvement, please open an issue — I’d love to learn from it.

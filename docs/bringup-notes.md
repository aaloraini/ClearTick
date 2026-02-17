# Bring-Up Notes

This file tracks real-world testing during first power-up.

Keep it honest. Document failures.

---

## Pre-Power Checks

- [ ] No shorts between VCC and GND
- [ ] Correct CR2032 polarity
- [ ] SBW header continuity verified
- [ ] RTC pull-ups present (I2C)

---

## First Power-Up

Date:
Notes:

---

## Programming Test

Tool: MSP-FET430UIF

- [ ] Device detected
- [ ] Flash successful
- [ ] Debug session stable

Notes:

---

## I2C Scan

Expected:
RV-3028 address: 0x52 (7-bit)

- [ ] ACK received
- [ ] Registers readable
- [ ] Seconds incrementing

Notes:

---

## LCD Test

Goal:
Turn on all segments to verify mapping.

- [ ] All COM lines active
- [ ] All SEG lines tested
- [ ] No ghosting observed
- [ ] No weak segments

Notes:

---

## Power Consumption

Mode: Idle  
Mode: RTC running  
Mode: LCD active  

Measurements:

---

## Known Issues

(None yet)


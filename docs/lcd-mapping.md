# LCD Mapping

Display: GDC0209  
Type: Passive LCD  
Configuration used: 4 COM, 9 SEG

---

## Confirmed Hardware Mapping

| LCD Pin | Function | MSP430 Pin |
|----------|----------|-------------|
| COM0 | L0 | P7.x |
| COM1 | L1 | P7.x |
| COM2 | L2 | P7.x |
| COM3 | L3 | P7.x |
| SEG0 | L10 | Px.x |
| SEG1 | L11 | Px.x |
| SEG2 | L12 | Px.x |
| SEG3 | L13 | Px.x |
| SEG4 | L14 | Px.x |
| SEG5 | L15 | Px.x |
| SEG6 | L16 | Px.x |
| SEG7 | L17 | Px.x |
| SEG8 | L18 | Px.x |


---

## Logical Segment Map (To Be Filled During Firmware)

Example structure:

Digit 1:
- Segment A → COMx/SEGx
- Segment B → COMx/SEGx
- Segment C → COMx/SEGx

Digit 2:
...

---

## Testing Strategy

1. Enable LCD module
2. Drive one segment at a time
3. Create visual mapping table
4. Document in this file


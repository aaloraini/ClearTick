# RTC Notes – RV-3028-C7

RTC: RV-3028-C7  
Interface: I2C  
7-bit address: 0x52

---

## Initial Goals

- Confirm I2C communication
- Read seconds register
- Enable timekeeping
- Configure 1Hz interrupt (optional)
- Evaluate drift

---

## Registers of Interest

- Seconds
- Minutes
- Hours
- Control register
- Status register

(Refer to RV-3028 datasheet for full register map.)

---

## Planned Configuration

- 24-hour mode
- Basic timekeeping
- No alarms initially
- No EEPROM features initially

---

## Future Enhancements

- Use timestamp feature
- Enable backup switchover
- Evaluate temperature compensation
- Calibrate offset register


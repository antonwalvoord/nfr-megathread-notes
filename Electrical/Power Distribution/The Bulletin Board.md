---
dg-publish: true
---
# PDM
## Hardware
- Implement efuse circuit fix on AC lines
- Connect and test Pump and Fan

## Software
- Officially get current sensing working properly
- Get software based fusing working
- Get software efuse resetting working
- Get AC PWM working

# Harness
## Purchases
- [x] Size 20 Pins
- [x] HDP20 Pin removers
- [ ] Replacement AC connectors and potentially more crimps
- [ ] Replacement penthouse TS connectors to repopulate with proper TS wire
	- [ ] TSMP
	- [ ] VIB
	- [ ] BMS
- [ ] Potentially buy more 3pin connectors for wheel brokers (*did find more after rooting through a box*)
- [x] New size 4 pins and sockets
	- [ ] Will need to stay up to date on whether or not these actually come after resubmitting sample request
	- [ ] Might be able to get away with 15A rated contactor/connectors instead in the same family
- [ ] Inertial switch connector
- [ ] Closed barrel splices

## Design updates
- Potentially a replacement connector for LV box power connector
- CAN breakout connector
	- **Need more crimps for this?**
- General polish (*Thorough look over to see what needs redoing*)
- CAN backbone length?

## Things that got pushed back
>Bolding means it needs something purchased for it
- **Heat shrinking and replacing bad connections in penthouse external GLV connector**
- **AC Wiring**
	- External stuff should be able to be assembled and half of internal but need new connector for the board
- Back box wiring
	- Board-side connectors should be assembled with extra length wires even though box is not modelled
- GLVMP wiring (*I think*)
- Properly pigtail and heatshrink cockpit shutdown connections
- **Implement inertial switch connection**
- BOTS wiring (*I think, at the very least likely needs redoing*)
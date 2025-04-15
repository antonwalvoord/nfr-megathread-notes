---
dg-publish: true
---
# TASKS POST FIRST DRIVE
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
- Check Dashbox internal harness for CAN wiring issues focusing on Dashboard specifically - ECU didn't have issues but Dash did
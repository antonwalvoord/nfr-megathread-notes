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
	- Assemble connectors for [DAQ Dynamics](https://americas-northwestern-formula-racing-northwestern-univ.365.altium.com/designs/0CC4AB71-D497-49EA-B222-C90C65C91CA3?variant=[No+Variations]&activeView=PCB&activeDocumentId=DAQ_Dynamics.PcbDoc&layers=[1,1,39,40,32,37,38,35,36,33,34,70,72,67108882,67108884,67108888,74,55,73]&location=[2,20.37,24.09,26.1,0]#design) and [DAQ Telemetry](https://americas-northwestern-formula-racing-northwestern-univ.365.altium.com/designs/3B3C07D6-C3D5-4EA0-A860-0AA923C21D01?variant=[No+Variations]&activeView=PCB&activeDocumentId=DAQ_Telemetry.PcbDoc&layers=[1,1,39,40,32,37,38,35,36,33,34,60,67108884,67108885,67108887,67108888,74,55,73]&location=[2,20.43,59.43,31.2,0]#design)
- GLVMP wiring (*I think*)
- Properly pigtail and heatshrink cockpit shutdown connections
- **Implement inertial switch connection**
- BOTS wiring (*I think, at the very least likely needs redoing*)
- Check Dashbox internal harness for CAN wiring issues focusing on Dashboard specifically - ECU didn't have issues but Dash did
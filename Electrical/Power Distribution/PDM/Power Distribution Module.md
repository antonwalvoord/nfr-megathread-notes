---
dg-publish: true
dg-pinned: true
---
### Members in charge
- [Ash Wei](https://nufsae.slack.com/team/U07PKBS1Y0K)
- [Michael Xing](https://nufsae.slack.com/team/U05TPFB4F51)

### [Project Google Drive](https://drive.google.com/drive/folders/1bUXDNzRZ9vC9e3OqMUGO0GZfrWr8vvME?usp=drive_link)

### Project Information
- #### Scope/Interactions:
	- Low Voltage (LV) Battery: Power Distribution Module (PDM) must take in LV power from the LV Battery and distribute it to the enclosures throughout the car
	- Active Cooling (AC): PDM must provide power to the AC (the pump and fan which regulate the coolant system).
- #### Skills:
	- C++
	- Soldering
	- Circuit debugging
	- PCB design
- #### Description:
	- PDM is the hub for LV power throughout the car. Everything in the car except for the motor runs off of this supply. Because of this it has to be both safe and reliable. PDM takes in the LV battery supply and monitors where the current goes and sends this data over CAN, the communication network throughout the car. It also has electronically resettable fuses in order to detect and protect against overcurrent faults. It drives the AC by providing power using PWM to control the strength of the cooling based on drive state data provided over CAN.
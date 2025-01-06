---
dg-publish: true
---
### Electrical
##### Tractive System (TS)
By **EV.1.1**: "Every part electrically connected to the Motor(s) and/or Accumulator(s)"
##### Grounded Low Voltage (GLV)
By **EV.1.2**: "Every electrical part that is not part of the Tractive System" More rules found in **EV.4.4** - must be Grounded to the Chassis and able to operate with the [[#Accumulator|Accumulator]] removed from the vehicle
##### Accumulator
By **EV.1.3**: "All the battery cells or super capacitors that store the electrical energy to be used by the Tractive System" More rules found in **EV.5.1**
##### Penthouse
This is an internal term which describes the upper portion of our Accumulator container. We make this distinction as the [[Car Architecture#Penthouse|penthouse]] contains the logic portion of the Accumulator, whereas we refer to the portion which contains the battery cells as simply the Accumulator. ==*By rules the penthouse is indistinguishable from the Accumulator*==
##### Energy Meter
Described in **EV.3.2**: Measures power and voltage of the accumulator to ensure [[FSAE 2025 Rules|rules]] compliance to **EV.3.3**
##### Motor Controller / Inverter
Supplies power from the [[#Accumulator|Accumulator]] to the motor. Converts DC to AC and regulates how much power goes to the motor based on a number of conditions, including torque requests from the [[ECU]]
##### Accelerator Pedal Position Sensor (APPS)
Described in **T.4.2**: Measures how far the accelerator pedal is depressed in order to determine how much power should go to the motor
##### Brake System Encoder (BSE)
Described in **T.4.3**: Measures brake system pressure.
##### Maintenance Plugs
Described by **EV.5.3**: Electrically connects and disconnects [[#Accumulator|Accumulator]] segments from one another for maintenance.
##### Isolation Relays (IR)
Described by **EV.5.4**: Normally open relays which disconnect the two poles of the [[#Accumulator|Accumulator]] and prevent High Voltage **T.9.1.1** from being present outside the Accumulator container.
##### Manual Service Disconnect (MSD)
By **EV.5.5** "A Manual Service Disconnect (MSD) must be included to quickly disconnect one or the two poles of the Accumulator **EV.11.3.2**"
##### Interlocks
Described in **EV.7.8**: Interlocks are wires or connections which when unplugged open the shutdown circuit. Think of it like a safety switch which detects whether or not a plug is plugged in. They are required on the [[#Manual Service Disconnect (MSD)|MSD]] and on any [[#Tractive System (TS)|TS]] connector outside of a housing (including those that are mounted on a housing)


##### Battery Pack Configuration Shorthand
Often it is helpful to know how many series and parallel connections a battery pack has. The number of series connections indicates the pack voltage, and the number of parallel connections indicates the pack current/capacity. To quickly share this information we use the shorthand "`XsYp`" where "X" denotes the number of series connections and "Y" the number of parallel connections. Meaning `10s4p` would represent a battery pack with `10` series connections and `4` parallel connections
### Mechanical
🚧Under [[How to contribute to the megathread|construction]]🚧
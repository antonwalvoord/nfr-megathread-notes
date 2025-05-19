---
dg-publish: true
---
🚧UNDER CONSTRUCTION [[How to contribute to the megathread|You Can Help!]]🚧
# Mechanical
Our vehicle is a single motor + differential car. Many other teams have more sophisticated drivetrains, including setups with hub motors, which allow you to eliminate all spinning shafts inboard of the wheels.
We have stuck with the traditional single motor + differential setup for simplicity.
🚧I need help for this🚧
# Electrical
>[!Warning] For most up to date information, check the [draw.io](https://app.diagrams.net/#G1aAUkTBznf-oBW0_HJwPR886YPGE_Ngbq#%7B%22pageId%22%3A%22AH0zOfJDxDtdpztpxlL7%22%7D)
## Overview
![](https://i.imgur.com/IrDRmHq.png)

🚧draw.io output and generals🚧

---
#### Shutdown Circuit
The shutdown circuit (Described in [[FSAE 2025 Rules|EV.7.2]]) is a safety mechanism which serves to disconnect the [[Team Terminology (Glossary)#Tractive System (TS)|Tractive System]] either automatically or manually. This is done through a series of switches and [[Team Terminology (Glossary)#Interlocks|interlocks]] which can break power supply to the [[Team Terminology (Glossary)#Isolation Relays (IR)|IR'S]] thus isolating the Tractive System from the outside world to protect us from the high voltage. For specifics on the wiring, see the drawing below.

![](https://i.imgur.com/p0XU1E7.png)

---
#### CAN (Controller Area Network)
CAN is a rugged information bus protocol that allows many devices to communicate with one another over a limited number of wires (two per bus). This means that devices can only communicate with other devices on the same bus (unless they use another device which is on both busses as an intermediary).

On NFR25 we originally designed to have two separate CAN busses but have modified our designs to use a single bus instead.

>[!Warning] All boards have been migrated over to the **DRIVE** bus. The *DATA* bus now is purely vestigial as it is not worth the effort of extracting it from the cabling in the harness.

Our two CAN busses are called *DATA* and **DRIVE** CAN. *DATA* is (as the name suggests) intended for purely data acquisition purposes and is not [[Team Terminology (Glossary)#Drive Critical|drive critical]]. **DRIVE** contains information directly related to controlling the driving of the car and is drive critical. There are two buses to reduce the [[Team Terminology (Glossary)#Bus Load|bus load]] of any one bus which is intended to make the car's communication network more robust.

>[!note] For more low level information on how CAN actually works, refer to [this article on DigiKey](https://forum.digikey.com/t/overview-of-the-can-bus-protocol/21170) or [this](https://www.digikey.com/en/blog/the-basics-of-the-controller-area-network) one, as well as [this](https://www.csselectronics.com/pages/can-bus-errors-intro-tutorial) article on CAN errors

The drawing below denotes which devices are connected to which CAN busses, arranged as to approximate location within the car.

![](https://i.imgur.com/821K77q.png)

## Battery Structure
#### Accumulator
🚧 *overview text* 🚧
The [[Team Terminology (Glossary)#Accumulator|Accumulator]] is the high voltage battery which supplies the power that drives our motor. It is important to exercise caution when handling the Accumulator
##### Full Pack Electrical Structure

| Cells        | Configuration                       | Max Voltage | Nominal Voltage | Capacity | Fused Current                                                                                                                                                                                                                                                          |
| ------------ | ----------------------------------- | ----------- | --------------- | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Molicel p45b | 5 Series Segments *see table below* | 588 V       | 504 V           | 13.5 Ah  | 80 A<br>[Fuse](https://www.mouser.com/ProductDetail/Littelfuse/L75QS080.V?qs=w%2Fv1CP2dgqquMmGcdv%252B%252BVQ%3D%3D)<br>[Datasheet](https://www.littelfuse.com/~/media/electrical/datasheets/fuses/semiconductor-fuses/littelfuse-industrial-l75qs-fuse-datasheet.pdf) |
##### Single Segment Electrical Structure

| Cells        | Configuration                                                    | Max Voltage | Nominal Voltage | Capacity | Fused Current |
| ------------ | ---------------------------------------------------------------- | ----------- | --------------- | -------- | ------------- |
| Molicel p45b | [[Team Terminology (Glossary)#Battery Pack Configuration Shorthand\|28s3p]] | 117.6 V     | 100.8 V         | 13.5 Ah  | 80 A          |

#### Low Voltage (LV) Battery
The [[LV Battery]] powers everything other than the [[Team Terminology (Glossary)#Tractive System (TS)|Tractive System]]. It's located in the [[#LV Box]]. The mechanical structure is designed by the [[Accumulator Home|Accumulator Subteam]] and the electrical structure is designed by the [[Power Distribution Home|Power Distribution Subteam]].
##### Electrical Structure

| Cells        | Configuration                                                              | Max Voltage | Nominal Voltage | Capacity | Fused Current                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------ | -------------------------------------------------------------------------- | ----------- | --------------- | -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Molicel p42a | [[Team Terminology (Glossary)#Battery Pack Configuration Shorthand\|6s3p]] | 25.2 V      | 21.6 V          | 12.6 Ah  | 40 A<br>[Fuse](https://www.amazon.com/Chanzon-50Pcs-Listed-Standard-Automotive/dp/B0CYP881ZL?crid=KOYM53VK3BJI&dib=eyJ2IjoiMSJ9.kAud1lwfnSJMHH_HHJksJ3AayT8HQIqm2DRrKdBcHMnv_5H38w8UA5qC38SW-9TZeDXUhWiUH5apFWH5WxkjyAqGwauFDSRfrqBKFBpEtEMMDnBAl-fw4ZHpuBtrKXKUkab2x4VEEME3K_TacMuT8-gI3TrKF94495g-FLnbpBmou8O6N8UpJYpcsO5qqdaKDeMduAyfolulBSMIC2Yjs8qKYCl8mqNGbtF5UdIVvy0.ofn3doJM6QnXEOKwYIaudk923TirJMeK_C6ZZ_5s2C0&dib_tag=se&keywords=40%2Bamp%2Batc%2Bfuse&qid=1721963859&sprefix=40%2Bamp%2Batc%2Bfus%2Caps%2C117&sr=8-4&th=1) |

## Power Distribution
All [[Team Terminology (Glossary)#Grounded Low Voltage (GLV)|GLV]] power is supplied by the [[#Low Voltage (LV) Battery|LV Battery]]. It runs throughout the car at an unregulated voltage straight from the battery (20-25V generally). It is then regulated down on a per-board basis as needed. Some projects like the [[Wheel Brokers]] have regulated voltage being fed to them from a parent board over a short distance.

## Enclosures
#### Dashbox
Contains [[ECU]] and [[Front DAQ]] boards as well as housing the [[Dashboard]] and mounting the [[#Shutdown Circuit|Cockpit Shutdown button and Inertia Switch]].
#### LV Box
Contains the [[Power Distribution Module]] and [[Low Voltage Battery Management System (LV BMS)]] as well as the [[LV Battery]].
#### Accumulator
Contains the [[#Accumulator|HV Battery]] as well as the [[HV BMS Daughterboards]] for pack monitoring.
#### Penthouse
Contains all of the HV related electronics. This includes the [[High Voltage Battery Management System (HV BMS)]], [[HV Board and IMD]], [[Team Terminology (Glossary)#Contactors|Contactors]], [[Team Terminology (Glossary)#Energy Meter|Energy Meter]], [[Voltage Indicator Board (VIB)]], and [[Team Terminology (Glossary)#Precharge Resistor|Precharge Resistor]].
#### Inverter
Contains the [[Team Terminology (Glossary)#Motor Controller / Inverter|Motor Controller / Inverter]], [[Team Terminology (Glossary)#Manual Service Disconnect (MSD)|Manual Service Disconnect]], and the [[Team Terminology (Glossary)#DC Link Capacitor|DC Link Capacitor]].
#### Backbox
Contains the [[Telemetry Board]] and the [[Dynamics Board]].
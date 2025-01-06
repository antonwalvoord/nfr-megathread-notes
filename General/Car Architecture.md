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
### Overview
🚧draw.io output and generals🚧
### Shutdown Circuit
The shutdown circuit (Described in [[FSAE 2025 Rules|EV.7.2]]) is a safety mechanism which serves to disconnect the [[Team Terminology#Tractive System (TS)|Tractive System]] either automatically or manually. This is done through a series of switches and [[Team Terminology#Interlocks|interlocks]] which can break power supply to the [[Team Terminology#Isolation Relays (IR)|IR'S]] thus isolating the Tractive System from the outside world to protect us from the high voltage. For specifics on the wiring, see the drawing below.

![](https://i.imgur.com/7lUzD3D.png)

### CAN (Controller Area Network)
### Battery Structure
#### Accumulator
🚧 *overview text* 🚧
###### Full Pack Electrical Structure

| Cells        | Configuration                       | Max Voltage | Nominal Voltage | Capacity | Fused Current                                                                                                                                                                                                                                                          |
| ------------ | ----------------------------------- | ----------- | --------------- | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Molicel p45b | 5 Series Segments *see table below* | 588 V       | 504 V           | 🚧       | 80 A<br>[Fuse](https://www.mouser.com/ProductDetail/Littelfuse/L75QS080.V?qs=w%2Fv1CP2dgqquMmGcdv%252B%252BVQ%3D%3D)<br>[Datasheet](https://www.littelfuse.com/~/media/electrical/datasheets/fuses/semiconductor-fuses/littelfuse-industrial-l75qs-fuse-datasheet.pdf) |
###### Single Segment Electrical Structure

| Cells        | Configuration                                                    | Max Voltage | Nominal Voltage | Capacity | Fused Current |
| ------------ | ---------------------------------------------------------------- | ----------- | --------------- | -------- | ------------- |
| Molicel p45b | [[Team Terminology#Battery Pack Configuration Shorthand\|28s3p]] | 117.6 V     | 100.8 V         | 🚧       | 80 A          |

#### Low Voltage (LV) Battery
The [[LV Battery]] powers everything other than the [[Team Terminology#Tractive System (TS)|Tractive System]]. It's located in the [[#LV Box]]. The mechanical structure is designed by the [[Accumulator Home|Accumulator Subteam]] and the electrical structure is designed by the [[Power Distribution Home|Power Distribution Subteam]].
###### Electrical Structure

| Cells        | Configuration                                                   | Max Voltage | Nominal Voltage | Capacity | Fused Current                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------ | --------------------------------------------------------------- | ----------- | --------------- | -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Molicel p42a | [[Team Terminology#Battery Pack Configuration Shorthand\|6s3p]] | 25.2 V      | 21.6 V          | 12.6 Ah  | 40 A<br>[Fuse](https://www.amazon.com/Chanzon-50Pcs-Listed-Standard-Automotive/dp/B0CYP881ZL?crid=KOYM53VK3BJI&dib=eyJ2IjoiMSJ9.kAud1lwfnSJMHH_HHJksJ3AayT8HQIqm2DRrKdBcHMnv_5H38w8UA5qC38SW-9TZeDXUhWiUH5apFWH5WxkjyAqGwauFDSRfrqBKFBpEtEMMDnBAl-fw4ZHpuBtrKXKUkab2x4VEEME3K_TacMuT8-gI3TrKF94495g-FLnbpBmou8O6N8UpJYpcsO5qqdaKDeMduAyfolulBSMIC2Yjs8qKYCl8mqNGbtF5UdIVvy0.ofn3doJM6QnXEOKwYIaudk923TirJMeK_C6ZZ_5s2C0&dib_tag=se&keywords=40%2Bamp%2Batc%2Bfuse&qid=1721963859&sprefix=40%2Bamp%2Batc%2Bfus%2Caps%2C117&sr=8-4&th=1) |
### Power Distribution
### Enclosures
#### Dashbox
#### LV Box
#### Accumulator
#### Penthouse
#### Inverter
#### Backbox
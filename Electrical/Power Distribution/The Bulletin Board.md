---
dg-publish: true
---
## Weekly Goals (Week of January 13)

###### **For Harness**
- [x] Add [manufacturing notes](https://nufsae.slack.com/archives/C07P7C9PF5F/p1733958734239609) to your designs
	- ***Many people have done this but I think there are still some I have not taught, reach out to me if this is the case!***
- [ ] Take a look at the frame in the autobay now that it is fully tacked
- [ ] Learn and practice how to crimp and assemble connectors
	- Here is a learning resource for [crimping connectors](https://www.youtube.com/watch?v=GJqt5VYRBro) 
- [ ] Test Big Papa's capability for CAN transmission and splicing
	- Here are some learning resource for [crimping splices](https://youtu.be/G8OpSIAQqtw?si=HFHrOl0FsHYRMd87) and [soldering splices](https://youtu.be/u7C2OqBngnw?si=ggfWaJrPUHmEXt7L). While the guy in the second video is *very* opinionated he isn't really correct as both crimps and solder splices have their advantages and disadvantages.
- [ ] Review the [[Harness]] design as a whole or at least the portion you're in charge of manufacturing, referencing the [[Car Architecture#Overview|electrical architecture]] might be useful

###### **For PDM**
- [ ] *Because it seems like hardware is facing delays:* Begin working on the software for PDM
- [ ] It seems like the replacement PMOS doesn't have a high enough current rating. I have found some substitutes but feel free to look for more. So far I have found the [DMP4006SPSWQ-13](https://www.mouser.com/ProductDetail/Diodes-Incorporated/DMP4006SPSWQ-13?qs=QNEnbhJQKvau%2F67E%252BtZDyg%3D%3D) and the [NTMFS002P03P8ZT1G](https://www.mouser.com/ProductDetail/onsemi/NTMFS002P03P8ZT1G?qs=stqOd1AaK79thd%252BWxQn8jQ%3D%3D)  
	- For reference, ideally we would like a PMOS with a similar footprint to the previous part: `SQJ147ELP-T1 GE3`. Otherwise we will have to have a breakout connection, which isn't ideal but is an option.

###### **For LV Charger**
- [ ] Create a presentation for [[Team Terminology#Preliminary Design Review (PDR)|PDR]] and prepare how to convey what the schematic does and how it does it (referencing the datasheet might be useful) [example DR for reference](https://docs.google.com/presentation/d/1-fCKBrOlIeWMv5JdjkKDEaHvMuicsPBqZMI5pWFt9S0/edit?usp=sharing)
	- **1 week behind schedule**
- [ ] Schedule a PDR
	- **1 week behind schedule**

## Monthly Goals (January)

###### **For Harness**
- [ ] *Completely* finalize internal harness designs
- [ ] External Harnesses largely manufactured
- [ ] Begin testing of external harness

###### **For PDM**
- [ ] Solve overcurrent protection issue
- [ ] Complete [testing plans](https://docs.google.com/document/d/1Ojkzd-2abVfz04r5hTp6LYRJP8-pr1D0azjeg3GUBKw/edit?usp=sharing) 
- [ ] Finish first draft of software (sans bugfixing)

###### **For LV Charger**
- [ ] Finish schematic and layout
- [ ] Complete a DR
- [ ] Have a design ready to be ordered for manufacture
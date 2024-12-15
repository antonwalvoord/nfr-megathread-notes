---
dg-publish: true
---
>[!WARNING] Altium is **Windows only!**
>In order to use Altium on a Mac you'll first need to set up [[UTM (Free Windows Emulator) Setup Guide|UTM]], a free windows emulator, or [Parallels](https://www.parallels.com/), a paid windows emulator.
>
>If you don't want to install or set up any emulators you can also use [Apporto](https://northwestern.apporto.com/), which is a virtual machine hosted by Northwestern. *This route has easier setup but a worse experience*
### Instructions for the new member
1. Create an account on [altium.com](http://altium.com)
2. During setup ***use your school email*** and select something that looks like "NA Formula Racing"
3. A request to join will be sent to a license admin and must be approved, see: [[#Instructions for the License/Workspace Admin]]
4. Download Altium from [THIS SPECIFIC LINK](https://www.altium.com/products/downloads) 
- Make sure the latest version is selected on the right for Altium Designer then click “Online Installer” and you’ll get an exe to install Altium

![step1](https://github.com/antonwalvoord/nfr-megathread/blob/main/src/site/img/altium_onboarding/step1.PNG?raw=true)
- Install and run Altium and sign into your account
- Click on the profile button in the top right and click **“Licenses”**
- Under the Altium Designer license with 50 slots click **“Use license”**
- Click on the cloud with a strikethrough and select the workspace

![step2](https://github.com/antonwalvoord/nfr-megathread/blob/main/src/site/img/altium_onboarding/step2.PNG?raw=true)
5. Congrats, you're all set up! Check out [[#Getting started using Altium]] for notes on how to use Altium. Consider adding the [[#Useful plugin (Samacsys Library Loader)|Samacsys Library plugin]]
### Instructions for the License/Workspace Admin
- ##### To get new members licenses:
1. Log into Altium 365 and go to **Company Dashboard** (Found by clicking on your profile photo in the top right corner)
2. Go to **“Licenses”** tab on the sidebar
	- View pending license requests and approve by adding requester to the “all members" group - any person who follows the steps outlined in [[#Instructions for the new member]] should appear here. If they aren’t there you may have to add them manually
3. Check that it worked by finding their name under the **“Users and Groups”** tab on the sidebar
- ##### To get new members into the workspace:
1. Log into Altium 365 and go to **“Workspace Members”** on the left sidebar
2. Click **“Invite Members”** and enter all email addresses
3. Click **“Request Invitation”** and contact a [[#List of Current Workspace Admin|Workspace Admin]] for approval - they will receive an email
### List of Current License Admin
- [Anton](https://nufsae.slack.com/team/U05U23W4WJV)
- [Arda](https://nufsae.slack.com/team/U05U23X8S73)
- [Benji](https://nufsae.slack.com/team/U043TF8RB6F)
- [Charlie](https://nufsae.slack.com/team/U044676UDBK)
- [Drake](https://nufsae.slack.com/team/U043T3CEQ06)
- [Evan](https://nufsae.slack.com/team/U044SGB5Q78)
- [Matias](https://nufsae.slack.com/team/U05U26CDE49)
### List of Current Workspace Admin
- [Charlie](https://nufsae.slack.com/team/U044676UDBK)
- [Evan](https://nufsae.slack.com/team/U044SGB5Q78)
### Getting started using Altium
On a fresh install of Altium you'll be greeted by the home page. On the left side panel is your file manager. The tab is called **"Projects"**. You'll need to either [open an existing project or create one of your own](https://www.altium.com/documentation/altium-designer/creating-projects-documents). *It is important to note that there are two categories of projects: those that are local, and those that are in the shared "workspace".* If you'd like others to be able to access and collaborate on your project, you should make it in the **==workspace==** **(this is recommended for most formula projects)**.

>[!TIP] The Basics
The basic design flow of Altium is as follows. First, [create a schematic file](https://www.altium.com/documentation/altium-designer/schematic-capture#setting-up-a-schematic-document) for your project and [design your circuit](https://www.altium.com/documentation/altium-designer/schematic-capture#searching-for-and-placing-components) (For more complicated designs it may be worth creating a [multi-sheet design](https://www.altium.com/documentation/altium-designer/schematic-capture#creating-a-multi-sheet-design)). Then [validate](https://www.altium.com/documentation/altium-designer/design-validation) your design and [create a PCB file](https://www.altium.com/documentation/altium-designer/laying-out-your-pcb#setting-up-a-pcb-document). Once you've created that file, you'll need to [sync it with your schematic](https://www.altium.com/documentation/altium-designer/laying-out-your-pcb#placing-components) and begin to roughly lay out components in functional groups. Finally you need to ensure your PCB document has the proper design rules ([hosted here](https://drive.google.com/drive/folders/1BwvYNkELOf7sJ1a7A252MouveoW5z5zN?usp=drive_link)) and you can begin [routing](https://www.altium.com/documentation/altium-designer/interactive-routing-pcb) the connections. When your design is finished and has been reviewed, you'll need to [export fabrication files](https://www.altium.com/documentation/altium-designer/preparing-your-design-for-manufacture) which can be sent to a manufacturer for purchase. All done!

When you're first getting started using Altium it will take a while to get used to the UI. As a little jump start, the most important tools for your workflow will likely include the **"Components"**, **"Manufacturer Part Search"**, and **"Properties"** panels (accessed by clicking on the "Panels" button in the bottom right which is shown below)

![500](https://i.imgur.com/cn0aUNw.png)
The **components panel** is used to place parts from [the workspace component library](https://americas-northwestern-formula-racing-northwestern-univ-2.365.altium.com/components) or your local component library. **Manufacturer part search** is useful to check for component schematics and footprints that are uploaded by the manufacturer (searching by component title or part number). Finally, the **Properties** panel is *EXTREMELY* useful for information about every part of your design, from the schematic, to component footprints and datasheets, to traces on your circuit board.

##### Useful shortcuts:
- (While in )
##### Useful plugin (Samacsys Library Loader):
Many components you'd like to use will not have their schematic and/or footprint in either the **components** or **manufacturer part search** panels. In this case it can be difficult to import them into your design. There is a plugin you can add to Altium which will automatically import a wide variety of parts into your project for you. While the list is not exhaustive, you will be happy to have this tool in your install. The tool is called [Samacsys Library Loader](https://www.samacsys.com/altium-designer-library-instructions/) and setup information can be found at the link provided.
#### Useful resources:
- [Altium Academy](https://www.youtube.com/@AltiumAcademy) is a great resource for Altium tips and general circuit knowledge. If you have specific questions it's worth using the channel's search bar to take a look
- [Falstad](https://www.falstad.com/circuit/) is a very easy to use online circuit simulator which can be helpful to check your design thinking with
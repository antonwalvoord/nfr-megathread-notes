1. Go to [UTM's Website](https://mac.getutm.app/) and download the the software
2. Follow these [Instructions](https://docs.getutm.app/guides/windows/) (Copied below)

If you run into issues, consult the “[Troubleshooting](https://docs.getutm.app/guides/windows/#troubleshooting)” section of the instructions

>[!WARNING]- Known Issue During Install
>If you run into UTM [boot looping](https://simple.wikipedia.org/wiki/Bootloop) during the install process, you need to make sure **not** to click anything when it prompts you to click any key to install with the drive. This should fix the problem.
## Instructions
1. Use CrystalFetch to download the latest installer ISO.
2. Open UTM and click the “+” button to open the VM creation wizard.
3. Select “Virtualize”.
4. Select “Windows”.
5. Make sure “Import VHDX Image” is _unchecked_ and “Install Windows 10 or higher” is _checked_. Also make sure “Install drivers and SPICE tools” is _checked_. Press “Browse” and select the ISO you built in step 1.
6. Pick the amount of RAM and CPU cores you wish to give access to the VM. Press “Next” to continue.
7. Specify the maximum amount of drive space to allocate. Press “Next” to continue.
8. If you have a directory you want to mount in the VM, you can select it here. Alternatively, you can skip this and select the directory later from the VM window’s toolbar. The shared directory will be available after installing SPICE tools (see below). Press “Next” to continue.
9. Press “Save” to create the VM. Wait for the guest tools to finish downloading and press the Run button to start the VM.
10. Press any key to start the Windows installer and follow the instructions on screen. If you have issues with the mouse, press the mouse capture button in the toolbar to send mouse input directly. Press Control+Option together to exit mouse capture mode. Sometimes, due to driver issues, you can enter and exit capture mode and the mouse cursor works normally again.
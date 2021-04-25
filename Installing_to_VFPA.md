# Installing to VFPA
I cloned the upstream to my local box.
Copied the Foxcode.app, FoxcodePlus.app, and FoxcodePlus directory in to the VFPA install folder.
Turning on the FoxcodePlus feature wouldn't "stay" on. 
VFPA UAC Virtualization is disabled, where VPF9 is enabled. 
This means to write to the protected Program Files(x86) folder, one must run VFPA as an administrator to get the FoxcodePlus ini file to write.

The next issue to solve is in VFPA, typing changes the position of the keyboard focus to the next line and highlights to the end of the line.
I found the Activate of the Toolbar that hosts the grid that shows the intelisense has a Mouse Drag command. This is causing the errant behavior.
Commenting the line out makes the code usable in VFPA. I'm not sure what is lost yet, as I'm new to the tool.


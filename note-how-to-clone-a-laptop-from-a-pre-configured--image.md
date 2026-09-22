# How to Clone a New Laptop from a Seed or Pre-Configured Image on an External Hard Drive

1.	Plug the external hard drive with the seed into the new laptop.
2.	When turning on the laptop, press [F12] to enter "Boot Menu". 
3.	A menu will appear listing bootable devices. Select your hard drive (e.g., “USD HDD…”). 
4.	This will launch the imaging environment (e.g., Clonezilla). 
5.	Choose language (e.g., "English").
6.	Choose keyboard layout (e.g., "Keep the default keyboard layout").
7.	Choose "Start Clonezilla". 
8.	To put the seed or image on your external hard disk onto the laptop's internal storage and use it to clone a disk, select "device-image…". 
9.	For “Mount Clonezilla image directory”, choose "local_dev Use local device…" (e.g., hard drive).
10.	Press [Enter] to continue.
11.	Make sure the external hard drive can be detected before pressing [Ctrl] + [C] to continue.
12.	To mount a device as home/partimag (Clonezilla image(s) repository), choose "sdb2…".
13.	For “Which directory is for the Clonezilla image repository?”, choose "Image_and_Software".
14.	Select "Done".
15.	For “Choose the mode to run the following wizard about advanced parameters”, choose "…Beginner mode…".
16.	Choose "restoredisk Restore an image to local disk" to overwrite the data on your hard drive. 
17.	If asked to choose the image file to restore, choose "…Notes 11…".
18.	If asked to choose the target disk(s) to be overwritten, choose the hard drive on the laptop. 
19.	Choose no checking if asked to check something. 
20.	Choose "Shutdown" as the action to perform after finishing. 
21.	Press [Enter] or input "y" if prompted. 

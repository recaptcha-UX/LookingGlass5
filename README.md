# LookingGlass5
Complete Operating System UX Scheme.

Looking Glass 5 is a complete UX addon scheme for the Moonshell 2.x operating system. Moonshell 2 is 100% proprietary so this
system uses a lot of files that ordinary developers may not understand. I will attemped to explain that in more detail below

Moonshell 2 was released in 2010, but the User interface is quite poor and lacking in quality. Looking Glass 5 fixes this by
adding crisp new images, sounds, visuals, and fonts to the Moonshell experience.

Below is an explanation of all of the pieces and how they all fit together:

# The .skn file:

This is perhaps the most important aspect of the UX package. This is a magical archive that contains all of the images, color 
data, and animations used by the Moonshell 2 system. It may seem like magic, but it's not. Each user interface element is created using a PNG with a transparent alpha layer, and these images have special labels. All of these images were hand made in GIMP, and other tools. Using a custom compiler, all of these images are collected and placed in this special archive. Then, the Moonshell kernal can recall these images quickly from the archive. 

# The splash.ani file:

As the name suggests, this is the data for the splash screen. It may look like an animated cursor file from the file container, but it's really once again a proprietary archive. Using stop motion animation, each frame of the splash screen is rendered by hand in a animation tool. Then, a special compiler places these images in a .ani file to be played back by the Moonshell kernal upon startup.

# The sndeff.dat file:

Once again, this is a custom archive. But what's in it? The SOUNDS. All of the sounds to make the UX scheme even more enjoyable are created and placed in a folder as .WAV. Then, a custom compiler places these sounds in a .DAT file for use on the system.


# The moonshell2.ini file:

This file is very important to the user interface. It tells the kernal what colors it will be using and what features should be turned on and turned off. It handles enabling of the sounds and splash screen. It also changes low level memory managment data.


# Setup.exe and LGWin.exe:

These files are the installers that surgically replace the UX data from Moonshell, with the new UX data for Looking Glass 5. Setup.exe extracts the files to a workarea on the destination SD Card, and then runs LGWin.exe. LGWin.exe then copies the files from that workarea to the correct locations deep in the Moonshell2 folder. After LGWin is finished, it deletes the temporary workarea.


# Final thoughts:

Looking Glass 5 was created by me to enhance the Moonshell 2 experience. Moonshell is a terrific operating system but it needed a facelift. Looking Glass 5 gives it that much needed transformation. 

Moonshell 2 has been discountinued and so has this project, but it does serve as an example of how to create a UX scheme for a very proprietary system.

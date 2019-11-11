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

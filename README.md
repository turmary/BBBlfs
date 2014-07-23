BBBlfs
======

Beagle Bone Black Linux Flash System

This project provides a way to boot a BB Black or White(same SoC) via USB from a Linux machine. The project is developed during Google Summer of Code '13. 
For more information: http://www.google-melange.com/gsoc/proposal/review/google/gsoc2013/ungureanuvladvictor/1001

#Build
- sudo apt-get install libusb-1.0-0-dev
- make dirs
- make

The binary will be located in the bin folder.

Press the S2 button on the BBB/BBW and apply power to the board. The board should start now into USB boot mode. 

Connect the board to the host PC. The kernel should now identify your board as an RNDIS interface. Be sure you do not have any BOOTP servers on your network.

Go to bin/ and execute runscript.sh. It needs the flashing image as argument to be provided.
#Usage
- sudo ./runscript.sh debian.img.xz

If there are bugs please feel free to contact me.


#Contact
ungureanuvladvictor@gmail.com
vvu or vvu|Mobile on #beagle, #beagle-gsoc


## AFM fixing progress

The central issue is the laser spot metering: With the Quadrex extension, the signal sum is stuck at 10V. When removing the Quadrex, the signal sum is following the expected intensity when moving the laser across the tip. However, without the quadrex the vertical deflection remains 0. I am not sure if this is another bug, indicating that there are more things broken. 

## Parts

# Necessary
Back panel
Nanoscope Controller IIIa
Head
Long Cable from Nanoscope Controller to Back panel

# Not necessary
Quadrex Extender
Signal Access Module
PC controller

## what I tried
#swapping components
Mark Smith from afmservicesllc@gmail.com is awesome! He sent us all necessary components (Controller, Back panel, cable, and PC controller (which I didn't try)). We have to return it to him ( 81 David Love Place Suite F Goleta CA 93117). I also shipped the AFM head to him and he confirmed (?) that it worked (which is not what I confirmed as seen below).
# measuring operation
Thanks to Manu from Support.AFM@bruker.com I got several manuals that allowed me to measure the signal on the boards without the PC.
I could confirm that the signal is not arriving in the Nanoscope controller. 

Also, Josh and I pulled out the wiring from the head to supply +-15V and 5V/0V from the back panel to the head. Then, we measured the photodiode signal directly and found that SDA/SDB are stuck at 15V when moving the laser spot while SDC/SDB would be proportionally controlled.

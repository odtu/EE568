# EE568 Project-3

## PM Motor Comparison Analysis

## Deadline 03/05 23:59

In this assignment you are going to design several surface-mount PM machines with the following constant parameters:

**Constant Parameters:** 

- Number of phases: 3 
- Number of poles: 4
- Motor Axial Length: 100 mm
- Air-gap clearance: 1 mm 
- Magnet to Pole Pitch Ratio: 0.8

### Q1- Magnetic Loading

In this part you are going to design a NdFeB magnet machine with the following parameters:

- Magnet Type: NdFeB N42 grade (ur=1.05), radial shaped
- Rotor Diameter: 100 mm 
- Magnet Radial Thickness: 4 mm 

a) Assume you have a solid stator in this part, draw the magnetic equivalent circuit for one pole-pair. Draw the load line and operating point on the B-H characteristics of the magnet. Also analytically calculate the peak air-gap flux density.

b) Calculate the magnetic loading of the machine for this condition

c) Draw the radial air-gap flux density distribution in the middle of air-gap clearance for a one pole-pair using an FEA tool and compare it with your analytical calculations.

### Q2- Electrical Loading & Machine Sizing

a) Choose a suitable number of slots for this machine. Discuss and justify your choice. Please assume open slot shape for the analysis. 

b) Assume the coil current is 2.5 A. If the  maximum current density is 5 A/mm^2 and maximum fill factor is 0.6, choose a suitable AWG cable.

c) Choose a reasonable slot height, number of coils per slot and a back-core thickness that does not saturate the core. You can use the rule-of-thumbs presented in the lecture and verify your decisions.

d) Calculate the electrical loading for your design and compare with the usual values presented in the lecture.

e) Calculate the average tangential stress in the rotor surface, total force that your design can produce.

f) Assuming a rotor speed of 1500 rpm, calculate the expected power output of your machine.


### Q3- Comparison & Optimization

In this part, assume the **stator outer diameter is fixed to 160 mm**, and the rotor diameter and other parameters are variable according to your design. You can assume open slots for this part, rectangular teeth shape is suggested, but please mention and justify any other slot-tooth shape combinations.

a) Try to estimate the optimum rotor diameter and slot ratio for maximum torque output. Calculate the required parameters (electrical loading, magnetic loading, stress etc.) analytically and verify your design in FEA and compare it to the machine you designed in Q1&Q2.

b) Now assume you replaced the NdFeB magnet with Ferrite magnets (Brem=0.4 T) as in the reading material (14/04),  while keeping all the dimensions same with the previous part, calculate the machine performance and compare it with the NdFeB design.

c) In this part, try to optimize the Ferrite machine by changing the parameters, but the outer diameter is still fixed to 160 mm. Choose the rotor diameter, magnet thickness, slot/tooth ratio to find the maximum torque output.  Present a comparison between NdFeB and Ferrite machines and justify your design decisions. Compare parameters like volume, copper cost, magnet cost etc.


## Useful Software

- [Motor Analysis](http://motoranalysis.com/)
- [FEMM](http://www.femm.info/wiki/HomePage)
- [X-FEMM](https://sourceforge.net/p/xfemm/wiki/Home/)
- [ANSYS Maxwell](https://www.ansys.com/products/electronics/ansys-maxwell)

There are also other software and useful links in the course web page.

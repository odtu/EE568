# EE568 Project-2

## Motor Winding Design & Analysis

## Deadline 29/05 23:59

## Grading and Procedure

See the [Evaluation](./evaluation.md) sheet for details. Please see the useful links and tips below.


### Q1- Integral-Slot Winding Design

Assume you have a 6-pole, 72 slot, 3-phase machine with double-layer winding configuration. Design the following windings for this machine:

- Full-pitched winding
- 11/12 short-pitched winding

For these winding configurations:

a) Show the winding diagram layout (just one pole-pair is enough)
b) Calculate the distribution factor, pitch factor and the winding factor for the fundamental component
c) Repeat the same for the 3rd and the 5th harmonics
d) Comment on the results

### Q2- Fractional-Slot Winding Design

In this part, you are going to analyze a 3-phase permanent-magnet synchronous machine with a fractional-slot winding. 

There are 5 different designs taken form the textbook "Brushless Permanent Magnet Motor Design, Dr. Duane Hanselman". You can find the your assigned design by taking mod(5) of your student ID.

- Calculate the phase angle of the induced voltage in each slot, and present them with a table.
- Draw the phasor diagram for one phase, and calculate the winding factor.
- Repeat the same procedure for the 3rd and 5th harmonics and comment on the results.
- Draw the winding diagram for all phases and verify you have a valid and balanced winding diagram.

### Q3 - Analytical Modelling

- Electrical loading
- Carter's coefficient
- Effective axial length
- Airgap peak magnetic flux density (no detailed calculation, just assume cylindrical rotor and stator by using Carter's coefficient)
- Choose a suitable number of turns, and calculate the induced voltage per phase

### Q4- 2D FEA Modelling

Using a computer tool (some suggestions are presented in the course webpage), verify the fractional-slot winding design. The specs for the machines are given below. 

Please don't try to optimize your design, a working design is enough.

Try to obtain at least the following (you can present more results if you like).

- Flux density distribution in the machine core (you are encouraged to use symmetry and boundary planes, but you can model the whole machine).
- Air-gap flux density distribution
- Flux-per-pole calculations (bonus: compare analytical and FEA results)
- Induced voltage waveforms (for phase and line-to-line) at rated speed
- Cogging torque (i.e. torque when there is no current in the windings)


### Common Specs

The specs are taken from "Brushless Permanent Magnet Motor Design, Dr. Duane Hanselman"

- The stator outside radius is Rso =50mm.
- The motor axial length is Ls/=100mm.
- The rotor outside radius Rm is chosen to maximize motor constant Km.
- The stator tooth body width (wtb), stator yoke width (wsy), and rotor yoke width (wry) are adjusted to keep the peak flux density in the regions close to 1.4T.
- No skewing of magnets or stator slots is employed.
- The ferromagnetic portions of the motor are constructed using common, high quality electrical steel.
- The radial magnet length is lm=4mm and the air gap length is g=lmm.
- The magnets are radially magnetized and operate at Br =1.3T and has a relative permeability of 1.05.
- The angular magnet pole width is set to 160° electrical, which gives a magnet to pole ratio of 160°/180°=0.89.
- The covered wire slot fill factor is set to kwc=60%.
- The phase currents are sinusoidal.
- The conductor current density is set to J=5Arms/mm2 .
- The windings operate at a temperature of 50°C.



## Useful Software

- [Emetor Winding Calculator](https://www.emetor.com/windings/)
- [Dolomites](https://gitlab.com/LuigiAlberti/dolomites-python): It has a few useful design snippets that you can refer.
- [Motor XP](https://www.mathworks.com/products/connections/product_detail/motorxp.html)
- ANSYS Maxwell, Rmxprt, MotorCad
- [Florence Meier PhD Thesis](http://www.diva-portal.org/smash/get/diva2:332/FULLTEXT01.pdf)

There are also other software and useful links in the course web page.

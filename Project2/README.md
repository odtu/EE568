# EE568 Project-2

## Motor Winding Design & Analysis

## Deadline 01/06 23:59

## Grading and Procedure

See the [Evaluation](./evaluation.md) sheet for details. Please see the useful links and tips below.


### Q1- Integral-Slot Winding Design

Assume you have a 6-pole, 72 slot, 3-phase machine with double-layer winding configuration. Design the following windings for this machine:

- Full-pitched winding
- 11/12 short-pitched winding

For these winding configurations:

- Show the winding diagram layout (just one pole-pair is enough),
- Calculate the distribution factor, pitch factor and the winding factor for the fundamental component,
- Repeat the same for the 3rd and the 5th harmonics,
- Comment on the results.

### Q2- Fractional-Slot Winding Design

In this part, you are going to analyze a 3-phase permanent-magnet synchronous machine with a fractional-slot winding. 

There are 5 different designs taken form the textbook "Brushless Permanent Magnet Motor Design, Dr. Duane Hanselman". You can find the your assigned design number by taking mod(5) of your student ID. The full specs for the machines are given below. 

- Calculate the phase angle of the induced voltage in each slot, and present them with a table,
- Draw the phasor diagram for one phase, and calculate the winding factor,
- Repeat the same procedure for the 3rd and 5th harmonics and comment on the results,
- Draw the winding diagram for all phases and verify you have a valid and balanced winding diagram.

### Q3 - Analytical Modelling

For the machine model, calculate the following analytically, show your calculations and explain where necessary.

- Electrical loading of the machine,
- Carter's coefficient (i.e. the factor for converting stator slots into a solid cylinder, no need to do for the rotor as it is a surface-mount topology), and effective air-gap clearance,
- Effective axial length of the machine,
- Air-gap peak magnetic flux density (no detailed calculation in this stage, just assume cylindrical rotor and stator by using Carter's coefficient). You may use analytical PM calculations and basic assumptions,
- Magnetic loading of the machine, specific machine constant, shear stress in the rotor and expected torque of the machine,
- Flux per pole (Although you are not required to choose a number of turns, you may choose it for a DC bus of 48 V and a rated speed of 1500 rpm).

### Q4- 2D FEA Modelling

Using a computer tool (some suggestions are presented in the course webpage), verify the flux density distribution and your fractional-slot winding design. 

Please don't try to optimize your design, a working design is enough for this project.

Try to obtain at least the following (you can present more results if you like).

- Flux density distribution in the machine core (you are encouraged to use symmetry and boundary planes, but you can model the whole machine). Especially verify the maximum flux density points in the teeth and back-core,
- Air-gap flux density distribution (plot it at the middle of the air-gap, not at the stator or rotor surface),
- Show a few leakage flux paths (ie. magnet-to-magnet, in-slot, magnet-tooth-magnet etc.) and comment on them,
- Flux-per-pole calculations (make sure the rotor position is aligned to give the maximum flux, and don't forget to multiply your 2D results with the effective axial length). Bonus: compare your analytical results from the previous part and FEA results),
- Bonus: Cogging torque as a function of the rotational angle (i.e. torque when there is no current in the windings).

### Common Specs

The specs are taken from "Brushless Permanent Magnet Motor Design, Dr. Duane Hanselman"

- The stator outside radius is Rso = 50mm.
- The motor axial length is Ls = 100mm.
- The rotor outside radius Rm is chosen to maximize motor constant Km.
- The stator tooth body width (wtb), stator yoke width (wsy), and rotor yoke width (wry) are adjusted to keep the peak flux density in the regions close to 1.4T.
- No skewing of magnets or stator slots is employed.
- The ferromagnetic portions of the motor are constructed using common, high quality electrical steel.
- The radial magnet length is lm = 4mm and the air gap length is g = 1mm.
- The magnets are radially magnetized and operate with a remanence flux, Br = 1.3T and has a relative permeability of 1.05.
- The angular magnet pole width is set to 160° electrical, which gives a magnet to pole ratio of 160°/180° = 0.89.
- The covered wire slot fill factor is set to kwc = 60%.
- The phase currents are sinusoidal.
- The conductor current density is set to J = 5Arms/mm2 .
- The windings operate at a temperature of 50°C.

### General Tips

- This project is time-consuming, so start early.
- Avoid over-calculating or over-optimizing. The evaluation will focus on your methodology and whether you understand the concepts—not on the precision of your calculations.
- A flexible Excel file (or a MATLAB script) that allows you to adjust parameters easily can be more useful than manual calculations. You are encouraged to develop additional tools (e.g., Excel files, MATLAB scripts, or vibe-coded scripts) for your analysis, but be sure to submit them with your project.
- You may use any FEA tools you prefer; FEMM and ANSYS are among the most suitable options.
- Ensure that the magnets are magnetized in the correct sequence (North–South–North–… in the radial direction). If you encounter difficulties when modeling magnets or slots, you may simplify the geometry (e.g., use rectangular magnets or open slots).
- The number of mesh elements is not highly critical, but ensure that the mesh between the rotor and stator is sufficiently fine. This will not only improve the visual quality of your results but also increase their accuracy.
- You are encouraged to do group work, but each student is responsible for submitting (and understanding) their own work. The same [evaluation rules of Project-1](../Project1/evaluation.md) will be applied.

## Useful Software

- [Emetor Winding Calculator](https://www.emetor.com/windings/)
- [Dolomites](https://gitlab.com/LuigiAlberti/dolomites-python): It has a few useful design snippets that you can refer.
- [Motor XP](https://www.mathworks.com/products/connections/product_detail/motorxp.html)
- ANSYS Maxwell, Rmxprt, MotorCad
- [Florence Meier PhD Thesis](http://www.diva-portal.org/smash/get/diva2:332/FULLTEXT01.pdf)

There are also other software and useful links in the course web page.

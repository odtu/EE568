# EE568 Project-2

## Motor Winding Design & Analysis

## Deadline 31/03 23:59

## Grading and Procedure

See the [Evaluation](./evaluation.md) sheet for details. Please see the useful links and tips below.

### Q1- Integral-Slot Winding Design

Assume you have a 20-pole, 120 slot, 3-phase machine. Design a winding (can be full-pithced or short-pitched).

- Show the winding diagram (just one pole-pair is enough)
- Calculate the distribution factor, pitch factor and the winding factor for the fundamental component
- Repeat the same for the 3rd and the 5th harmonics
- Comment on the results

### Q2- Fractional-Slot Winding Design

In this part, you are going to analyze a 3-phase permanent-magnet synchronous machine with a fractional-slot winding. 

Choose a pole number of 20 or 22. For this pole number, choose a slot number between 20 and 30. You can use [Emetor Winding Design](https://www.emetor.com/windings/) for an initial design.

- Calculate the phase angle of the induced voltage in each slot, and present them with a table.
- Draw the phasor diagram for one phase, and calculate the winding factor.

- Repeat the same procedure for the 3rd and 5th harmonics and comment on the results.

Now for the same pole number you had choosen, choose a different slot number. This choice would not be as good as the first one, but still should be a viable one.

- Repeat the same analysis with the previous one.

- Compare the results of the two designs and comment in detail.


### Q3- 2D FEA Modelling

Using a computer tool (some suggestions are presented in the course webpage), verify one of your designs with the fractional-slot winding. For reference you can use the same parameters given at the last section of your textbook (Hanselman). Alternatively you can use any other designs you found in the literature (but please give reference if you used someone else's design). Please don't try to optimize your design, a working design is enough.

Try to obtain at least the following (you can present more results if you like).

- General 2D drawing and winding diagram of your design
- Airgap flux density distribution
- Induced voltage waveforms (for phase and line-to-line) at rated speed
- Cogging torque


## Useful Software

- [Emetor Winding Calculator](https://www.emetor.com/windings/)
- [Dolomites](https://sourceforge.net/projects/dolomites/): It has a few useful design snippets that you can refer.
- [Homebuilt ELectric Motors](http://www.bavaria-direct.co.za/scheme/calculator/)
- [Florence Meier PhD Thesis](http://www.diva-portal.org/smash/get/diva2:332/FULLTEXT01.pdf)

There are also other software and useful links in the course web page.

 

### Lamination Selection

In the project folder you'll find the several induction motor laminations from [Kienle Spiess](http://www.kienle-spiess.de/induction-machines.html). Please select a lamination. Although, students are allowed to work on same laminations, I don't want close friends to work on the same lamination. I expect you to work independently, and there is no difference of difficulty between laminations. 

You can find the definitions of the parameters in the legend file. You can also get registered in [Kienle Spiess](http://www.kienle-spiess.de/induction-machines.html) to get extra information. Throughout the assignment, please ignore small features of the drawings (i.e. drill holes, shaft opening, tolerances, fillet radius etc).

You can select any lamination material, but please refer to the data-sheet of the material and thickness you choose.


## Q1) Winding Design

For the lamination you had chosen, depending on the number of stator slots and rotor slots, design a winding diagram including but not limited to:

- Number of poles
- Type of winding (integral, fractional, single layer, double layer etc.)
- Winding diagram
- Winding factors (including first few harmonics)
- Number of turns, and wire size
- Fill factor
- Winding connection (delta-wye)
- Aimed voltage and current ratings

For the winding you selected please plot the MMF waveform for two different instants for a balanced three-phase current (i.e. Ia=1 A, Ib=-0.5 A, Ic=-0.5A) ignoring rotor slots for this stage.

## Q2) Motor Parameter Estimation

Choose an axial length for the lamination. Also choose an airgap clearance value (reduce the rotor diameter appropriately).  There is not a definite answer, but please try to choose reasonable numbers. Then determine the following:

- Choose (calculate) the specific magnetic loading and also the flux densities in stator teeth, stator back core.
- Determine (calculate) the specific electric loading (in the last step you will be required to verify these)
- Calculate the approximate torque and speed of your design based on your assumptions
- Calculate the equivalent circuit parameters for your design (i.e. phase resistance, phase inductance, leakage inductance etc.)
- Calculate the approximate core and copper losses at the rated operating conditions.

You can find useful examples in your handouts and also [in this link](http://www.ssmengg.edu.in/weos/weos/upload/EStudyMaterial/electrical/6thsem/Machine%20design(ELE-603)/Electrical%20Machine%20Design%20Unit6VH.pdf).


## Q3) Detailed Analysis & Verification

Using a computer tool (some suggestions are given below), verify the analytical designs. Try to obtain the following and any other relevant data you may suggest:

- Torque-Speed Characteristics
- Flux density distribution at different conditions
- Current waveforms at rated conditions
- Efficiency curves 
- Equivalent circuit parameters
- Effect of skewing etc.

## Useful Software

Apart from the analytical calculations you are required to use software tools to verify your calculations.

- [ANSYS Maxwell](https://www.ansys.com/products/electronics/ansys-maxwell): Especially the RmXprt toolbox of Maxwell will the most useful option. You can also use Maxwell 2D simulations for flux density calculations.
- [MotorAnalysis](http://motoranalysis.com/): A free MATLAB GUI for induction motor design. Although it may be slow for some cases, it is easy to use and simple tool.
- [Dolomites](https://sourceforge.net/projects/dolomites/): It has a few useful design snippets that you can refer.

There are also other software you can use in the course web page.

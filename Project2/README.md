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

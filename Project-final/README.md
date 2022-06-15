# EE568 Final Project

### Deadline: 07/07/2022 23:59

In this assignment you are going to design and analyze a machine that you choose, or the one from the templates given below. The machine topologies can be different, so this is a general guide about the content of your project.

All rules regarding the report format, Github repo and number of commits still hold **(10pts)**. Please do your own work. You need to submit a PDF report summarizing all the works you did, please discuss any important points and state any assumptions you make. Reports that give just the analysis and FEA results without enough discussion and comments get a low grade.


### Literature Review **(15pts)**

In this section, I expect you to summarize the current status of the literature on your machine topology. Please read and summarize journal papers that are relevant to your machine topology. Please cite at least 5-6 recent SCI journals, discuss and synthesize them properly. 

- https://www.scribbr.com/dissertation/literature-review/
- https://writingcenter.unc.edu/tips-and-tools/literature-reviews/

### Analytical Calculation & Sizing **(25pts)**

In this part, please discuss the relevant analytical calculations, and give the details for the rough sizing of the machine. These can be listed as (but not limited to):

- Choose a specific machine constant by choosing proper values for  the magnetic and electrical loading, current density etc.
- Define the rough dimensions (airgap clearance, rotor diameter, axial length) 
- Choose the winding configurations (number of slots, number of coils, cable size etc.)
- Calculate the other parameters such as the teeth/slot dimensions, back-core thickness etc.
- Material selection (laminations, magnet grade etc.)
- Electrical circuit parameter estimations (induced voltage, flux per pole, phase resistance, phase inductance etc.)


### FEA Modelling **(30pts)**

Model your analytical design using a FEA software. 2D analyses should be fine for this project, but for some topologies 3D FEA analysis may be more accurate. If this is the case, you may simplify the model by using rotational symmetry or linear materials etc.

In this part, please present and discuss the following:

- Air-gap flux density distribution
- Flux density distribution in the critical parts such as back-core, stator teeth etc.
- Phase resistance (in the 2D FEA calculations  don't forget  to include the end-winding) 
- Phase inductance (if our machine has saliency please calculate d-axis and q-axis inductances separately) 
- Induced phase voltage (you don't have to make a transient analysis, but use magneto-static analysis to calculate the flux per-pole at various rotor positions and approximate the induced phase voltage) 
- Efficiency calculation at rated load and half-load (please include the temperature effects, core losses etc.)

### Comparison & Discussion **(20pts)**

In this stage, if you see any unfeasible designs please go back to the analytical model and modify your design. I expect to be a few iterations (changing a few parameters etc.), please reflect and discuss these in the report. Compare the analytical and FEA models clearly and discuss any discrepancies. 

If you tried a few different designs, such as with different pole number, magnet grade, rotor diameter, slot/tooth dimensions etc. Please give a comparison between these designs, and summarize why you choose the final design.

Also in this part, please give main mechanical parameters of the machine:

- Outer Diameter, axial length, aspect ratio 
- Material mass (iron, copper, magnet)
- Torque density, power density



## Machine Design Options


You are free to either choose a design from the options below or  propose another motor/generator design problem. If you want to complete the project with a custom design, please email with the specs, topology etc. no later than 19/06 and get my approval.

Please fill your preferred design into this [spreadsheet](https://docs.google.com/spreadsheets/d/14sv7CdKSjpOYbqJVdYcRRiru_I93UjyO_biOcn4TH3E/edit?usp=sharing) until 19/06.
Any students who didn't make a choice by then will be randomly assigned a design from the options below:

### A: Direct-Drive PM Generator

- Rated Power: 1 MW
- Rated Speed: 18 rpm
- Surface mount radial flux PM machine
- Line voltage: 3.3 kV
- Natural air cooling
- Design objective: a light machine and low cost machine (beware of PM cost)

### B: BMW i-3 Motor

- Rated Power: 125 kW
- Maximum Torque: 250 Nm
- Rated Speed: 5000 rpm (can go up to 16000 rpm at rated power with reduced torque)
- Nominal battery voltage: 800 V
- Synchronous reluctance machine (or you may design as IPM machine or PM assisted synchronous machine)
- Liquid cooled system
- Design objective: achieve a high power density without sacrificing efficiency

### C: Hydro-Electric Generator

- Rated Power: 44 MVA (0.9 pf lagging)
- Rated Speed: 187.5 rpm
- Rated voltage: 13.800 V (line-to-line)
- Salient-pole synchronous generator
- Air-forced cooling

 ## Useful Software

- [Motor Analysis](http://motoranalysis.com/)
- [FEMM](http://www.femm.info/wiki/HomePage)
- [X-FEMM](https://sourceforge.net/p/xfemm/wiki/Home/)
- [ANSYS Maxwell](https://www.ansys.com/products/electronics/ansys-maxwell)

There are also other software and useful links in the course web page.

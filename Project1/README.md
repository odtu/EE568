# EE564 Project-1

## Torque in a Variable Reluctance Machine

## Deadline 17/04 23:59

## Grading and Procedure

See the [Evaluation](./evaluation.md) sheet for details.

Assume you have a variable reluctance machine as shown in the figures below:

![core](./core.jpeg)

![dimensions](./dimensions.jpeg)

- Coils are wound within 30 mm x 10 mm rectangle areas
- Each airgap clearance is 0.5 mm
- Depth of the core is 2 0mm
- Number of turns = 250
- Coil Current = 3 A DC

## Q1) Analytical modelling

a) Calculate analytically the maximum and minimum reluctance (and inductance) as the rotor makes a full rotation. You can make necessary assumptions to simplify your calculations, please please state them explicitly. You may assume the core is infinitely permeable for this section. Please obtain and plot the inductance variation as a function of rotation. You may assume sinusoidal variation.

b) Derive and plot the torque generated in the system under constant DC excitation.

c) Suggest a method to improve your model by including non-linear effects (fringing flux, non-homogeneous flux distribution) etc. A detailed description is enough, a full derivation is not required.

## Q2) FEA Modelling (2D - Linear Materials)

Model the system in a 2D FEA software (you can use any software you want, please have a look at the options at the course page).

Here are a few suggestions:

- If you haven't used any FEA software before, I advise you to start with FEMM, which is free and a simple program. If you are planning to use FEA simulations in your professional life, then it makes sense to learn a more capable program (e.g.  ANSYS Maxwell)

- 2D simulations will be enough for assignments in this course. If you feel comfortable, you can proceed with the bonus 3D simulations (you have been warned).

- You can approximate the coils by solid copper regions (i.e. you don't have to model each number of turns),  you can model each coil as a bonus to have a better understanding of leakage flux.

- There are a few people already using FEA software, if you feel stuck, please ask for help. The solution is usually very simple.

For this part choose a realistic electric steel lamination (you can use software library or use real material data-sheets). For this part assume the material is LINEAR (i.e. assume permeability is constant).

a) Draw the flux density vectors for three positions (0, 45, 90 degrees), adjust the scales so the figures are readable.

b) Calculate the inductance, and stored energy in the system for these three positions.

c) Derive the torque generated in your system as a function of rotation angle for at least ten positions. Compare your results with the analytical model results from part-1.


## Q3) FEA Modelling (2D - Nonlinear Materials)

In this section, use the same model, but make the material properties NON-LINEAR (i.e. permeability will change as the core saturates).

a,b,c) Repeat the same procedures as in Q2)

d) Compare the effects of fringing and saturating effects with the linear and non-linear materials by presenting the FEA results.


## Q4) Control Method

Propose a control method to enable continuous rotation. You can use an on/off DC current, square wave, sinusoidal excitation as you like. Show a positive torque can be generated  by using your analytical model and also your 2D models. Present any graphs or FEA results to prove your point.


## Q5) Bonus-I (Motion Animation)

Prepare a short video, or .gif image to animate the rotation of the rotor. You can use the conditions in Q3, or Q4. In the animations show the flux density variation (either lines or vectors) in the core during rotation.

## Q6) Bonus-II (3D FEA Analysis)

For this part, repeat your simulations in 3D with non-linear material properties. Compare your results with the analytical and 2D FEA results. Compare and discuss the effects of fringing and leakage flux that are mode accurately modelled in 3D. 


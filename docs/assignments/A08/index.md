# A8 – Gearbox Design

## Objective

For this assignment, we are to design and parametrically model parts for a gearbox, including a shaft design for strength. The design should be able to be assembled and disassembled without failure. The objective list is as follows.

- Design a gearbox that can be assembled and disassembled.

- Analyze and size input and output shafts for strength.

- Design journal bearings to support shafts.

- Create a gearbox housing with proper clearance and fastening.

- Use parametric CAD modeling to generate a final design.

- Document calculations, sketches, and lessons learned.

The spur gears have a gear ratio of 24:9 and are listed in the resource section. The output gear torque and speed are to be 1.25 in-lbf and 1100 rpm, respectively. The input (pinion,power-transmission) and output (gear, short shaft) shaft diameters are .125 and .25 inches, respectively, and each has a length of 1 inch.

Assumptions

- Assume appropriate strength of shafts, use Machinery’s Handbook.

- The gear train is ideal.

- The moment of the radial force from the gear train is small enough to be ignored.

## Known and Unknown Values

<img width="4284" height="5712" alt="IMG_1901" src="https://github.com/user-attachments/assets/4664186c-2625-4c1f-abeb-caa231195959" />

I started y doing a list of all the given/known values and all the values I need to solve for. 

## Calculations

<img width="4284" height="5712" alt="IMG_1902" src="https://github.com/user-attachments/assets/c8b86ac2-98c0-4c73-86d1-f491c3831794" />

Before begining design I had to solve for all the unknown values. I started by solving for the gear ratio by divifing the number of teeth on the output shaft pinion by the number of teeth on the input shaft gear and got 2.667 rotations on the input shaft for every one rotation on the output shaft. I then solved for the input rotational speed. I set the gear ratio equal to the rotational speed ratio and solved for input shaft speed and got 2933.33rpm. Next was the input shaft torque. We know the output torque is equal to 1100in*lbf. We also assume this is an ideal shaft with no power loss. So I set the tourque in times the rotational speed in equal to torque out times rotational speed out and solved for torque in. I got a value of .4688in*lbf. Lastly I solved for the shaft shear stress. I got that theshear stres of the input shaft is 1222.44psi and the output shear stress is 407.44psi. Both the values are under the maximum allowed stress values.
## Communicate


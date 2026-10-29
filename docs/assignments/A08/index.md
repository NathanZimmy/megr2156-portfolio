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

I started by making a list of all the given/known values and all the values I need to solve for. 

## Calculations

<img width="4284" height="5712" alt="IMG_1902" src="https://github.com/user-attachments/assets/c8b86ac2-98c0-4c73-86d1-f491c3831794" />

Before beginning the design, I had to solve for all the unknown values. I started by solving for the gear ratio by dividing the number of teeth on the output shaft pinion by the number of teeth on the input shaft gear and got 2.667 rotations on the input shaft for every one rotation on the output shaft. I then solved for the input rotational speed. I set the gear ratio equal to the rotational speed ratio and solved for input shaft speed and got 2933.33rpm. Next was the input shaft torque. We know the output torque is equal to 1100 in-lbf. We also assume this is an ideal shaft with no power loss. So I set the torque in times the rotational speed in equal to the torque out times the rotational speed out and solved for torque in. I got a value of .4688in-lbf. Lastly, I solved for the shaft shear stress. I got that the shear stress of the input shaft is 1222.44psi and the output shear stress is 407.44psi. I found the input max to be 4000psi and the output max to be 8500psi, so both of my calculated values are sufficient. 

### Free Body Diagrams

<img width="227" height="76" alt="image" src="https://github.com/user-attachments/assets/ac128e8a-8e85-4ae6-a65d-bf589a4c977b" />

### Safety Factor check

<img width="248" height="112" alt="image" src="https://github.com/user-attachments/assets/3c488407-3cdd-4d56-9253-c2e1ce3d1ef5" />

Using the strength values found in the book, I calculated the safety factors of each shaft, and both are acceptable. 

### Diameter check

<img width="187" height="273" alt="image" src="https://github.com/user-attachments/assets/7d21b0aa-073d-442e-9d6c-f702d41fb027" />

Using the equations given in class, I found that both the input power and output power are within the acceptable range, and both shaft diameters are of sufficient size. 

## Journal Bearings


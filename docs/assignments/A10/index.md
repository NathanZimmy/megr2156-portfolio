# A10 – Lead Screw Design

## Objective


## Analyze


## Decide
_Reference your concept selection (Pugh matrix) here. How does this design follow from that decision?_

## FEA on Crosshead

For this section, we are to run FEA on our crosshead to evaluate stiffness and strength under a 2KN axial load. We are to use our results to optimize the geometry by reducing weight and stress concentrations using fillets, changing thickness, or cutting extra material out. 

<img width="600" height="475" alt="image" src="https://github.com/user-attachments/assets/27555967-2c67-428a-8bd2-c0e96737886c" />

We are using 6061-T6-SS which is an aluminum alloy with a yield strength of 275Mpa and a modulus of elasticity of 69000Mpa so we will have to keep the design within these material properties. 

<img width="920" height="367" alt="image" src="https://github.com/user-attachments/assets/e6809634-54ee-4ef9-a64a-fd964ac8ada2" />

<img width="800" height="352" alt="image" src="https://github.com/user-attachments/assets/21af7a46-a1cb-44a4-86c0-e802ead049a5" />

I started by adding fixed geometries to all the screw holes where the crosshead will be mounted assuming the screws are perfectly rigid in this assignment. This will hold those ends in place. Then I added a force on the center hole of 2KN or 2000N and set it 

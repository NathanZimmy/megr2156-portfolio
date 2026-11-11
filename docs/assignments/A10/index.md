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

I started by adding fixed geometries to all the screw holes where the crosshead will be mounted assuming the screws are perfectly rigid in this assignment. This will hold those ends in place. Then I added a force on the center hole of 2KN or 2000N and clicked selected direction. this is because if I simply click the holy the force will be applied in all directions around the circumference of the cylindrical hole. So, with using selected direction I can click the top surface and have the force be pointed downwards through the hole which is where the part that is being tested will be applying the force onto the crosshead. 

### Test 1

<img width="803" height="377" alt="image" src="https://github.com/user-attachments/assets/49acd147-e292-47f2-b2fa-813a2c5cb2db" />

<img width="755" height="367" alt="image" src="https://github.com/user-attachments/assets/f2a7f7f9-c8e9-4d05-83e2-ad528ca56d5d" />

<img width="755" height="356" alt="image" src="https://github.com/user-attachments/assets/c0887c18-d891-4986-839b-cd1f4b4238f3" />

<img width="277" height="243" alt="image" src="https://github.com/user-attachments/assets/d21b2528-6e01-49fe-822f-83fad6af97b3" />

After running the first test we can see that we have no strain and our deflection is very little having a max of .005mm which is pretty much negligible. However, our max stress is 10257662N/M^2 but it is a huge stress concertation at the innermost screw holes with the rest of our model having a much less stress.  

For this first test I did not edit the mesh and left it as was.

### Test 2

<img width="818" height="370" alt="image" src="https://github.com/user-attachments/assets/67c8d6c5-1bab-46aa-a350-a89ae0754a46" />

For this second test all I did was change the max element size of the mesh to .6in making it more fine to see how the values would change before I edit the model. 


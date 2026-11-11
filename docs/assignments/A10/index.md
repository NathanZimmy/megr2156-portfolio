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

### Test 0.1

<img width="803" height="377" alt="image" src="https://github.com/user-attachments/assets/49acd147-e292-47f2-b2fa-813a2c5cb2db" />

<img width="755" height="367" alt="image" src="https://github.com/user-attachments/assets/f2a7f7f9-c8e9-4d05-83e2-ad528ca56d5d" />

<img width="755" height="356" alt="image" src="https://github.com/user-attachments/assets/c0887c18-d891-4986-839b-cd1f4b4238f3" />

<img width="277" height="243" alt="image" src="https://github.com/user-attachments/assets/d21b2528-6e01-49fe-822f-83fad6af97b3" />

After running the first test we can see that we have no strain and our deflection is very little having a max of .005mm which is pretty much negligible. However, our max stress is 10257662N/M^2 but it is a huge stress concertation at the innermost screw holes with the rest of our model having a much less stress. But this value is okay because our material yield strength is 275 Mpa or 275000000pa so we are way under this value. 

For this first test I did not edit the mesh and left it as was.

### Test 0.2

<img width="818" height="370" alt="image" src="https://github.com/user-attachments/assets/67c8d6c5-1bab-46aa-a350-a89ae0754a46" />

<img width="569" height="203" alt="image" src="https://github.com/user-attachments/assets/def012ab-b614-4a99-82c7-aa567b825514" />

For this second test all I did was change the max element size of the mesh to .6in making it more fine to see how the values would change before I edit the model. 

<img width="767" height="353" alt="image" src="https://github.com/user-attachments/assets/3338d9b0-8574-4271-837b-2b88edfd00b2" />

<img width="730" height="365" alt="image" src="https://github.com/user-attachments/assets/25a79eb7-9dca-4e84-9080-279195d2e6c0" />

<img width="739" height="362" alt="image" src="https://github.com/user-attachments/assets/82d4a22f-a150-4e05-bebc-18eb0d6128b5" />

After changing the mech size to a smaller element size the stress concentration went up but the other values stayed the same. So we know the screw holes are where the problems are and we also know the average stress throughout the model is very low compared to the max which will allow us to cut out some of the material. 

### Optimization 1

<img width="521" height="289" alt="image" src="https://github.com/user-attachments/assets/c6e63ccb-24cb-4d3a-8ebe-d27719d0fc73" />

To try and reduce the stress on the screw hole I added a .1in fillet on all the holes . 

#### Test 1.1

<img width="770" height="358" alt="image" src="https://github.com/user-attachments/assets/be5f889e-e376-4cc5-b3f8-c3d6166456b0" />

After adding the fillets and running another test we found that this actually raised our max stress by over 1 million pascals. While this isn't what we were going for its okay because this is still way under our maximum yield strength. 

### Optimization 2

<img width="580" height="332" alt="image" src="https://github.com/user-attachments/assets/c0335c8c-f787-44a6-8212-9fa193a5ddc7" />

<img width="454" height="254" alt="image" src="https://github.com/user-attachments/assets/577954f7-91ec-474f-a948-aec8c34c5182" />

<img width="673" height="317" alt="image" src="https://github.com/user-attachments/assets/a9e44183-41cd-458d-adc9-f8236ab6068c" />

After seeing that most of the material in our crosshead undergoes almost no stress or deflection we wanted to remove some of the material to save on weight. So, I cut out sections in the center of the body and used the mirror feature to mirror the one sketch into four across both centerline. 

#### Test 2.1

<img width="581" height="290" alt="image" src="https://github.com/user-attachments/assets/98f89727-5dec-44a4-8cdc-9bc2e4d76586" />

<img width="575" height="289" alt="image" src="https://github.com/user-attachments/assets/94a147e9-1781-4889-8664-fbd44b5a82f1" />

<img width="649" height="333" alt="image" src="https://github.com/user-attachments/assets/e41c247e-f64a-46e4-bafc-820d21e0aaf7" />

After running another test the cutouts actually raised our stress and deflection but not by enough where it hurts our model.

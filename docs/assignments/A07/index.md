# A7 – [FEA on Bracket Design]

## Objective
In this assignment, I am going to take the bracket design from my previous assignment and use SolidWorks FEA (finite element analysis) on the design to improve and optimize it. Here is the objective list from the assignment. 

Your task is simply to create a high-stiffness, high-strength, and lightweight component. Use Finite Element Analysis to drive your decision-making process throughout your design. At each step of the analysis and before you make geometric changes, make sure the component’s results (stress/displacement/Safety Factor) converge to within a 7% difference. Achieve this by modifying the number of elements. If after three attempts to converge use the stiffness and stress from the finer mesh size use the finest mesh size and proceed through the process.

- Use Finite Element Analysis (FEA) to improve the bracket design from previous assignments.

- Ensure high stiffness, strength, and lightweight optimization through iterative design.

- Conduct multiple FEA simulations, refining geometry based on results.

- Perform static stress analysis, including constraints, loading, and meshing selection.

- Interpret data by identifying max stress, displacement, and safety factors.

- Optimize the design by modifying geometry to enhance performance.

- Document the entire process with images, calculations, and insights.

- Reflect on key engineering lessons learned and time spent.


## Initial Design

<img width="296" height="326" alt="image" src="https://github.com/user-attachments/assets/a6b5b0cb-8020-4678-bf43-6fd6a8ec38a7" />

Before running FEA or changing the design at all, here is the bracket I designed in the last assignment. 

<img width="596" height="446" alt="image" src="https://github.com/user-attachments/assets/f58a78b8-941f-475e-96d9-68a96fbb0d83" />

I also had to create and apply my chosen material. I chose to use Titanium Ti-6Al-4V. After applying the correct values for this material, I applied it to my bracket. 

## Design 1

### Fixtures and Forces
Before running the first study, I had to add fixtures to show where the bracket is undergoing force and being supported. This is so the study knows exactly what is happening to the design and where the stress concentrations are due to the forces acting upon it. 

<img width="442" height="278" alt="image" src="https://github.com/user-attachments/assets/86be065a-3af4-4637-b199-1ce260b01dd7" />

For the first fixture, I added a fixed geometry on the underside of feature E. This is to simulate something sliding into the bracket.

<img width="671" height="364" alt="image" src="https://github.com/user-attachments/assets/aed02de4-9259-485a-a718-f5e8fa684d9f" />

Next, I added a distributed force on Feature A, the cylinder. I chose the force to be equal to 600 lbf, and W = 2F, so the force will be 1200lbf. I selected the cylinder to be the shape the force is acting on, then one of the vertical corner edges for the direction it would be acting in. However, it kept going upwards, so I had to select it to reverse direction. Lastly, I changed it to English(IPS) units and set it to 1200lbf.

### Mesh 1.1

<img width="755" height="372" alt="image" src="https://github.com/user-attachments/assets/91518f96-44cd-427d-a4fc-c8fe992f1b1f" />

I added my first mesh and left all the settings completely as they were automatically set. This was to see what would happen and where my design currently sits. 

<img width="312" height="148" alt="image" src="https://github.com/user-attachments/assets/1036c76f-45b0-4d03-9e0a-c3df4c5a42ec" />

After creating my first mesh, I hit run to test the first study. However, I had this pop-up and had no idea what it meant or what to do, so I screenshot it and asked AI. AI told me that I didn't do anything inherently wrong, but that my design may be going through a very large displacement, with my force being 1200lbf. It notified me that I should hit no so I can analyze my initial geometry because hitting yes will automatically cause changes. 

### First simulation

<img width="568" height="355" alt="image" src="https://github.com/user-attachments/assets/d105dcbf-4094-4c76-ae54-2355f29a3562" />

<img width="501" height="344" alt="image" src="https://github.com/user-attachments/assets/d0c47629-7808-474e-9c22-2e0a66ce1fed" />

<img width="494" height="325" alt="image" src="https://github.com/user-attachments/assets/b943f40c-fa8a-4d35-9253-c17b465425ae" />

<img width="783" height="473" alt="image" src="https://github.com/user-attachments/assets/2a6c1a9e-6de0-41e8-8e2a-192be24e6bfa" />

Here are my first three simulation results; above, you can see the Von Mises (stress), displacement, and strain. I first noticed, after getting the error code before, the displacement values. Currently, it is showing that my bracket's max displacement is 1.244x10^5mm or 124.4m which is about 400ft. This is completely unrealistic and shows there is something wrong with the simulation or my model itself. So after doing some looking and showing AI my results of what went wrong, I found that my material had not saved. I also found that when creating my materials, I input the wrong values and made them 1000 times smaller by putting a decimal instead of a comma, so I fixed that as well. 

So after making sure my material was selected this time and double-checking that my model was all one solid body I ran the simulation again. 

<img width="341" height="300" alt="image" src="https://github.com/user-attachments/assets/ccc6b894-b2d8-4ca1-981f-8416a042a1c3" />

<img width="581" height="359" alt="image" src="https://github.com/user-attachments/assets/9efe61e1-b0f1-4855-9c5a-9258bf0b5da6" />

<img width="593" height="370" alt="image" src="https://github.com/user-attachments/assets/675df3e6-7db0-4328-8419-a6092dfad4ff" />

<img width="222" height="185" alt="image" src="https://github.com/user-attachments/assets/8af51ded-4802-45c7-bbfa-688cab87b526" />

After running the simulations again, my stress and displacement values were still way over the maximum allowed values. So, to start working towards fixing this, I added the chart annotation to show where the pinpoint maximum values were. I also got my mesh details so I could start my first mesh convergence. 

### Mesh 1.2/Simulation 1.2

<img width="134" height="332" alt="image" src="https://github.com/user-attachments/assets/be462a8b-2468-4199-ad01-71f262bb5c24" />

For my second mesh, I changed my maximum element size from 0.128937in to .1in. This is approximately a %22 reduction in size to let me see a more defined result. 

<img width="543" height="361" alt="image" src="https://github.com/user-attachments/assets/208bafbd-ee58-45a6-ba5e-a97c97370835" />

<img width="551" height="359" alt="image" src="https://github.com/user-attachments/assets/b3e84ed7-9097-4764-8e41-9955a5189034" />

<img width="530" height="365" alt="image" src="https://github.com/user-attachments/assets/be71f21e-8b64-4090-a7cc-8b11c4bea737" />

<img width="275" height="261" alt="image" src="https://github.com/user-attachments/assets/aa87aa58-6b59-4ad5-be12-4786f96d3f5b" />

<img width="350" height="503" alt="image" src="https://github.com/user-attachments/assets/8b9735a9-e8b6-43ff-86c2-b1c355604b6a" />

After just the second mesh, my design hit the 7% mesh convergence requirement, but the stress and displacement values are way over, so I will have to fix this in my second design. 

### Design 1 Data Results

<img width="478" height="133" alt="image" src="https://github.com/user-attachments/assets/389fbba8-686e-4c26-a104-ca8e9c8519e5" />

After just changing the mesh once from 8548 elements to 15560 elements, I was able to get under the 7% mesh convergence requirement. But I learned that my design is not physically possible and has extremely high stress values that I need to fix. I do now know where the exact max stresses are and what areas I need to focus on in my second design. 

## Design 2

<img width="755" height="329" alt="image" src="https://github.com/user-attachments/assets/7e7b03f2-4dfb-488d-a3b2-980273d07b7a" />

<img width="717" height="380" alt="image" src="https://github.com/user-attachments/assets/594be5df-7c56-46dd-872d-2df3f87acd0a" />

<img width="326" height="343" alt="image" src="https://github.com/user-attachments/assets/23610152-f38f-402a-bcf0-d1786eaead35" />

For my second design, I need to focus on the fact that most of the stress is in member B. So my thoughts at first were to, one, make it thicker, and two, add fillets at the meeting points of B and A, as well as B to the top. The thickness of member B was originally .06in so I just doubled it to .12in not to make it too much of a change, but enough to make a difference. Next, I added the fillets where member B connects and set it to a radius of .1in.

### Mesh 2.1/simulation 2.1

<img width="709" height="366" alt="image" src="https://github.com/user-attachments/assets/90f00ce7-7354-4cee-9423-0aedaa8ecaca" />

<img width="312" height="282" alt="image" src="https://github.com/user-attachments/assets/a5ebf0a6-dc2d-442a-9450-3e94b6221f21" />

For my first mesh of the second design, I set the element size to .1in which is where I ended on the previous design.

<img width="527" height="341" alt="image" src="https://github.com/user-attachments/assets/7bc26a9e-af43-4f03-bb01-f28ff9659924" />

<img width="508" height="338" alt="image" src="https://github.com/user-attachments/assets/7c4cccb4-7680-42a6-8267-85a25afa8fd3" />

<img width="533" height="320" alt="image" src="https://github.com/user-attachments/assets/ac9f0da4-4fa4-4508-baf9-7ddbca505a31" />

This design performs much better in all areas, lowering my stress and displacement by almost 75%, but it still isn't enough for my yield strength. 


### Mesh 2.2/Simulation 2.2

<img width="499" height="302" alt="image" src="https://github.com/user-attachments/assets/16aa33e4-3a60-458c-af40-74225e6143f6" />

<img width="517" height="329" alt="image" src="https://github.com/user-attachments/assets/34241033-e152-404d-bc3d-1f9d20c5dc81" />

<img width="518" height="336" alt="image" src="https://github.com/user-attachments/assets/60682810-2c7b-44eb-ac80-2c5869b293d2" />

For the second mesh, I changed the element size to .75in. This met the 7% mesh convergence requirement, allowing me to not have to do a third mesh, and I can start on my third design. 

### Design 2 Data Results

<img width="479" height="131" alt="image" src="https://github.com/user-attachments/assets/5c1eb189-0474-440e-973c-699a9f4dddfa" />

In my second design, I massively cut the maximum stress and maximum displacement down, but I did gain.01lbs of mass, and that doesn't matter with it being so minuscule. From this design changed i learned how such small changed can make a huge difference when design for stress and loading forces. A simple fillet or making a part ever so slightly larger can really help the design. However, in the future, I have to remember that you can't always just make things bigger to account for forces. 

## Design 3

<img width="241" height="335" alt="image" src="https://github.com/user-attachments/assets/a7914f8b-0619-4860-a93b-7d482c6c05b4" />

<img width="311" height="282" alt="image" src="https://github.com/user-attachments/assets/bd3a171e-8fc7-425b-9702-31bf398dd871" />

<img width="619" height="296" alt="image" src="https://github.com/user-attachments/assets/675abe1b-2fcf-49cf-a7f5-0f5142744d18" />

<img width="800" height="372" alt="image" src="https://github.com/user-attachments/assets/dad825d9-8e52-4036-bb26-2833cb75b22a" />

<img width="674" height="374" alt="image" src="https://github.com/user-attachments/assets/4970d1e8-8fee-43a5-b13a-6ea636c3fbb7" />

<img width="325" height="344" alt="image" src="https://github.com/user-attachments/assets/67b7eb4b-2aaa-4c4a-99ca-cce3ce61ac92" />

For my third design, I wanted to add a triangular support on the front of member B to member A (the cylinder)to transfer some of the load directly. Knowing triangles are the strongest and most supportive shape, I chose it to help brace my design to stop some of the deflection. To do this, I had to first remove the fillet I previously added for now so I could add the support in its place. I then added a reference geometry and selected the two outer top walls as references, and selected the mid plane. This will give me a plane in the middle of the design to sketch on so I can extrude the triangle support much more easily. I did have to stretch the plane a little to make it reach where I needed to sketch. Next, I sketched and extruded a triangle connecting the two members and set it to a thickness of .1in. I mirrored the extrusion across the midplane I made to make it symmetrical. Lastly, I added my previous fillets and added some new ones. 

### Mesh 3.1/Simulation 3.1

<img width="829" height="370" alt="image" src="https://github.com/user-attachments/assets/51863abe-f4d9-4cc7-ae96-2febdc57d7e4" />

For this mesh, I set the maximum element size to .10in

<img width="605" height="335" alt="image" src="https://github.com/user-attachments/assets/c4c77a99-ebaa-41de-8eac-faf7f14c8765" />

<img width="557" height="342" alt="image" src="https://github.com/user-attachments/assets/60fdd1bc-cafd-451e-b9db-38c6a4212352" />

<img width="577" height="359" alt="image" src="https://github.com/user-attachments/assets/e5b2ea7f-2726-4ace-ae0b-5ba2589576cc" />


### Mesh 3.2/Simulation 3.2

<img width="131" height="322" alt="image" src="https://github.com/user-attachments/assets/d9120b14-06ef-400c-9754-14a9cd8264cd" />

<img width="497" height="343" alt="image" src="https://github.com/user-attachments/assets/4c728003-d24c-4036-ad29-10707058e9b9" />

<img width="512" height="354" alt="image" src="https://github.com/user-attachments/assets/dcb45e3e-c332-455f-ab1d-767cfa65b236" />

<img width="481" height="343" alt="image" src="https://github.com/user-attachments/assets/2a94010c-f5eb-4286-aa83-4c80c46cf6c4" />

### Mesh 3.3/Simulation3.3

<img width="128" height="278" alt="image" src="https://github.com/user-attachments/assets/8959bd71-b20d-41a8-8889-304eeac9753e" />

<img width="515" height="347" alt="image" src="https://github.com/user-attachments/assets/f1cca2a4-71cd-4e04-bf47-073d72297706" />

<img width="531" height="350" alt="image" src="https://github.com/user-attachments/assets/8dd87f16-22ef-437a-949e-162e83593d70" />

<img width="525" height="352" alt="image" src="https://github.com/user-attachments/assets/2e808206-f88e-4f08-8fb0-5d8f96aa02fc" />

### Design 3 Data Results

<img width="479" height="138" alt="image" src="https://github.com/user-attachments/assets/b3339cad-5f85-40ef-9b00-48ace562b8da" />

After three attempts, my mesh did not converge, so, going off the rules of the assignment, I will be using the finest mesh results. The triangle support did help some, but not as much as I predicted. I think maybe adding another support to the top of member B could have been enough to lower the displacement. 

<img width="475" height="178" alt="image" src="https://github.com/user-attachments/assets/64707bd5-c100-4224-8f3c-35b8a906fbf9" />

## Lessons Learned

The biggest thing I learned from this assignment is what it's like to design for a purpose and not just blindly model an object and hope it works because you like the way it looks. In the real world, objects go through forces, stresses, and other external factors that can change our artifact or even cause failure. So when designing something that you know is going to go through something like this, it's a much different process than designing something with a snap fit or linkage. Another lesson I learned is engineering is never a one-and-done solution. In the end, my design did not come out to be able to work with the forces applied to it if this were the real world. There was more stress than my material had yield strength, and this would've cause major failure if a real object. This was after doing three different iterations to my design to make it stronger and more supported. This shows that engineering a real design for a job may take multiple prototypes and many different iterations to your initial design before you have a producible product. 

I spent a total of around 13 hours on this assignment. 
## CAD Files
[A6 Bracket design 3.zip](https://github.com/user-attachments/files/34209243/A6.Bracket.design.3.zip)




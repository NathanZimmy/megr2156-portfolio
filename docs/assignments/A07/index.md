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

### Mesh 1

<img width="755" height="372" alt="image" src="https://github.com/user-attachments/assets/91518f96-44cd-427d-a4fc-c8fe992f1b1f" />

I added my first mesh and left all the settings completely as they were automatically set. This was to see what would happen and where my design currently sits. 

<img width="312" height="148" alt="image" src="https://github.com/user-attachments/assets/1036c76f-45b0-4d03-9e0a-c3df4c5a42ec" />

After creating my first mesh, I hit run to test the first study. However, I had this pop-up and had no idea what it meant or what to do, so I screenshot it and asked AI. AI told me that I didn't do anything inherently wrong, but that my design may be going through a very large displacement, with my force being 1200lbf. It notified me that I should hit no so I can analyze my initial geometry because hitting yes will automatically cause changes. 

### First simulation

<img width="568" height="355" alt="image" src="https://github.com/user-attachments/assets/d105dcbf-4094-4c76-ae54-2355f29a3562" />

<img width="501" height="344" alt="image" src="https://github.com/user-attachments/assets/d0c47629-7808-474e-9c22-2e0a66ce1fed" />

<img width="494" height="325" alt="image" src="https://github.com/user-attachments/assets/b943f40c-fa8a-4d35-9253-c17b465425ae" />

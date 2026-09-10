# A3 – [Parametric and FEA]

## Objective
-Use axial deflection modeling to design its dimensions

-Use parametric design to determine a bars length

-Introduce you to FEA (Finite Element Analysis)

-Introduce you to linking dimensions to appropriate parameters in CAD.

-Compare and contrast the different analysis

You are to design a bar which has a circular cross section where the values of the criteria given for the material, maximum deflection, and load. Determine the bar’s minimum geometry (ie.. length, diameter, and weight) through parametric design while under direct tension. Then verify the geometry through finite element analysis.

The bar must be made out of aluminium with a range of Young’s Modulus from (8.5 - 11.5) x 106 psi. The design must have a direct load between 300 lbf < F < 500 lbf, and the max axial deflection of the bar is .009 inches.
## Calculations
Before I am able to start modeling on this project, I must first calculate the beam I am working with. To start, I need to choose a diameter and solve for the area. I chose 0.5in and used the area of a circle to find the area is .19635in^2. I then needed to choose a force for this beam. We are allowed 300lbf to 500lbf, so I chose the maximum force allowed at 500 lbf. I did this because I want to solve for the strongest bar I can. Lastly, I needed to choose a material from SolidWorks to get Young's Modulus. I went online to search for which aluminum alloys are the strongest in terms of resistance to permanent deformation and found that 7075-T6 works very well for this, and SolidWorks also has it in its material list. So, I chose this material, and it has an elastic modulus of 72000MPa. I can convert this to PSI and get 10.44x10^6PSI and this fits in the required range. Now that I have all the values, I can solve for the length using the direct tension elongation equation. If I solve for L and then put in my values, I get that my bar needs to be 36.90in.

<img width="418" height="290" alt="image" src="https://github.com/user-attachments/assets/6d3e3b68-6d07-47db-a40b-08fe08536e8e" />

## SolidWorks Design

<img width="590" height="253" alt="image" src="https://github.com/user-attachments/assets/9a28e1e7-e983-4870-b1af-ab6f881cc99e" />

My first step to modeling was going in and setting all my global variables. This is to check my hand calculations and make sure they are correct, but this is also to make modeling easier, so I don't have to type in all the number i can just click my global variable, and it automatically inputs the correct value.

<img width="414" height="200" alt="image" src="https://github.com/user-attachments/assets/3fa254a7-cecb-41f3-8316-5fe50ec2ff6e" />

<img width="779" height="485" alt="image" src="https://github.com/user-attachments/assets/0326681f-2842-4d85-805c-1d05f82b65ae" />

Now that I have my equations set, I am able to start CAD modeling it. I started with a sketch on the top plane and drew a circle and set the diameter to my global variable "d". I also went ahead and changed the material to 7075-T6(SN).

<img width="697" height="379" alt="image" src="https://github.com/user-attachments/assets/3714ce20-cd51-43bb-8942-1ce5cc23acc1" />

Next, I extruded the sketch and set the length to the global variable "L". Now my model is complete.

## Finite Element Analysis (FEA)

<img width="684" height="74" alt="image" src="https://github.com/user-attachments/assets/64162d65-5bdc-48da-91f7-883c42d00a35" />

<img width="698" height="317" alt="image" src="https://github.com/user-attachments/assets/4affcb40-5997-4cd7-8bb4-33525a3853bf" />

<img width="677" height="371" alt="image" src="https://github.com/user-attachments/assets/0fa58b8d-c639-4d6f-b409-8be3a04d6c2f" />

With my model complete, I am able to start doing FEA. To start this in SolidWorks, I first must hit simulations, then New Study. After starting the study, I apply a fixed geometry to the end of my beam under the Feature tab.

<img width="819" height="374" alt="image" src="https://github.com/user-attachments/assets/000df154-bafd-4884-8391-a626057d268c" />

Next, I applied my 500lbf force to the other side of the beam. While doing this, I had to change my units to English so it would be in lbf, as well as flip the direction of the force. I also had to manually type in 500lbf, as you cannot use global variables here.

<img width="776" height="410" alt="image" src="https://github.com/user-attachments/assets/96fca535-4f2d-4837-9e3a-4f17caca683d" />

<img width="959" height="426" alt="image" src="https://github.com/user-attachments/assets/82b820b5-2102-4864-b5cc-724fe2c2e4e8" />

<img width="959" height="371" alt="image" src="https://github.com/user-attachments/assets/91282258-98c5-428d-a952-ff793f3fdf87" />

<img width="955" height="373" alt="image" src="https://github.com/user-attachments/assets/c76d03d0-3175-473c-be0c-c6be1c16ebca" />



Now I ran the study to get my deformation results. The first graph is displacement, the second is strain, and the third is stress. I had to go in and change all the units for each graph.

## reflection

The axial deflection I used in my hand calculations was 0.009in, and the value given by my FEA was .0093. I calculated the percent difference to be .03% which is most likely due to the fact that I rounded the length to an even number. This means the beam I modeled worked almost exactly as I calculated. I would be more likely to trust the SolidWorks design because it does not round or have human error when calculating results.

I learned a lot of things on how to use SolidWorks more efficiently, as well as being able to simulate forces and run tests. Setting equations and using global variables makes things much faster when modeling, as well as lowering the chance of error by typing in the wrong value. I also learned you can implement a fixed geometry and forces on your models in SolidWorks to check your math and see what is actually happening to the things you design. This will make designing and modeling much better for future projects and designs.

I spent a total of two and a half hours on this project.

## Cad Files
[lecture A3 beam.zip](https://github.com/user-attachments/files/32057937/lecture.A3.beam.zip)


## sources
https://rochemetal.com/tools/aluminum-alloy-selector/


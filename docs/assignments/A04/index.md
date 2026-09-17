# A4 – [Motor Mount]

## Objective
The task we were given is to design a motor mount for a (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) that will attach to a rigid wall labeled A. We are to look at the motor mount as two different features and act as if both features are cantilever beams. For each feature, we first must design for yield strength and second design for a maximum deflection of .30 mm at the free end. When solving for these, we must also draw free-body diagrams of the forces and our design concepts. Lastly, we are to research the design of different motor mounts and place the links in an appendix on your page.

<img width="100" height="84" alt="image" src="https://github.com/user-attachments/assets/de8e6c9c-15d7-4a03-8b1a-e32aef8888d8" />

<img width="365" height="339" alt="image" src="https://github.com/user-attachments/assets/60de88a3-fff4-4b05-9c55-f2e2b9873d3b" />
<img width="215" height="141" alt="image" src="https://github.com/user-attachments/assets/8c9221f2-15f2-4881-bd81-9c39bc2f91e6" />

Image of motor and physical dimensions

### Criteria
-Can use PETG, PLA, or ABS

-Safety factor of 3

-Maximum deflection of .30mm

-P=300N

-Design as cantilever beams

Assume the safety factor accounts for the holes for the motor shaft and the screws in your calculation

-Weight is negligible

### Material Research
<ins>ABS</ins>

Yield Strength = 29.6 - 48 MPa

Young's Modulus = 1.79 - 3.2 GPa

<ins>PLA</ins>

Yield strength = 8.00 - 103 MPa

Yield strength = 46.0 - 49.0 MPa at temperatures of 30 to 110° Celsius
Average value: 45.2 MPa

Young's Modulus = 0.00232 - 13.8 GPa
Average value: 2.35 GPa

<ins>PETG</ins>

Yield strength = 28.3 - 101 MPa

Young's Modulus = 1.10 - 20.3 GPa

## Feature 1
Feature 1 is the piece that the motor is connected to. I decided to go with PLA for my design because I am familiar with how it works and I've printed with it before. After using the given websites, I found that it has a yield strength of 8.00 - 103 MPa and a Modulus of elasticity of 0.00232 - 13.8 GPa. It also listed the average values for both of those measurements at 45.2MPa and 2.35GPa. I decided to use the average values since that's what would be most common. Next, I had to choose a length and width for my design. I did this by looking at the given motor measurements. The motor body is about 27.7 mm diameter × 38 mm, the gearbox is 28 mm diameter × 36.6 mm, and the shaft is 6 mm diameter × 18 mm long. So I chose to make my length 50mm and my width 40mm to give myself some working room and have it be an even number. 

<img width="302" height="241" alt="image" src="https://github.com/user-attachments/assets/b5a1dc68-7fa6-48ac-ade5-7a1c0ca4dbe0" />

This was my first attempt at designing, but I restarted after realizing that I had swapped the features and was solving feature 1 as feature 2.

<img width="263" height="315" alt="image" src="https://github.com/user-attachments/assets/10231f64-9420-4398-9f42-88f58aa2a959" />

To start solving, I first drew my free-body diagram and labeled my forces. We are given that M = PL, so with that I can label my moment and know that P goes at the very end of the feature because M = PL; we use the same length of distance that I chose earlier. I then solved my static equations and got M=15000N*mm. Then I solved for maximum strength using the bending equation. I calculated that the height needs to be at least 12.22mm. Lastly, I calculated for maximum deflection using the given equation and found the height needs to be a minimum of 19.98mm. Since the deflection value is larger, that's the height I will go with. To make it easier, I will be rounding up to 20.0mm to be safer and make modeling and designing easier.

## Feature 2
<img width="302" height="326" alt="image" src="https://github.com/user-attachments/assets/f9d73e66-b549-47fb-8a35-22b41f58444d" />

Feature 2 was much easier to solve for since we didn't have to worry about the force, and I already figured out the equations to use, so I carried them over. I started by drawing my free-body diagram and solving for M, which is the same as Feature 1. I then solved for max strength and max deflection, and the strength was the same as feature one because I used the same length. The deflection, however, was different, and I calculated it to be 17.22mm. I'm going to round that to 18mm to make it even and easier to model. 

## Isometric View

## CAD Model Parametric
<img width="476" height="414" alt="image" src="https://github.com/user-attachments/assets/cd42e306-5652-4c34-9109-1d7850ef689b" />

<img width="200" height="262" alt="image" src="https://github.com/user-attachments/assets/05ada8c2-80fe-421c-a298-9e43d4c9f7fc" />

<img width="257" height="235" alt="image" src="https://github.com/user-attachments/assets/1a621c86-c103-4d52-acac-99291c28369e" />

To start, I went in and changed the units to mm and then started a sketch on the top plan and drew a simple rectangle. I then extruded that rectangle by the thickness of feature one I solved for earlier, of 20mm.

<img width="700" height="334" alt="image" src="https://github.com/user-attachments/assets/ae1c3873-0614-442e-92d0-e96c0564469a" />

Next, I added feature two by starting a sketch on the top of the previous extrude. I set the thickness to 18 and extruded it to a length of 40.

<img width="581" height="201" alt="image" src="https://github.com/user-attachments/assets/5aeaa0ca-cfd5-41d4-9d56-efe875570ded" />

<img width="296" height="301" alt="image" src="https://github.com/user-attachments/assets/239f562b-c329-42f8-9e8e-07582ed052fe" />

Now I had to add the bolt holes and space for the motor to fit. I went based on the appendix image given for the measurements and depths to make the cuts. First, I started a sketch on feature 1 and made two center lines that intersected so I knew where the center of the shape is. Next, I drew a circle on the center intersection point with a diameter of 18mm. I then extrude cut that circle with a depth of 2mm

<img width="350" height="271" alt="image" src="https://github.com/user-attachments/assets/a64660d6-76a7-4f65-a0af-34d82f86b082" />

<img width="404" height="329" alt="image" src="https://github.com/user-attachments/assets/67413b85-dbcd-4c01-a9db-468960e0ff6f" />

<img width="798" height="361" alt="image" src="https://github.com/user-attachments/assets/87986309-64a1-4a95-9930-6c2cb82278aa" />



Next, I added the center hole where the D-cut part of the shaft will go. I did this by doing another extrude cut in the center of the previous hole and selecting to through all. I also added the tolerance of -.03mm. Lastly, I created the bolt holes. There are four of these at equal distances from each other, with a diameter of 22 mm, so I created one hole, then patterned the other three off that one. I made an extrude cut and sketched a circle of 3.40mm and set it to a distance of 11mm from the center of the shaft hole. To make the other three, I selected Circular Pattern and set the instances to four at a 360° angle and used and clicked the center shaft hole to be my axis of rotation. 

<img width="260" height="317" alt="image" src="https://github.com/user-attachments/assets/c116edc8-0f84-4c5d-90b5-dcf072c35a89" />

This is the final model of my motor mount.
### CAD Files

[Lecture A4.zip](https://github.com/user-attachments/files/32332752/Lecture.A4.zip)

## Lessons learned
One big take away I got from this assignment was that what it's like to design with a purpose from scratch to solve a problem. We are given a motor and need to make a bracket that will hold or mount this motor to something. Ive seen motor mounts before and know what they are and it looks so simple at fire. But I never realized how much goes into designing something from scratch with no measurements or given requirements. When you look at simple objects such as a motor mount you don't think much of it but there really is so much more to creating something with a purpose starting from just an idea. I also learned about cantilever beams and what they are. I was introduced to this term during this project and leaned that a cantilever beam is just a beam that is fixed at one (rigid) end and free to move or bend at the other. 

In total this assignment took me 7 hours to complete.

## Sources
https://www.matweb.com/search/DataSheet.aspx?MatGUID=ab96a4c0655c4018a8785ac4031b9278&ckck=1
https://www.specialchem.com/plastics/guide/acrylonitrile-butadiene-styrene-abs-plastic
https://www.omc-stepperonline.com/brushed-24v-dc-gear-motor-3-6kg-cm-46rpm-w-99-5-1-planetary-gearbox-pa28-28245800-g100


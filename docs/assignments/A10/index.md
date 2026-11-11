# A10 – Lead Screw Design

## Minimum Diameter Logan Sulyi

The knowns include the total force, 2 kN, which is 1 kN per screw; a safety factor of 4; and the material is 1045 cold-drawn steel, so the yield strength is 530 MPa. To solve for the minimum diameter, I used the equations for axial and allowable stress, and found the minimum diameter to be 3.10mm (0.122 in).

<img width="3050" height="3577" alt="IMG_3677" src="https://github.com/user-attachments/assets/4c77c622-273b-4b79-b82c-4cca8a43321b" />


## Rotational Speed Logan Sulyi

The knowns for the rotational speed are the crosshead speed, Vmin = 1 mm/min, and Vmax = 50 mm/min. The Lead equals 0.25 in, which equates to 6.35 mm/rev for a 2-start screw. The pitch is 0.125 in. The unknowns are the maximum and minimum rotational speeds. Using the equation N = V / L, I found the minimum rotational speed to be 0.157 rpm, and the maximum rotational speed to be 7.87 rpm.

<img width="3416" height="3831" alt="IMG_3678" src="https://github.com/user-attachments/assets/74dc2f83-018a-4d5b-82d4-ab88924713f7" />


## Max Torque Logan Sulyi

The knowns for the maximum torque are the load per screw, 1 kN, which equates to 224.8 lbf. The lead equals 0.25 in, and the diameter equals 0.5 in. Using the efficiency provided, I used the formula included below and calculated the maximum torque to be 17.2 in*lbf.

<img width="3464" height="3423" alt="AdobeExpressPhotos_011b1fb3e1f64902842edfabed110a32_CopyEdited" src="https://github.com/user-attachments/assets/4b87b027-e977-4d24-bc45-d4dd34d93942" />


## Lead Screw Selection Logan Sulyi

After looking at my numbers, I chose a 1018 Carbon Steel Precision Acme Lead Screw for this project. It is a Class 2C thread fit, and it is 3 ft long.
<img width="1182" height="690" alt="image" src="https://github.com/user-attachments/assets/afe9ff48-b64e-4645-a825-f9ff8b9b2fba" />


## Nut and Flange Logan Sulyi

Knowns for the nut and flange include the load per screw (224.8 lbf), nut diameter (0.5 in), and pitch (0.125 in). The height is half the pitch: 0.0625 in. The safety factor is 4, and after choosing the nut, the material is 673 bronze, meaning the yield strength is 30 ksi.

<img width="3424" height="4687" alt="IMG_3680" src="https://github.com/user-attachments/assets/51b31db3-cefc-4a44-b0cb-5c7659fdb1cd" />


## Crossshead Strength & Deflection Logan Sulyi

The knowns for the crosshead include the load (2 kN, which equals 449.6 lbf),  the length between screws (8 in), and the width (3 in). The safety factor is 4, and after picking the material to be 6061-T6 aluminum, I found the yield strength to be 35 ksi. Using the maximum bending moment, area moment of inertia, and the minimum beam height, I found the height to be 0.453 in (11.5mm).

For the deflection, the knowns are the same, except we also include the maximum deflection, which is 0.1 mm, which equates to 0.003937 in, and the young modulus, which is 10 x 10⁶ psi. Using the maximum deflection and area moment of inertia equations, I calculated the deflection to be 0.0206 in.

<img width="3696" height="4391" alt="IMG_3681" src="https://github.com/user-attachments/assets/b6ed64b0-55c0-47bf-a564-871db460c608" />



## Crosshead Size and Material Logan Sulyi

The knowns for the size and material include the load (2 kN, which equals 449.6 lbf),  the length between screws (8 in), and the width (3 in). The safety factor is 4, the maximum deflection, which is 0.1 mm, which equates to 0.003937 in, and the young modulus, which is 10 x 10⁶ psi. Using the  maximum deflection and area moment of inertia equations, I calculated the thickness to be 1.249 in.


<img width="3117" height="4003" alt="IMG_3682 (1)" src="https://github.com/user-attachments/assets/03b2d060-9d71-4e94-97f3-60ab4904cec8" />



## Multiview Sketch of Crosshead Logan Sulyi

Below is a multiview sketch of the crosshead. It is an 11 in long by 3 in wide by 1.5 in thick rectangle made out of 6061-T6 Aluminum. The two screw holes are 0.5625 inches in diameter, 8 inches apart. The smaller screw holes are 0.266 inches in diameter, 0.453 inches away from the larger screw hole.

<img width="3633" height="3773" alt="IMG_3685 (1)" src="https://github.com/user-attachments/assets/3aab28b0-98e2-42b2-ae9c-0902ce34517b" />



## Bill of Materials Logan Sulyi
Listed below is our Bill of Materials, which includes the lead screw, the threaded nut, the flange, head screws, and an aluminum bar for the crosshead.
<img width="425" height="526" alt="image" src="https://github.com/user-attachments/assets/3c7f5743-0c83-4ce6-8b26-c36932a66089" />



## Parametric Modeling - Austin Williams

Crosshead Design:

Based on the calculations from my group members, I started the crossmember design as a rectangle 11" X 3"

<img width="556" height="212" alt="image" src="https://github.com/user-attachments/assets/4c4d0883-b804-4ee2-85d1-ae7ff54d9c6b" />

Next, I needed to make the holes for the leadscrews; I was able to make the holes using a linear sketch pattern that created perfect geometry across the crosshead. The size of the holes was also based on the previous calculations.

<img width="753" height="318" alt="image" src="https://github.com/user-attachments/assets/2add0f07-7ea3-444f-b99e-031d1cadb307" />

Once that was done, I extruded the holes through so that the screws could go through

<img width="643" height="269" alt="image" src="https://github.com/user-attachments/assets/e2c2a8f9-d2c7-4314-a342-2b9cd7b17da3" />

Here are the parametric equations used to make the crosshead:

<img width="593" height="244" alt="image" src="https://github.com/user-attachments/assets/bb8fa88d-1b49-4af2-951d-62e99177ac4e" />

After that, I downloaded the necessary parts to complete the assembly

Here is the channel that I used for the frame of the machine; This is a rectangular-style channel.

<img width="1120" height="641" alt="image" src="https://github.com/user-attachments/assets/7bf92fdc-e46b-44c1-9164-b11323287806" />

<img width="332" height="188" alt="image" src="https://github.com/user-attachments/assets/65374971-52bb-4771-a457-34d8606b2080" />

The first major issue that I ran into was that the CAD files were imported from another software, so I could not change the dimensions of the channel as needed to create the correct sizes for our assembly. I solved this by creating a new plane along the axis of the channel, making a sketch around the channel, and extruding the extra length out of the equation.

<img width="821" height="549" alt="image" src="https://github.com/user-attachments/assets/74f743d7-1a25-4a2b-b1e9-3b216cfb6ade" />

I had to repeat that step twice to get the sides and the top/bottom of the frame.

<img width="877" height="568" alt="image" src="https://github.com/user-attachments/assets/1677c3c2-e42b-4da2-a0db-6a6900d9ba3c" />

The assembly itself was not terrible, but it was very time-consuming because mates don't always like to work with each other in SolidWorks

Below are a few pictures of the full assembly from different angles;

<img width="326" height="602" alt="image" src="https://github.com/user-attachments/assets/2fc30db6-071e-4449-b41b-6a21372121cb" />

****Note**** - The assembly in SolidWorks did not want to stay together properly, so I had to use an auto 3D feature in SolidWorks to visually get rid of the threads for the assembly. I was going to try it without that; however, the software automatically did this on its own. The parts would physically fit in a real-life scenario, but the threads on the crosshead did not match 100% to the leadscrews, and I have no way of making them the exact same myself.

<img width="462" height="432" alt="image" src="https://github.com/user-attachments/assets/e0d53920-7875-4f01-add6-53e0d8113d95" />

This final picture shows the flange, screws, and the nut that were required for our tensile tester.

<img width="398" height="299" alt="image" src="https://github.com/user-attachments/assets/87468528-4be0-4b69-b3c1-fd9620c18dab" />

[CAD Files Here](https://github.com/AustinW-UNCC/megr2157-portfolio/blob/main/Final%20Assembly%20A10.SLDASM)

## Decide
_Reference your concept selection (Pugh matrix) here. How does this design follow from that decision?_

## FEA on Crosshead (Nathaneal Zimmerman)

For this section, we are to run FEA on our crosshead to evaluate stiffness and strength under a 2KN axial load. We are to use our results to optimize the geometry by reducing weight and stress concentrations using fillets, changing thickness, or cutting extra material out. 

<img width="600" height="475" alt="image" src="https://github.com/user-attachments/assets/27555967-2c67-428a-8bd2-c0e96737886c" />

We are using 6061-T6-SS which is an aluminum alloy with a yield strength of 275Mpa and a modulus of elasticity of 69000Mpa so we will have to keep the design within these material properties. 

<img width="920" height="367" alt="image" src="https://github.com/user-attachments/assets/e6809634-54ee-4ef9-a64a-fd964ac8ada2" />

<img width="800" height="352" alt="image" src="https://github.com/user-attachments/assets/21af7a46-a1cb-44a4-86c0-e802ead049a5" />

I started by adding fixed geometries to all the screw holes where the crosshead will be mounted, assuming the screws are perfectly rigid in this assignment. This will hold those ends in place. Then I added a force on the center hole of 2KN or 2000N and clicked Selected Direction. This is because if I simply click the hole, the force will be applied in all directions around the circumference of the cylindrical hole. So, by using Selected Direction, I can click the top surface and have the force be pointed downwards through the hole, which is where the part that is being tested will be applying the force onto the crosshead. 

### Test 0.1

<img width="803" height="377" alt="image" src="https://github.com/user-attachments/assets/49acd147-e292-47f2-b2fa-813a2c5cb2db" />

<img width="755" height="367" alt="image" src="https://github.com/user-attachments/assets/f2a7f7f9-c8e9-4d05-83e2-ad528ca56d5d" />

<img width="755" height="356" alt="image" src="https://github.com/user-attachments/assets/c0887c18-d891-4986-839b-cd1f4b4238f3" />

<img width="277" height="243" alt="image" src="https://github.com/user-attachments/assets/d21b2528-6e01-49fe-822f-83fad6af97b3" />

After running the first test we can see that we have no strain and our deflection is very little having a max of .005mm which is pretty much negligible. However, our max stress is 10257662N/M^2 but it is a huge stress concentration at the innermost screw holes, with the rest of our model having much less stress. But this value is okay because our material yield strength is 275 MPa or 275000000pa so we are way under this value. 

For this first test, I did not edit the mesh and left it as is.

### Test 0.2

<img width="818" height="370" alt="image" src="https://github.com/user-attachments/assets/67c8d6c5-1bab-46aa-a350-a89ae0754a46" />

<img width="569" height="203" alt="image" src="https://github.com/user-attachments/assets/def012ab-b614-4a99-82c7-aa567b825514" />

For this second test, all I did was change the max element size of the mesh to .6in making it finer to see how the values would change before I edit the model. 

<img width="767" height="353" alt="image" src="https://github.com/user-attachments/assets/3338d9b0-8574-4271-837b-2b88edfd00b2" />

<img width="730" height="365" alt="image" src="https://github.com/user-attachments/assets/25a79eb7-9dca-4e84-9080-279195d2e6c0" />

<img width="739" height="362" alt="image" src="https://github.com/user-attachments/assets/82d4a22f-a150-4e05-bebc-18eb0d6128b5" />

After changing the mech size to a smaller element size, the stress concentration went up, but the other values stayed the same. So we know the screw holes are where the problems are, and we also know the average stress throughout the model is very low compared to the max, which will allow us to cut out some of the material. 

### Optimization 1

<img width="521" height="289" alt="image" src="https://github.com/user-attachments/assets/c6e63ccb-24cb-4d3a-8ebe-d27719d0fc73" />

To try to reduce the stress on the screw hole, I added a .1in fillet on all the holes. 

#### Test 1.1

<img width="770" height="358" alt="image" src="https://github.com/user-attachments/assets/be5f889e-e376-4cc5-b3f8-c3d6166456b0" />

After adding the fillets and running another test, we found that this actually raised our max stress by over 1 million pascals. While this isn't what we were going for, it's okay because this is still way under our maximum yield strength. 

### Optimization 2

<img width="580" height="332" alt="image" src="https://github.com/user-attachments/assets/c0335c8c-f787-44a6-8212-9fa193a5ddc7" />

<img width="454" height="254" alt="image" src="https://github.com/user-attachments/assets/577954f7-91ec-474f-a948-aec8c34c5182" />

<img width="673" height="317" alt="image" src="https://github.com/user-attachments/assets/a9e44183-41cd-458d-adc9-f8236ab6068c" />

After seeing that most of the material in our crosshead undergoes almost no stress or deflection, we wanted to remove some of the material to save on weight. So, I cut out sections in the center of the body and used the mirror feature to mirror one sketch into four across both centerlines. 

#### Test 2.1

<img width="581" height="290" alt="image" src="https://github.com/user-attachments/assets/98f89727-5dec-44a4-8cdc-9bc2e4d76586" />

<img width="575" height="289" alt="image" src="https://github.com/user-attachments/assets/94a147e9-1781-4889-8664-fbd44b5a82f1" />

<img width="649" height="333" alt="image" src="https://github.com/user-attachments/assets/e41c247e-f64a-46e4-bafc-820d21e0aaf7" />

After running another test, the cutouts actually raised our stress and deflection, but not enough to hurt our model.

## Engineering Drawing

<img width="418" height="323" alt="image" src="https://github.com/user-attachments/assets/9c2af9dd-95a3-4ff7-b1e6-e3fc1445713b" />

Here is the drawing of the optimized crosshead model.

## Lessons Learned (Nathaneal Zimmerman)

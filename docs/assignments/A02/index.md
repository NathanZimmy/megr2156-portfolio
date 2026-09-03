# A2 – Truss Stress Analysis

## Objective
The objective for this assignment is to design a basic lightweight planar truss using A500 steel or an alternative material, while following the specified measurements listed below. We are also to show all calculations for the required cross-sectional area of truss elements with a safety factor, create free-body diagrams for all joints and pins, show calculations for determining the pin sizes based on shear forces with a safety factor, solve all equations symbolically and numerically for both truss and pin design, and estimate the total weight of the truss and pins. Lastly, we are to create a CAD model with accurate dimensions and connections of the design we chose and then compare the CAD weight predictions to the hand calculations. Lastly, we are to document key engineering lessons learned from the process.

<img width="320" height="194" alt="image" src="https://github.com/user-attachments/assets/78e9c3e8-249e-45f5-959b-db6fa12fc66d" />

## Given Parameters
Choose a P between 20 - 30 kN. a = .4 m, b = .3 m. Point A is a pin, and point B is a roller.

## Truss Sketches and Geometry Calculations

<img width="259" height="320" alt="image" src="https://github.com/user-attachments/assets/91499b10-7b44-407d-83a7-ed4d3865abc3" />

<img width="227" height="47" alt="image" src="https://github.com/user-attachments/assets/78aed67a-c57a-498c-9f75-dd122c2eae8f" />

#### Minimum Cross-Sectional Area of Truss 

<img width="335" height="250" alt="image" src="https://github.com/user-attachments/assets/7ee749dc-cd16-4e6f-ba4b-1a57c12c7b7f" />

Determining the minimum cross-sectional area was far less time-consuming and a lot more straightforward during calculation than designing the truss itself. First, I collected my known values and my unknown values so I would know what I am trying to solve for and what I have to use when solving. I know the equation for normal stress is Sigma= F/A, where Sigma is stress, F is force, and A is cross-sectional area. This equation can be derived into A=F/sigma, which can further be interpreted as Amin =F/ sigma allowed, which in words means the minimum cross-sectional area equals the largest force calculated on the truss divided by stress allowed. Stress allowed is equal to the yield strength divided by the safety factor. The yield strength of A500 structural steel I found online is 345 MPa or 50,000psi. I went with grade C A500 steel because it is the most commonly used in engineering. The safety factor was given to me in the problem and is 3.5. I got a final area of the minimum cross-sectional are being 385.1mm^2. I then needed to know how long each of the sides are off the cross-section, so I took the square root of that number because the trusses are square, and I got 19.6 mm per side. To make the math easier and to make sure I am above the safety factor, I rounded up to 20 mm per side.

#### Approximate Weight of Truss

<img width="294" height="144" alt="image" src="https://github.com/user-attachments/assets/942e42f8-8042-4064-bda0-08cdf95f8420" />

To find the approximate weight of the truss, I first had to do a little research. I know weight is equal to density multiplied by volume, but I don't know the volume of A500 grade C structural steel. After searching, I found the density to be .282 lb/in^3. I then found the total length of all the truss members and multiplied it by the cross-sectional area to get the volume. I then converted the volume from meters to inches so that my units would remain consistent. Lastly, I found the approximate weight by multiplying my found volume by the density I researched and got my truss weighs about 24lbs.

#### Cross-Sectional Area and Weight of Pins

<img width="316" height="385" alt="image" src="https://github.com/user-attachments/assets/e597ffee-4210-4215-8539-f297a843de77" />

Finding the cross-sectional area of the pins was pretty straightforward after already doing a relatively similar process for the truss. I started with my knowns and unknowns so I know what I have and what I need. We were given the yield strength of 170ksi, the density of .278 lb/in^3, a safety factor of 4, and that we are using a single-shear connection. Previously, I also found the Ay and By support forces. What I didn't know was the weight, the shear force, or the cross-sectional area. So I started by finding V. V is just the shear force acting through the pins, and since these pins are support pins, we can find it by getting the magnitude of the support forces Ay and By, which equaled to be 6.67kN. Then I took my shear stress equation tau=V/A and derived it down until I got the equation Amin= V/ (yield strenght/safety factor). I then converted the units for yield strength and shear force so that all my units would be consistent for finding weight later. After plugging in my values, I got that the minimum area of the pins is 0.0353in^2. I then used that to find the cross-section by rearranging the formula for the area of a circle, A = pi (d)^2/4, to get d=the square root of 4A/pi. After plugging in the values, I got that the diameter of the pins are .212in. Lastly, I needed to find the approximate weight of all the pins combined. I used the same equation I used for the truss, which is W=density multiplied by volume. The only thing different is I had to multiply that product by 4 to account for all 4 pins. After plugging in values, I got W=.0393L. L is not solved for yet because it is a dependent variable on how long I make the pins.

## CAD Modeling the Truss system

<img width="723" height="280" alt="image" src="https://github.com/user-attachments/assets/92fc0898-4731-4c2d-93a2-475c1432fc98" />

To start with the model, I thought it would be easiest to just make the framework and add in the geometry. I converted everything to millimeters and added the dimensions to prepare for an extrude. But I quickly ran into a problem as my angled members (members BC and AD) weren't closing, and I couldn't extrude until they were closed geometry. So I had to start experimenting to find how to close these sketches.  

<img width="276" height="257" alt="image" src="https://github.com/user-attachments/assets/d3162d8a-0784-4a44-a7df-4285a5f49264" />

At first, I thought I didn't add all the lines to enclose the shape, so I tried overlapping a line onto the shapes that were already enclosed. But that didn't work, and the geometry still came up open.

<img width="423" height="150" alt="image" src="https://github.com/user-attachments/assets/41969e46-bf0c-4d52-b38b-ce52912760d5" />

So then I went ahead and extruded the sketches that were enclosed to see if I could add onto it later and that might fix my open geometry.

<img width="475" height="174" alt="image" src="https://github.com/user-attachments/assets/ed4f9e2d-ad70-4492-85ad-d3b8d61cf7de" />

<img width="653" height="192" alt="image" src="https://github.com/user-attachments/assets/16581ad6-213e-4d4f-9292-e15b463c948b" />

That idea ended up working, and when I added another sketch onto the same plane as before (I chose the top plane), the geometries came up enclosed. However, I was skeptical that when I extruded it, they wouldn't come up connected and it would have a line in between the two extrudes showing they weren't one solid figure. But that did not happen, and it all came out as one solid shape.

<img width="576" height="239" alt="image" src="https://github.com/user-attachments/assets/ad98a56b-b4a3-485d-bc97-ffe435371f59" />

<img width="666" height="263" alt="image" src="https://github.com/user-attachments/assets/f078b1e5-fe4e-4535-b5b5-2b7ac4f4af1e" />

 I then needed to add the last slanted member (member AC), which I had a little trouble with. I started by adding a third sketch onto the top plane and adding in the lines as I did for the last two members. But when I did that, it came out way out of dimension and not the right lengths.

<img width="529" height="212" alt="image" src="https://github.com/user-attachments/assets/7472a1f7-6a45-42dc-906d-b540d6a7578c" />

<img width="184" height="166" alt="image" src="https://github.com/user-attachments/assets/bacab80a-1ecd-4749-9705-4f2c6c190d01" />

 But I quickly realized my mistake and realized what I needed to do. I added a centerline from the vertices on the inside of A and C. This showed me where I needed to place my sketch to have it centered properly. I added the dimensions, making the width 20 mm, and added a dimension of 10mm from the centerline on each side so it would be centered. 
 
<img width="360" height="203" alt="image" src="https://github.com/user-attachments/assets/d80c1756-4ef0-4078-b726-9363b47034c4" />

This  is the final truss before adding the pinholes and pins.

<img width="448" height="280" alt="image" src="https://github.com/user-attachments/assets/851fa5d8-a58d-4fa3-a4d2-0c2f6b6261ac" />

<img width="397" height="257" alt="image" src="https://github.com/user-attachments/assets/5a954922-ef34-414c-bbfe-c15f64ac3961" />

<img width="229" height="250" alt="image" src="https://github.com/user-attachments/assets/77d9863b-62f0-4cbb-b6db-73fe6c9487ef" />

<img width="736" height="308" alt="image" src="https://github.com/user-attachments/assets/9f9763ac-5620-4ebf-8b59-6ebbf7df165a" />

Next, I had to add holes for each of my pins. I already found the minimum area, which is .0353 in^2 or .897mm^2 and the minimum diameter needed for the pins, which is .212 in or 5.38mm. So, to start modeling, I added two centerlines perpendicular to each other so I could extrude the hole in the center of the member. I did this for each pin hole.

<img width="215" height="185" alt="image" src="https://github.com/user-attachments/assets/6798b29a-1ad9-4851-9150-52d27cc513c2" />

<img width="262" height="292" alt="image" src="https://github.com/user-attachments/assets/134ef112-53af-498c-a931-a1cd3c27c8f7" />

<img width="192" height="215" alt="image" src="https://github.com/user-attachments/assets/ee5f8399-a221-4ddb-b3d1-f6a201775708" />

<img width="285" height="161" alt="image" src="https://github.com/user-attachments/assets/5ab98861-7df4-476d-b989-16a9670c6219" />

I then went and sketched a circle on each of the center points and made the diameter of the circles 5.38mm. These will be the pin holes.

<img width="646" height="273" alt="image" src="https://github.com/user-attachments/assets/19170665-46c3-4010-b824-54ccd2c281d3" />

<img width="206" height="220" alt="image" src="https://github.com/user-attachments/assets/6b170dad-993d-460f-85e3-012bfe23c2e8" />

<img width="767" height="242" alt="image" src="https://github.com/user-attachments/assets/dd7093e4-ac55-40e2-a9b2-5db7cda18e16" />

 Lastly, I did an extrude cut and set it to through all to finish the holes for my pins. This completes the CAD model before inserting the pins.
 
<img width="261" height="181" alt="image" src="https://github.com/user-attachments/assets/9ab41e35-e216-43d5-ba06-9561553ff59d" />

<img width="272" height="274" alt="image" src="https://github.com/user-attachments/assets/b32f628a-00eb-4e43-9b52-c6ab5e7228e6" />

 The pins themselves were very simple to create. I started a sketch on the top plane where I drew a circle and gave it a diameter of 5.38mm. I then extruded that circle to a length of 20mm which is the same length as the cross-section for the truss.

<img width="253" height="175" alt="image" src="https://github.com/user-attachments/assets/4b21e44a-5f00-4c68-9981-f09ef359c013" />

<img width="289" height="202" alt="image" src="https://github.com/user-attachments/assets/8ccb3237-de13-4437-88a4-bcb4b6c06c10" />

<img width="254" height="304" alt="image" src="https://github.com/user-attachments/assets/05e9cf35-ad95-4a34-90eb-12c78e8dabf8" />

<img width="159" height="211" alt="image" src="https://github.com/user-attachments/assets/9e5097c5-f80d-4886-88bb-34382bf77ca6" />

<img width="205" height="142" alt="image" src="https://github.com/user-attachments/assets/3a100540-b03b-4b19-906a-f1ba18b1bf2e" />

<img width="294" height="197" alt="image" src="https://github.com/user-attachments/assets/3f3caba3-2568-43f8-9eff-8fb4ad7fb3fc" />

 Lastly, I had to create an assembly to combine my pins and truss. I started by adding the truss and one of the pins and coincident the pin into place. I used the mate feature to first move the pin on the same center axis as the whole, then a second mate feature to align the top of the pin to the surface of the truss. I did the same process for all four pins.

 <img width="721" height="248" alt="image" src="https://github.com/user-attachments/assets/47abfc9c-0386-4404-823a-43686877b409" />

Here is my final product. The files to download my CAD model have been submitted on Canvas and are linked below.

[A2 truss aseembly.pdf](https://github.com/user-attachments/files/31767161/A2.truss.aseembly.pdf)

#### SolidWorks Mass Approximation

<img width="347" height="401" alt="image" src="https://github.com/user-attachments/assets/75c8077f-4715-46aa-94e6-34d26cc22d51" />

<img width="350" height="396" alt="image" src="https://github.com/user-attachments/assets/77245203-72c0-480f-bf62-ea3aa32ed099" />

I had a little trouble finding the approximate mass using SolidWorks at first because SolidWorks does not contain the materials we used in this assignment. I used A500 steel grade C and hardened tool steel. So, I had to manually create new materials and add the properties for each. I went online to find the properties, and my sources are linked below.

<img width="338" height="308" alt="image" src="https://github.com/user-attachments/assets/a16ecc87-ca39-458e-86e4-3da4c766ba54" />

After inserting my material values and setting the parts to the correct material, I was able to generate an approximate mass.

## Lessons learned
This assignment has taught me more about engineering and the engineering process than any other assignment I have done. I learned what it is like to be given basic criteria and actually free will to make decisions on what I am going to design and produce. In previous classes and school, I have been given a straightforward list of instructions and step-by-step guidance on what to do, but this assignment let me make the decisions and document it along the way, just like how engineering in the job field is like. I also learned how to make an assembly in SolidWorks. I've made an assembly in Creo before, but in SolidWorks I have only done parts before. So learning how to put the parts together was extremely useful and is a needed skill for the future. Lastly, I learned how to put my learnings in solids to use. Using a safety factor and yield strength to calculate minimum areas and cross sections, but it's for a real-life concept and something I designed, not another word problem.

I took a total of 10 hours to complete this assignment
## Sources

https://www.botopsteelpipes.com/wp-content/uploads/ASTM-A500-Grade-C-Specification.pdf

https://www.beamdimensions.com/materials/Steel/ASTM/ASTM_A500/#Grade_C

https://learnsolidworks.com/solidworks-tricks/measure-weight-solidworks


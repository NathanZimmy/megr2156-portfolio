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

TO find the approximate weight of the truss, I first had to do a little research. I know weight is equal to density multiplied by volume, but I don't know the volume of A500 grade C structural steel. After searching, I found the density to be .282 lb/in^3. I then found the total length of all the truss members and multiplied it by the cross-sectional area to get the volume. I then converted the volume from meters to inches so that my units would remain consistent. Lastly, I found the approximate weight by multiplying my found volume by the density I researched and got my truss weighs about 24lbs.

#### Cross-Sectional Area of Pins


## Analyze


## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

## Sources

https://www.botopsteelpipes.com/wp-content/uploads/ASTM-A500-Grade-C-Specification.pdf


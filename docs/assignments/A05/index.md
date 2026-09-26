# A5 – [Bracket Design]

## Objective
The purpose of this assignment is to design a component by analyzing the normal stress, bending stress, and stiffness equations using strength of materials to determine dimensions. The component we are designing is a simple bracket referencing the design given below. 

### Objectives listed on the assignment

Conduct stress analysis to determine appropriate dimensions for structural features.

Generate free body diagrams (FBDs) to visualize forces and constraints for each feature.\

Identify and document known and unknown variables, assumptions, and algebraic models for stress calculations.

Perform stiffness analysis to establish minimum required dimensions based on deflection constraints.

Compare stress and stiffness analyses to ensure structural integrity and compliance with given constraints.

Create detailed multiview sketches illustrating dimensions derived from both stress and stiffness analyses.

Reflect on and document key engineering lessons learned throughout the process.

<img width="333" height="317" alt="image" src="https://github.com/user-attachments/assets/708d10ee-a06f-486f-84fe-c09c32418e4e" />

<img width="490" height="227" alt="image" src="https://github.com/user-attachments/assets/783a4623-1f4f-4fce-a749-9a303c2bd780" />

### Criteria

The bracket’s dimensions are designed with different fit classes. Each dimension of the T beam is part of the fit:

“a” intention for use where accuracy is not essential
“b” is about the closest fits that can be expected to run freely
“c” is where accurate location and minimum play is desired

Design using a safety factor of 4 and applied load in between 500 lbf < F < 800 lbf. Choose one of three metals, aluminum 6061 T6, Steel (ASTM A36), or Titanium (Ti-6Al-V4). Furthermore, state assumptions and approximations about the design in order to use fundamental strength of materials analysis. For example, use the proper stress analysis and deflection analysis where appropriate. Assume no failure due to direct shear stress. 
## Material choice
For this assignment, we were given three materials to choose from. Aluminum 6061 T6, Steel (ASTM A36), or Titanium (Ti-6Al-V4). I chose to go with Titanium (Ti-6Al-V4). Titanium (Ti-6Al-V4) has a yield strength of 1100 MPa (160,000 psi), a modulus of elasticity of 114 GPa (16,500 ksi), and a shear strength of 760 MPa (110,000 psi).

## Feature A

<img width="254" height="317" alt="image" src="https://github.com/user-attachments/assets/49c2b6b6-ea6b-4b1b-80c9-b3351e7e08bd" />

<img width="482" height="389" alt="image" src="https://github.com/user-attachments/assets/78aa630f-f56a-49f5-8ccc-58b4d1512968" />

For feature A, I assumed a length of 1.5in and that F=600lbf. I used these to then calculate my Z and r values using the equations given in Appendix A. 

<ins>stress</ins>
To solve for the radius required by stress, I used the equation given to us in Appendix A. I first had to solve for Z and then plug in my values to get r=.306in. To find the stress, I used the stress equation given Wl/2Z, which came out to be 40000psi. I checked to make sure this was okay by finding my stress allowable and found that they were the same value. 

<ins>Stiffness</ins>
We were given a max deflection to be .005in. So when solving for stiffness, I had to take this into account and compare my values. When I solved for stiffness, I found that my calculated deflection was going to be .0119in and this is greater than the max deflection, so that means that the radius I found previously due to stress would not work. I then had to solve for radius due to deflection, and I got that the minimum required radius is .380in. This shows that stiffness dictates what size the radius needs to be on this design. 

## feature B

<img width="251" height="329" alt="image" src="https://github.com/user-attachments/assets/7bfeaca8-7be8-4cb9-8fe8-b7445139e15e" />

For feature B, I assumed a length of 1in and a width of .5in.

<ins>stress</ins>
To find the base required by stress, I used the quation stress=P/A. A = bw, so I can solve for b by rearranging the equation and plugging in my values. I calculated b to be .060in.

<ins>stiffness</ins>
To solve for stiffness, I used the equation stiffness=PL/EA and used that A=bw. Doing the same system as before, I solved b to equal .0291in. This means that stress will govern the dimension since it is the larger value.

## Feature C


<ins>stress</ins>
For feature C we were instructed to act as if it was a simple supported beam with a concentrated load at the center. SO to find the height due to stress I first had to find what my support values were using statics. Since there are only forces in the y which is the force from B then RA and RB are going to be the same value at 1/2 P. Nex I used the equation stress=MC/I and plugged my values in. I had to find the Mmax as well since that was the first variable needed and then I plugged I and C in since but didn't solve them yet because they both contain h. After rearranging my variables and plugging in my values I found the minimum height due to stress to equal .367in.

<ins>stiffness</ins>
To find the height due to stiffness I used the equation δ=PL^3/48EI. We know I=wh^3/12 so I plugged that in and solved for h. I found that the minimum height due to stiffness is .291in. This value is smaller than the minimum height due to stress so stress will govern the heigh of feature C.

## Feature D

​<ins>stress</ins>
Feature D was very simple as it was just on of the force acting on feature C previously. So our P=600 (half of PC) and i used the stress equation to find the minimum base thickness due to stress is .0300in. 

<ins>stiffness</ins>
for the minimum base due to stiffness I used the basic deflection equation and plugged in that area is L*b. After solving for b i found the minimum required base thickness due to stiffness is .00727in. This is much smaller than stress showing that stress controls the value. 

## Feature E

<ins>stress</ins>
## Sources
https://www.aerospacemetals.com/wp-content/uploads/2023/07/Titanium-Ti-6Al-4V-Grade-5-STA-Data-Sheet.pdf


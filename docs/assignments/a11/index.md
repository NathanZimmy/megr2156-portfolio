# A11 – Motor Selection

## Analyze and Design Frame - Austin Williams

### FEA: Top of the Frame

Model Setup - The boundary conditions are set by adding the necessary fixtures and forces onto the frame piece as seen below.

<img width="544" height="222" alt="Screenshot 2026-11-18 182818" src="https://github.com/user-attachments/assets/3128e302-bae8-43ac-a537-9f5ffb4f2830" />

Mesh Creation - here is the mesh that was needed to be able to run the simulation

<img width="875" height="512" alt="image" src="https://github.com/user-attachments/assets/26caceb9-0c87-4d9a-b89b-a6004ebb59a6" />

A finer Mesh for convergence -

<img width="465" height="525" alt="image" src="https://github.com/user-attachments/assets/28d0101f-a0b8-4c1b-a62b-f84601591f18" />

### Results to Report -

1. Max Von Mises Stress -

<img width="829" height="393" alt="Screenshot 2026-11-18 183341" src="https://github.com/user-attachments/assets/edd5876c-afa7-4a25-8379-1feb383cbe28" />

<img width="149" height="350" alt="image" src="https://github.com/user-attachments/assets/1618150f-e076-4907-814f-aff275b1cc4d" />

2. Max vertical deflection -

<img width="764" height="342" alt="Screenshot 2026-11-18 183404" src="https://github.com/user-attachments/assets/e4e37f65-8f69-4783-8d56-4536579758a6" />

<img width="107" height="335" alt="image" src="https://github.com/user-attachments/assets/e7fde29e-9dd8-43c3-91f9-02d162448271" />

3. Factor of Safety - 3.61

4. Brief Discussion - I noticed that the deflection looked very high, and I was worried at first, but then I looked at the actual data and noticed that there was a very small (1/10th of a mm) amount of total deflection. The load path was direct through the frame as the lead screws would end up transmitting most of that force to the frame and the amount of twist from the motor was not actually that high after all.

### Optimization Pass -

1. Targeted changes - I would not propose any major changes as the frame was able to withstand the forces without any major deflection or issues with the factor of safety. I may end up adding more filets to make the design seem more pleasing to the eye, but for now I want to focus on finishing the required part of the assignment before making extra changes.

2. Shift in Critical Locations - There was not any major shift in critical locations that would cause any portion of the frame to become misaligned with the critical parts of the design.

FEA: Side Bars of the Frame

Model Setup: The Forces fixture geometry was reversed from the top of the frame and is shown below

<img width="421" height="198" alt="Screenshot 2026-11-18 190108" src="https://github.com/user-attachments/assets/6adcf266-ae76-4ff4-a13d-332e370f19b5" />

Meshing and verification - I used the same mesh for this part of the frame in order to ensure consistency within the entire FEA for the frame.

<img width="386" height="575" alt="image" src="https://github.com/user-attachments/assets/33c66b6c-fb80-4972-8c8e-82c4379202df" />

A more fine mesh for convergence:

<img width="223" height="482" alt="image" src="https://github.com/user-attachments/assets/3702cea7-ff5e-41ae-8733-c786c1624baa" />

Results to Report -

1. Von Mises Stress:

<img width="671" height="494" alt="image" src="https://github.com/user-attachments/assets/6d969934-d49d-4c5c-9404-3308f3a9964f" />

2. Deformation:

<img width="387" height="577" alt="image" src="https://github.com/user-attachments/assets/9f4169f8-fc73-4ea3-b956-7ea56f16b4f7" />

3. Factor of Safety: 3.517

4. Brief Discussion: The stresses and deformation was slightly higher here than they were on the top part of the frame which was a little surprising because the forces do not act directly on the sides as they do on the top, but the sides are much longer so it does line up with the calculations from earlier. I would not change anything at this time because the factor of safety is still high and there are no stress concentrations in critical areas where I could end up seeing a failure point.

Optimization Pass -

1. Targeted Changes: I would target to leave these alone as they work for the assignment and in the past when I tried to get fancy with designs using my limited CAD skills, it has caused me more headache than help. Therefore, since all necessary target points are within constraint, I will be leaving this side portion of the frame in place to ensure that the Tensile Tester works properly if we were to actually build this in real life.

2. Critical Shift - Again, for this part of the frame, there were no shifts in critical locations or point along the frame where connections are. If there were critical shifts, the connections could be taking on more stress and end up failing due to unexpected load. The only part that I was originally worried about was the flex in the middle causing stress on the connection points, but then I realized that the endpoints will be connected to the other part of the frame and they will provide extra support so where the sidebar will not even have the same amount of flex as seen in the other pictures.


## Motor Mount Design (Nathaneal)

<img width="619" height="746" alt="image" src="https://github.com/user-attachments/assets/05a0a73b-2f1f-48a8-98c5-19b67545362d" />

<img width="1432" height="585" alt="image" src="https://github.com/user-attachments/assets/0ac75c0c-6bd3-42cc-902e-759945ea13b3" />

Here is the motor we selected in a SolidWorks file as well as the part drawing with dimensions included off the website. 

<img width="956" height="838" alt="image" src="https://github.com/user-attachments/assets/06aeacd1-5726-4dc4-8a9f-5c93fb6d5ea5" />

<img width="369" height="329" alt="image" src="https://github.com/user-attachments/assets/bc79551f-1ada-49d8-a473-c8618c779f5c" />

<img width="1053" height="1044" alt="image" src="https://github.com/user-attachments/assets/f6798317-501d-4c39-9672-fa8eb0888b3e" />

To start with the motor mount model I made a square base of 86mm by 86mm and extruded it to 10mm thick. I then made the shaft hole and an indention for the outer ring of the top. I made the shaft hole a 16mm diameter because the diameter of the shaft is 14mm and we want a snug fit but enough room to spin. I made the indention of the ring a little tighter tolerance because it needs to fit smoothly to the front surface of the motor. 

<img width="1079" height="891" alt="image" src="https://github.com/user-attachments/assets/d469df90-578a-417b-808b-33512886fdea" />

Next I made the screw holes going off the dimensions of the drawing and creating a hole through all. 

<img width="1010" height="726" alt="image" src="https://github.com/user-attachments/assets/3e4c3b1b-c28f-4b6d-8f66-9a9f90e7c598" />

Lastly I added fillets to all the outer corners with a radius of 4.5mm to match the face of the motor and keep it smooth. 

<img width="870" height="892" alt="image" src="https://github.com/user-attachments/assets/335c381b-1c5a-4b41-819d-ed4d24f290d4" />

<img width="1025" height="410" alt="image" src="https://github.com/user-attachments/assets/4c8192ad-9ff0-48d5-a808-764dcea9bf26" />

To test the fitments and clearances I ran a quick assembly to make sure everything looked good and fit properly. 

<img width="555" height="459" alt="image" src="https://github.com/user-attachments/assets/2b70ec34-f98c-440f-a354-52b1c6c6cdb1" />

Here is the motor and motor mount mated to the assembly.

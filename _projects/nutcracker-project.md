---
title: Nutcracker Project
layout: project
permalink: /projects/nutcracker-project/
---

Design problem: Imagine you have a macadamia nut that you want to crack open by hand using a simple lever nut cracker.

a) Draw a figure of the nut cracker with the nut when it’s about to crack. Calculate the necessary dimensions of the nutcracker and come up with a design to make this task feasible. You can assume a very simple geometry for the nutcracker to make your calculations easier.

Given:
Required load to crack nut = 222.18 kg (2178 N)
Grip strength = 300 N
Size of nut = 2.5 cm

Find:
Dimensions of nutcracker

Plan:
1. Draw free body diagram
2. Moment balance at joint
3. Determine length
4. Determine height


Solution:

<p align="center">
<img src="https://github.com/user-attachments/assets/e2f10877-5e3e-4e08-bdf0-81f3e46503d6" width="450">
</p>


Moment balance:

Sum of moments = 0

ln * Fn - lc * Fa = 0

lc / ln = Fn / Fa

lc / ln = 2178 / 300

lc / ln = 7.26

lc = 7.26 ln


From similar triangles:

lc / ln = Hc / Hn

Hc / Hn = 7.26


Hc = 7.26 Hn

Hc = 7.26 (2.5 cm)

Hc = 18.15 cm


Solve for ln assuming lc = 20 cm:

ln = lc / 7.26

ln = 20 / 7.26

ln = 2.75 cm


If the length of the nutcracker is 20 cm long then the nut must be placed 2.75 cm away from the joint.


b) Discuss the usability of the nutcracker that you designed

If Hc is 18.15 cm, that is too large for a hand to comfortably grip and apply force to crack the nut. This design is therefore not very practical or ergonomic.


c) Now, instead of relying on grip strength to apply the input force, modify your design to use a linear actuator.

Given:

Linear Actuator: IP65 Mini Linear Actuator  
Stroke: 1–40 inch  
Force: 16–225 lbs  
Stroke length: 1 inch  
Closed length: 5.13 inches


Find:
New dimensions


Plan:
1. Free body diagram
2. Moment balance
3. Determine lengths


Solve:

<p align="center">
<img src="https://github.com/user-attachments/assets/c39f050f-68a6-46bf-9f85-53a33b35d7c4" width="450">
</p>


Moment balance:

ln * Fn - lc * Fa = 0


lc / ln = Fn / Fa

lc / ln = 2178 N / 751.75 N

lc / ln = 2.89


Assume lc = 20 cm

ln = 20 / 2.89

ln ≈ 6.9 cm


Using similar triangles:

lc / ln = Hc / Hn

Hn = (ln * Hc) / lc


Convert actuator length:

5.13 in × 2.54 cm/in = 13.03 cm


Hn = 13.03 / 2.89

Hn ≈ 4.50 cm


Since Hn is greater than the size of the nut (2.5 cm), the design must be modified so that the closed position has Hn = 2.5 cm.


New design:

<p align="center">
<img src="https://github.com/user-attachments/assets/65523ea4-8bad-464c-b851-6363986b35f1" width="450">
</p>

New Design Problem:  
Initially, the handles were considered in the design to be rigid. Now, assume the nutcracker handles are no longer rigid. The handles are modeled as beams that bend due to the combined action of the forces from the nut and from the actuator. Only the force components transverse to the beam are considered.

a) Find the location of maximum elastic deflection in the handles. State assumptions clearly and describe the analysis.

b) Choose a beam design, including cross-section and material, such that the vertical elastic deflection is below 2% of its length and is as mass-efficient as possible.

c) Present the final design in an image or drawing.

Given:

Nut force, Fn = 2178 N  
Actuator force, Fa = 751.75 N  
Handle length, lc = 20 cm = 0.20 m  
Nut location, ln = 6.9 cm = 0.069 m  
Maximum allowed deflection = 2% of handle length  

Find:

Location of maximum deflection  
Beam material and cross-section  
Final handle design  

Plan:
1. Draw free body diagram of one handle
2. Model the handle as a beam
3. Identify where maximum deflection occurs
4. Use the deflection limit to choose a cross-section
5. Choose a mass-efficient material and shape

Solution:

Free body diagram:

<p align="center">
<img src="[YOUR_IMAGE_LINK_HERE](https://github.com/user-attachments/assets/b56c1f42-9b21-4e15-b14d-6d90034cdfb2)" width="450">
</p>

Maximum deflection location would be near the end of the handle, where the actuator is attached at x = lc = 20cm.

δmax ≤ 0.02L

L = 0.20 m

δmax ≤ 0.02(0.20)

δmax ≤ 0.004 m

δmax ≤ 4 mm

Beam Design:

Increasing height would be the most efficient way to reduce bending, and in terms of material, aluminum should be used because it's lightweight but is still strong and has a sufficient Young's modulus. A rectangular hollow aluminum section would be best because it provides a high second moment of area while keeping mass low. The taller dimension should be oriented vertically to maximize resistance to vertical bending.

Height h = 40 mm = 0.040 m  
Width b = 20 mm = 0.020 m  
Thickness t = 2 mm = 0.002 m  


Moment of inertia:

I = [bh³ − (b−2t)(h−2t)³] / 12  

I = [(0.020)(0.040)³ − (0.016)(0.036)³] / 12  

I = 4.45 × 10⁻⁸ m⁴  

Deflection calculation:

δ = δ_actuator + δ_nut  

Actuator contribution:

δ₁ = (F_A L³) / (3EI)  

δ₁ = (751.75 × 0.20³) / [3(69×10⁹)(4.45×10⁻⁸)]  

δ₁ ≈ 0.00065 m  

Nut contribution:

δ₂ = (F_N a²(3L − a)) / (6EI)  

δ₂ = (2178 × 0.069² (3×0.20 − 0.069)) / [6(69×10⁹)(4.45×10⁻⁸)]  

δ₂ ≈ 0.00030 m  

δ ≈ 0.00065 + 0.00030  

δ ≈ 0.00095 m  

δ ≈ 0.95 mm which is less than 4mm

Final design:

Material: Aluminum 6061-T6 (From Appendix C in textbook)
Cross section: Hollow rectangular tume

Dimensions:

- Height: 40 mm  
- Width: 20 mm  
- Thickness: 2 mm

<p align="center">
<img src="[YOUR_IMAGE_LINK_HERE](https://github.com/user-attachments/assets/16b0769b-b856-4ee1-a27f-88f6150e34cd)" width="450">
</p>

Conclusion:

The handle can be modeled as a beam with point loads from the nut and actuator. Using Aluminum 6061-T6 and a hollow rectangular cross-section makes the design lightweight while limiting deflection to less than 1 mm, which is below the allowable 4 mm.
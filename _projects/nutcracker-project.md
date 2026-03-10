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
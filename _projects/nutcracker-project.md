---
title: Nutcracker Project
layout: project
permalink: /projects/nutcracker-project/
---

<script type="text/javascript" id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>
<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$', '$$'], ['\\[', '\\]']]
    }
  };
</script>

Design problem: Imagine you have a macadamia nut that you want to crack open by hand using a simple lever nut cracker.

a) Draw a figure of the nut cracker with the nut when it’s about to crack. Calculate the necessary dimensions of the nutcracker and come up with a design to make this task
feasible. You can assume a very simple geometry for the nutcracker to make your
calculations easier.

  Given: Required load to crack nut: 222.18 kg or 2178 N
        Grip strength: 300 N
        Size of nut: 2.5 cm

  Find: Dimensions of nutcracker
  Plan: 1) FBD
        2) Moment balance at joint
        3) Determine length
        4) Determine height

  Solution: 
  ![IMG_0189](https://github.com/user-attachments/assets/e2f10877-5e3e-4e08-bdf0-81f3e46503d6)

  ```python
  $\sum M = l_n x F_n - l_c x F_a = 0, \qquad 
  \frac{l_c}{l_n} = \frac{F_n}{F_a} = \frac{2178}{300} = 7.26, \qquad 
  l_c = 7.26\,l_n, \qquad 
  \frac{l_c}{l_n} = \frac{H_c}{H_n} = 7.26, \qquad 
  H_c = 7.26\,H_n = 7.26(2.5\text{cm}) = 18.15\text{cm}, \qquad 
  l_n = \frac{l_c}{7.26}, \qquad 
  l_n = \frac{20\text{cm}}{7.26} = 2.75\text{cm}$

  ```

  If the length of the nutcracker is 20cm long then the nut must be 2.75cm away from the joint.

b) Discuss the usability of the nutcracker that you designed

  If Hc is 18.15cm, that's too large for a hand to grip, much less apply force to crack the nut. This design as is isn't usable.
  
c)  Now, instead of relying on grip strength to apply the input force, modify your design to use a linear actuator.

  Given: Linear Actuator: IP65 Mini Linear Actuator, Stroke: 1-40 inch, Force: 16-225 lbs, Stroke length: 1", Closed length: 5.13"

  Find: New dimensions

  Plan: FBD, moment balance, Determine Lengths

  Solve: 

  ![IMG_0189 2](https://github.com/user-attachments/assets/c39f050f-68a6-46bf-9f85-53a33b35d7c4)

```python
  $\sum M = l_n x F_n - l_c x F_a = 0$

$\frac{l_c}{l_n} = \frac{F_n}{F_a}
= \frac{2178\text{N}}{751.75\text{N}} = 2.89$
Use lc = 20cm, so ln = 6.9cm
$\frac{l_c}{l_n} = \frac{H_c}{H_n}, \qquad
H_n = \frac{l_n H_c}{l_c}$

$H_n = \frac{5.13\text{in}\left(\frac{2.54\text{cm}}{1\text{in}}\right)}{2.89}
= 4.50\,\text{cm}$
```

Hn is greater than the size of the nut, so the design must be modified so that the closed position Hn = 2.5cm
  
New Design:  
![IMG_0189 3](https://github.com/user-attachments/assets/65523ea4-8bad-464c-b851-6363986b35f1)

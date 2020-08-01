---
layout: post
author: Sanket Kundu
title: Humanoid Robotic arm
date: 2020-03-14T06:40:18.719Z
thumbnail-img: /assets/img/posts/assembly2.jpg
category: Arduino,3D printing,Nema motors
summary: Humanoid robotic arm made using 3d printed parts,nema (stepper motors)
  and controlled using arduino and interfaced with pronterface.
keywords: Humanoid robotic arm,Nema motors,using pronterface
thumbnail: /assets/img/posts/post-img.png
permalink: /blog/Humanoid robotic arm
---
Hello! My next creation(more likely training) was **Humanoid Robotic Arm**!

This project was done as an internship at Li2 pvt ltd during the period of 10th January to 10th February.

Li2 pvt ltd gave an opportunity to show case our skills in arduino as well as manupulation of softwares for the need of the project,the supportive staff and environment always encouraged me.

The Project was done and made possible with help of my friend.So I will share maximum I can about the project which we did as an intern.

**1st week**:
We started with gathering details,checking the inventory according to BOM given in the website of [BCN3D](https://www.bcn3d.com/bcn3d-moveo-the-future-of-learning/#) .
It is fully open source 3D printed robotic arm.

The project had some changes according to our level of knowledge,hence it was decided to be moved in only 2 directions z axis and y axis.

For reference I made an approximate drawing for the location of the motors and its appearance

Fig: drawing :

![drawing](/assets/img/posts/diagram.jpg "drawing"){:class="img-fluid"}

These are some of the main components we used:(more are given in BOM ([pdf](https://drive.google.com/file/d/14LHNKQbmhss2dg5fZe8fYuVJrBUtA915/view?usp=sharing)))

Fig: arduino mega:

![arduino mega](/assets/img/posts/arduino-mega.jpg "arduino mega"){:class="img-fluid"}

Fig:Stepper Motor SM42HT47(nema 17):

![Stepper Motor SM42HT47(nema 17)](/assets/img/posts/stepper-motor-sm42ht47-nema-17-.jpg "Stepper Motor SM42HT47(nema 17)"){:class="img-fluid"}

Fig: Nema23:

![Nema 23](/assets/img/posts/nema-23.jpg "Nema 23"){:class="img-fluid"}

Fig: Stepper motor driver (tb6560):

![Stepper motor driver (tb6560)](/assets/img/posts/tb6560.jpg "Stepper motor driver (tb6560)"){:class="img-fluid"}

Fig: Gear Ratio 51 Planetary Gearbox Nema 17 Stepper:

![Gear Ratio 51 Planetary Gearbox Nema 17 Stepper](/assets/img/posts/gear-ratio-51-planetary-gearbox-nema-17-stepper.jfif "Gear Ratio 51 Planetary Gearbox Nema 17 Stepper"){:class="img-fluid"}

Fig: Servo:

![Servo](/assets/img/posts/servo-motor.jpg "Servo"){:class="img-fluid"}

Fig:Power supply 24V:

![Power supply 24V](/assets/img/posts/24-v-power-supply.jpg "Power supply 24V"){:class="img-fluid"}

Fig:Jumper wires:

![Jumper wires](/assets/img/posts/cables.jfif "Jumper wires"){:class="img-fluid"}

**2nd week**:
We started learning 3D printing from the incharge ,have a look what it looked like!!
Video:3d printer view (https://youtu.be/Bhml2e7C60I)

<iframe width="560" height="315" src="https://www.youtube.com/embed/Bhml2e7C60I?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

The gripper parts after 3D printing.
Fig: 3D printed gripper parts:

![3D printed gripper parts](/assets/img/posts/3d-printed-gripper.jpg "3D printed gripper parts"){:class="img-fluid"}

The base and middle part
Fig: Base and Mid part:

![Base and Mid part](/assets/img/posts/mid-part.jpg "Base and Mid part"){:class="img-fluid"}

It took almost took 2 weeks just to gather the things because of delay in delivery and availability of the components in the market,we had to go market about 5 or 6 times,just because of unavailability and sometimes because of our mistakes.

**3rd week**:
We started assembly after completion and ongoing printing of some parts
Here is the logic diagram
Fig: Logic:

![ Logic](/assets/img/posts/diagram.png " Logic"){:class="img-fluid"}

The base was assemble first without motors,as it was important to check whether the parts fit according to the requirements.
Fig: Assembly1:

![Assembly1](/assets/img/posts/assembly-1.jpg "Assembly1"){:class="img-fluid"}

Since the top were still being printed (each print took 6-7 hours) , the assembly of the gripper was done

Fig: Gripper:

![Gripper](/assets/img/posts/gripper.jpg "Gripper"){:class="img-fluid"}

After printing all the parts we started testing the motors arrived according to the specifications.
We assembled all the motors with the parts,it was time taking task as the parts had to be opened again and each screw had its importance (we had to search many times as they used to roll away).

After assembly it looked like this
Fig: Assembly 2:

![ Assembly 2](/assets/img/posts/assembly2.jpg " Assembly 2"){:class="img-fluid"}

Still we had to check whether the motors work under the load of the bolts
We started with the upper body and voila!!
 We encountered our 1st problem!!

The upper motor wasn’t responding properly:

Video:upper motor failure(https://youtu.be/66UEDwFwmCo)

It took 2 days to rectify it
Video:upper motor test(https://youtu.be/XTS9jxpSqSc)

The only way to know other motors worked was to test after assembly of everything .The model was assembled without second thought about the base and we ended up having no base to keep the structure.The platform was searched and it was decided that the whole assembly had to be bolted down to a platform(we had to unscrew everything again!!!)

Fig :Before assembly:

![Before assembly](/assets/img/posts/before-formation.jpg "Before assembly"){:class="img-fluid"}

After we assembled:

Fig:Formation side view:

![Formation side view](/assets/img/posts/formation-side-view.jpg "Formation side view"){:class="img-fluid"}

Fig:Formation:

![Formation](/assets/img/posts/formation.jpg "Formation"){:class="img-fluid"}

**4th week**:

After the assembly was bolted and assembled properly(finally!!!) ,the first test was run.
and guess what?it was complete failure.

Video:test 0(https://youtu.be/1j0MBw1Di8U)

To know the cause, we dismantled it

Video:test 0 problem(https://youtu.be/ZgJZGAjicaQ)

We arrived at our 2nd problem. 

Video: motor test not working(https://youtu.be/P8kmNxAdZOA)

The problem was still persisted after few attempts,but after testing so many times we got little bit information about the error.

Video: problem identification 1(https://youtu.be/AGgInzR-ozE)

It took few more attempts to understand the proper problem.
Video:problem identification 2(https://youtu.be/01uu97VMBLo)

It took 1 or 2 days and many attempts to rectify it.

Video:motor success(https://youtu.be/_gCgqmMDu0I)

This is the working model we recorded .
Video:final run (https://youtu.be/_FPGHSQDmDg)

Benefits I recieved from this project:
1.An entirely new experience
2.Team membership.
3.Knowledge of the Market cost of NEMA motors.
4.Operations performed by CNC machines.
5.How stepper motor works.
6.Knowledge of 3D printing,cost and designing.
7.Time management.
8.Knowledge of autodesk fusion to model different things.

A special thanks to my partner ,Harsh Biradar and Li2 pvt ltd. who gave me assistance in every turn.
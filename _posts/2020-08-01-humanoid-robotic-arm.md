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
thumbnail: /assets/img/posts/assembly21.jpg
permalink: /blog/humanoid-robotic-arm
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

![diagram](/assets/img/posts/diagram1.jpg "diagram"){:class="img-fluid"}

These are some of the main components we used:(more are given in BOM ([pdf](https://drive.google.com/file/d/14LHNKQbmhss2dg5fZe8fYuVJrBUtA915/view?usp=sharing)))

Fig: arduino mega:

![arduinomega](/assets/img/posts/arduinomega.jpg "arduinomega"){:class="img-fluid"}

Fig:Stepper Motor SM42HT47(nema 17):

![nema17](/assets/img/posts/17nema.jpg "nema17"){:class="img-fluid"}

Fig: Nema23:

![nema 23](/assets/img/posts/nema23.jpg "nema23"){:class="img-fluid"}

Fig: Stepper motor driver (tb6560):

![tb6560](/assets/img/posts/tb65601.jpg "tb6560"){:class="img-fluid"}

Fig: Gear Ratio 51 Planetary Gearbox Nema 17 Stepper:

![Gear Ratio 51 Planetary Gearbox Nema 17 Stepper](/assets/img/posts/gear-ratio-51-planetary-gearbox-nema-17-stepper.jfif "Gear Ratio 51 Planetary Gearbox Nema 17 Stepper"){:class="img-fluid"}

Fig: Servo:

![Servo](/assets/img/posts/servo-motor.jpg "Servo"){:class="img-fluid"}

Fig:Power supply 24V:

![24v power supply](/assets/img/posts/powersupply.jpg "24v power supply"){:class="img-fluid"}

Fig:Jumper wires:

![Jumper wires](/assets/img/posts/cables.jfif "Jumper wires"){:class="img-fluid"}

**2nd week**:
We started learning 3D printing from the incharge ,have a look what it looked like!!

<iframe width="560" height="315" src="https://www.youtube.com/embed/Bhml2e7C60I?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

The gripper parts after 3D printing.
Fig: 3D printed gripper parts:

![printedparts](/assets/img/posts/3dprintedgripper.jpg "printedparts"){:class="img-fluid"}

The base and middle part
Fig: Base and Mid part:

![basemid](/assets/img/posts/midpart.jpg "basemid"){:class="img-fluid"}

It took almost took 2 weeks just to gather the things because of delay in delivery and availability of the components in the market,we had to go market about 5 or 6 times,just because of unavailability and sometimes because of our mistakes.

**3rd week**:
We started assembly after completion and ongoing printing of some parts
Here is the logic diagram
Fig: Logic:

![logic](/assets/img/posts/logic.jpg "logic"){:class="img-fluid"}

The base was assemble first without motors,as it was important to check whether the parts fit according to the requirements.
Fig: Assembly1:

![assembly1](/assets/img/posts/assembly1.jpg "assembly1"){:class="img-fluid"}

Since the top were still being printed (
each print took 6-7 hours) , the assembly of the gripper was done

Fig: Gripper:

![gripper](/assets/img/posts/gripper1.jpg "gripper"){:class="img-fluid"}

After printing all the parts we started testing the motors arrived according to the specifications.
We assembled all the motors with the parts,it was time taking task as the parts had to be opened again and each screw had its importance (we had to search many times as they used to roll away).

After assembly it looked like this
Fig: Assembly 2:

![assembly 2](/assets/img/posts/assembly21.jpg "assembly 2"){:class="img-fluid"}

Still we had to check whether the motors work under the load of the bolts
We started with the upper body and voila!!
 We encountered our 1st problem!!

The upper motor wasn’t responding properly:

<iframe width="560" height="315" src="https://www.youtube.com/embed/66UEDwFwmCo?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

It took 2 days to rectify it

<iframe width="560" height="315" src="https://www.youtube.com/embed/XTS9jxpSqSc?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

The only way to know other motors worked was to test after assembly of everything .The model was assembled without second thought about the base and we ended up having no base to keep the structure.The platform was searched and it was decided that the whole assembly had to be bolted down to a platform(we had to unscrew everything again!!!)

Fig :Before assembly:

![before assembly](/assets/img/posts/beforeformation1.jpg "before assembly"){:class="img-fluid"}

After we assembled:

Fig:Formation side view:

![sideview](/assets/img/posts/formationsideview1.jpg "sideview"){:class="img-fluid"}

Fig:Formation:

![formation](/assets/img/posts/formation1.jpg "formation"){:class="img-fluid"}

**4th week**:

After the assembly was bolted and assembled properly(finally!!!) ,the first test was run.
and guess what?it was complete failure.

<iframe width="560" height="315" src="https://www.youtube.com/embed/1j0MBw1Di8U?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

To know the cause, we dismantled it

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZgJZGAjicaQ?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

We arrived at our 2nd problem. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/P8kmNxAdZOA?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

The problem was still persisted after few attempts,but after testing so many times we got little bit information about the error.

<iframe width="560" height="315" src="https://www.youtube.com/embed/AGgInzR-ozE?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

It took few more attempts to understand the proper problem

<iframe width="560" height="315" src="https://www.youtube.com/embed/01uu97VMBLo?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

It took 1 or 2 days and many attempts to rectify it.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_gCgqmMDu0I?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

This is the working model we recorded .

<iframe width="560" height="315" src="https://www.youtube.com/embed/_FPGHSQDmDg?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

Benefits I recieved from this project:
1.An entirely new experience
2.Team membership.
3.Knowledge of the Market cost of NEMA motors.
4.Operations performed by CNC machines.
5.How stepper motor works.
6.Knowledge of 3D printing,cost and designing.
7.Time management.
8.Knowledge of autodesk inventor to model different things.

A special thanks to my partner ,Harsh Biradar and Li2 pvt ltd. who gave me assistance in every turn.
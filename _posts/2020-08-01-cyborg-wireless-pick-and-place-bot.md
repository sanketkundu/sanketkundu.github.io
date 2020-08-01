---
layout: post
author: Sanket Kundu
title: Cyborg(Wireless Pick and place bot)
date: 2020-03-31T11:00:11.975Z
thumbnail-img: /assets/img/posts/m1ain.jpg
category: arduino,motors,mobility
summary: a small prototype of wireless pick and place bot used in military and
  industrial applications
keywords: cyborg,pick and place bot
thumbnail: /assets/img/posts/m1ain.jpg
permalink: /blog/Cyborg(pick-and-place-bot)
---
Hello!This is my 3rd project,related to robotics(using arduino).Done shortly after humanoid robotic arm.
The last internship provided us knowledge to built a gripper for our own use,the application here was however different.
Last project was immobile ,so we(me and my team mate) decided to apply on movable bot with wireless controls at our hand.
This took 1 month time.

The planning was made about the working design and the equipment needed.
The plan was divide into 2 parts.
1.Testing the compatibility of motors,remotes,microcontroller for this project.(to avoid the problem of building the whole thing and jumping at testing)
2.assembly and testing as whole.

The block diagram of the whole project was simple.
Fig:block diagram:

![block diagram](/assets/img/posts/block-diagram.jpg "block diagram"){:class="img-fluid"}

The components were brought in terms:
1.Fig:4 DC motors:

![4 dc motors](/assets/img/posts/4dc-motors.jpg "4 dc motors"){:class="img-fluid"}

2.Fig: Chasis:

![chasis](/assets/img/posts/chais.jpg "chasis"){:class="img-fluid"}

3.Fig: Arduino mega:

![Arduino mega](/assets/img/posts/arduino-mega.jpg "Arduino mega"){:class="img-fluid"}

4.Fig: Wireless remote:

![ Wireless remote](/assets/img/posts/remote.jfif " Wireless remote"){:class="img-fluid"}

5.Fig:Cables:

![cables](/assets/img/posts/cables.jfif "cables"){:class="img-fluid"}

6.Fig: 2 motor drivers(ln298N):

![l298n](/assets/img/posts/l298n.jpg "l298n"){:class="img-fluid"}

7.Fig:Bread board:

![breadboard](/assets/img/posts/breadboard.jpg "breadboard"){:class="img-fluid"}

8.Fig:Lead acid battery(12V):

![leadacid ](/assets/img/posts/bat.jpg "leadacid"){:class="img-fluid"}

9.Fig:Aluminium frame:

![aluminium](/assets/img/posts/webp.net-resizeimage-1-.jpg "aluminium"){:class="img-fluid"}

10.Fig:4 wheels:

![4 wheels](/assets/img/posts/wheels.jpg "4 wheels"){:class="img-fluid"}

11. Fig:gripper mechanism:

![gripper](/assets/img/posts/grip.jpg "gripper"){:class="img-fluid"}

With the help of arduino Ide the capability of 1 motor driver was tested using arduino nano.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_IHGFBZqqDA?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

So it was clear that with enough power supply 2 motors can be handled by 1 motor driver.

Soon I started working on remote control,since that was the essential part of the whole project
The remote used in testing was of my own(later we switched to new one).It communicated with the arduino using [processing](https://learn.sparkfun.com/tutorials/connecting-arduino-to-processing/all#shaking-hands-part-1).
The controls of the remote was assigned with the help of open source[ library](https://github.com/madsci1016/Arduino-PS2X) of ps controller.

it looked somewhat like this:

fig: interface:

![controller config](/assets/img/posts/controller-configuration.jpeg "controller config"){:class="img-fluid"}

i refered alot of websites to understand the code and made changes to them according to my remote.
Later we switched to the project remote and made changes with respect to that
We followed [this](https://create.arduino.cc/projecthub/electropeak/how-to-interface-ps2-wireless-controller-w-arduino-a0a813).

<iframe width="560" height="315" src="https://www.youtube.com/embed/SHIadfyKoNc?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

Changes in the codes were made for the 4 motors to run on the commands from the buttons in the remote.

<iframe width="560" height="315" src="https://www.youtube.com/embed/R65iKdqmpW0?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

The gripper was assembled in aluminium frame(we chose because it was light weight and strong enough to lift the load).

<iframe width="560" height="315" src="https://www.youtube.com/embed/dUHcaW6d7wk?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

The remote control was switched to ps2 remote and testing of 2 motors was done with that.

<iframe width="560" height="315" src="https://www.youtube.com/embed/i-iZ11XMtY8?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

It took few days to assemble everything properly with lot of test and failures.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Pdzf2LAYW0w?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

With all components the test run was made in small area,few errors were discovered in the program and as well as design,which were solved in further trials.

<iframe width="560" height="315" src="https://www.youtube.com/embed/LvdvFGiKxSY?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

This is the final run we had with all the components installed and working.

<iframe width="560" height="315" src="https://www.youtube.com/embed/vXyIbaD5Q_8?rel=0&amp;controls=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>
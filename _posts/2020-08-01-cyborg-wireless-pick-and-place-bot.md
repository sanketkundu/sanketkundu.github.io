---
layout: post
author: Sanket Kundu
title: Cyborg(Wireless Pick and place bot)
date: 2020-03-31T11:00:11.975Z
thumbnail-img: /assets/img/posts/main.jpg
category: arduino,motors,mobility
summary: a small prototype of wireless pick and place bot used in military and
  industrial applications
keywords: cyborg,pick and place bot
thumbnail: /assets/img/posts/main.jpg
permalink: /blog/Cyborg(pick-and-place-bot)
---
Hello!This is my 3rd project,related to robotics(using arduino).Done shortly after humonoid robotic arm.
The last internship provided us knowledge to built a gripper for our own use,the application here was however different.
Last project was immobile ,so we(me and my team mate) decided to apply on movable bot with wireless controls at our hand.
This took 1 month time.

The planning was made about the working design and the equipment needed.
The plan was divide into 2 parts.
1.Testing the compability of motors,remotes,microcontroller for this project.(to avoid the problem of building the whole thing and jumping at testing)
2.assembly and testing as whole.

The block diagram of the whole project was simple.
Fig:block diagram:

![block diagram](/assets/img/posts/block-diagram.jpg "block diagram"){:class="img-fluid"}

The components were brought in terms:
1.Fig:4 DC motors:

![4 DC motors](/assets/img/posts/4-dc-motors.jpeg "4 DC motors:"){:class="img-fluid"}

2.Fig: Chasis:

![Chasis](/assets/img/posts/chasis.jpeg "Chasis"){:class="img-fluid"}

3.Fig: Arduino mega:

![Arduino mega](/assets/img/posts/arduino-mega.jpg "Arduino mega"){:class="img-fluid"}

4.Fig: Wireless remote:

![ Wireless remote](/assets/img/posts/remote.jfif " Wireless remote"){:class="img-fluid"}

5.Fig:Cables:

![cables](/assets/img/posts/cables.jfif "cables"){:class="img-fluid"}

6.Fig: 2 motor drivers(ln298N):

![ln298n](/assets/img/posts/ln298n.jpg "ln298n"){:class="img-fluid"}

7.Fig:Bread board:

![breadboard](/assets/img/posts/breadboard.jpg "breadboard"){:class="img-fluid"}

8.Fig:Lead acid battery(12V):

![battery](/assets/img/posts/battery-12v-7ah-sealed-lead-acid.jpg "battery"){:class="img-fluid"}

9.Fig:Aluminium frame:

![aluminium frame](/assets/img/posts/aluminium-arm.jpeg "aluminium frame"){:class="img-fluid"}

10.Fig:4 wheels:

![4 wheels](/assets/img/posts/wheels.jpg "4 wheels"){:class="img-fluid"}

11. Fig:gripper mechanism:

![gripper mechanism](/assets/img/posts/gripper-mechanism.jpeg "gripper mechanism")
{:class="img-fluid"}

With the help of arduino Ide the capability of 1 motor driver was tested using arduino nano.
Video:motor testing(https://youtu.be/_IHGFBZqqDA)
So it was clear that with enough power supply 2 motors can be handled by 1 motor driver.

Soon I started working on remote control,since that was the essential part of the whole project
The remote used in testing was of my own(later we switched to new one).It communicated with the arduino using [processing](https://learn.sparkfun.com/tutorials/connecting-arduino-to-processing/all#shaking-hands-part-1).
The controls of the remote was assigned with the help of open source[ library](https://github.com/madsci1016/Arduino-PS2X) of ps controller.

it looked somewhat like this:

fig: interface:

![controller config](/assets/img/posts/controller-configuration.jpeg "controller config")

i refered alot of websites to understand the code and made changes to them according to my remote.
Later we switched to the project remote and made changes with respect to that
We followed [this](https://create.arduino.cc/projecthub/electropeak/how-to-interface-ps2-wireless-controller-w-arduino-a0a813).

Video:test1 muted(https://youtu.be/SHIadfyKoNc)

Changes in the codes were made for the 4 motors to run on the commands from the buttons in the remote.
Video: test 2 rotate(https://youtu.be/R65iKdqmpW0)

The gripper was assembled in aluminium frame(we chose because it was light weight and strong enough to lift the load).
Video:gripper arm(https://youtu.be/dUHcaW6d7wk)

The remote control was switched to ps2 remote and testing of 2 motors was done with that.

video:using ps2 remote(https://youtu.be/i-iZ11XMtY8)

It took few days to assemble everything properly with lot of test and failures.
Video:test 3(https://youtu.be/Pdzf2LAYW0w)

With all components the test run was made in small area,few errors were discovered in the program and as well as design,which were solved in further trials.
Video: 1st Run(https://youtu.be/LvdvFGiKxSY)

This is the final run we had with all the components installed and working.
Video: mute Final run(https://youtu.be/vXyIbaD5Q_8)
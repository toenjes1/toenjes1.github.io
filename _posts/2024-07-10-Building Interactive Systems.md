---
title: Building Interactive Systems
date: 2024-07-10
tags: [c, c-sharp, hardware, low-level, uni, unity, gamedev]
toc: false
comments: false
image:
    path: /media/bis/bis.png
    alt: the DualPanto interfacing with Unity
---

The Chair for Human-Computer Interaction at HPI ran a university lab on "what \[they] think of as 'full stack development'". This "full stack" is composed of electronics, low-level code, a communication layer, application code and the development cycle surrounding it. I found this very intriguing and luckily managed to secure a spot and participate.

In a team of two, we worked on the chair's own [DualPanto](https://hpi.de/baudisch/projects/dualpanto.html), a physical device that uses handles for providing haptic input/output on a 2D plane to visually impaired users. 

As a part of this course, we followed the design process up to the DualPanto by constructing haptic devices with fewer df and working our way up to the DualPanto. We started with a simple lever. It was our task to write microcontroller firmware that could, for instance, render a "wall" on this one axis of movement. That is, running the motor to oppose the user's force when pushing past a certain point. 

At the end of the process, we had assembled and soldered the DualPanto device and had written Proportional-Integral-Derivative (PID) real-time haptic firmware to render objects on a 2D plane for it. 
Additionally, we designed a PCB for a battery status indicator using LEDs in KiCAD that the chair then printed and incorporated into the device.

Lastly, we developed a simple game in Unity that could then be played on DualPanto. 

At the end of the semester, the chair invited visually impaired people to come and try out our and the other team's games. It was awesome to see our result being used by the target audience as opposed to only us.

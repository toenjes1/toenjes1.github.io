---
title: Contributing to FüSim MANV
description: Working on a large pre-existing code base
date: 2025-07-15
tags: [fullstack, ts, angular, uni]
toc: false
comments: false
image:
    path: /media/fuesim_manv/fuesim-manv.png
    alt: Screenshot from within the simulation
---

As part of my degree, I have taken several courses that incorporate substantial practical components into the lecture series, which is also the case for this lecture about software project organisation. The real core of the course was a group project in which we contributed directly to development codebases of a digital training simulation used by local German fire brigades. This was my first experience working within a large, pre-existing system, and it presented a set of challenges that differed significantly from my previous development work. Much of the architecture had to be inferred from the code itself, as documentation was incomplete, and the original developers were not often available for consultation. It also led to working with technologies which I do not favour personally or with which I had no prior experience. In some ways, the burden of designing architecture is relieved but then replaced by the burden of learning that foreign architecture and its implementation. 

A key aspect of the project was engaging with actual end users. We conducted structured interviews with fire brigade representatives to identify meaningful extensions to the simulation. Based on this feedback, our team implemented the requisites for a vehicle extrication scenario. This involved introducing multiple vehicle types as well as a general vehicle template for extensibility, modelling specialised rescue tools, and adding timers to certain cumbersome actions, whereas previously all actions taken by the personnel were simulated as instantaneous. 

From a technical perspective, the project required full-stack development from all team members. Its backend ran on node.js and was written in TypeScript, while the frontend used AngularJS and also TS. Based on the input we received during lectures, our workflow adhered to an agile SCRUM framework, with two-week sprints, related retrospectives, and sprint planning sessions. The latter included effort estimation and backlog prioritisation. Naturally, we used Git extensively, working with feature branches and incorporating structured merge reviews into our development cycle.

Overall, I feel that the project provided a realistic insight into collaborative software development in a professional context; in fact, it resembles how I now experience it at my student job now (barring the fact that the initial developers are present for consultation). It required not only technical work but also team communication and structured project organisation. Our project was ultimately awarded a grade of 1.3 (A−). You can check out the public production code base on [GitHub](https://github.com/hpi-sam/fuesim-digital), though our development codebases were private copies since all student groups worked on theirs simultaneously.

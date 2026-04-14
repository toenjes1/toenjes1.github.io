---
title: Participating in one of Europe's largest hackathons
description: One weekend to design and build a webapp for planning buildings in 3D
date: 2024-11-10
tags: [fullstack, js, react, vite, py, contest, hackathon]
toc: false
comments: false
image:
    path: /media/junction/junction.jpg
    alt: cheaky group photo
---

The Junction hackathon calls itself "one of the largest hackathons in Europe". Some friends and I decided to find out what it's all about. A hackathon is much like a [GameJam](/posts/18th-HPI-GameJam) in that it requires designing and building software quickly, the difference being that it's typically productive software and not a video game being built. 

![Desktop View](/media/junction/helsinki.jpg){: .w-50 .left}

We thus flew to Helsinki, where Junction takes place every year. This year, Junction had booked an event space in the _Kaapelitehdas_, an old cable factory turned cultural centre right by the harbour.

Junction and some partner companies had prepared several challenges, of which teams could choose one to compete in. Every challenge consisted of descriptions about the desired product with various levels of detail. Since team size was limited to five, and we were eight (one of us is indeed missing from the group photo), we split up into five and three. We figured that if we wanted the best possible chances at success, having one team reach the size limit would be more valuable than balancing the team sizes.

I joined the five-person team, and we settled on competing in KONE's challenge.

For this challenge, teams had to create software that takes the floor plans of a building and uses them to render it in 3D, where models of lifts and escalators (KONE's main products) should then be placeable. In essence, they wanted a clearer visualisation of the planning stage for incorporating lifts into buildings. Namely to better show their clients how the lift will be positioned in three-dimensional space.

So we developed **monoplan**. Our software consists of three main steps. The user interacts with our web app. First, the user can upload any number of floor plans for all the storeys of the building and input the storey height. Without even the press of a button, the walls of the building are intelligently detected within the floor plans and displayed on it. In the second step, the user has the option to readjust walls, delete them or add in more. Or the user moves right along to step three: the building is now rendered in 3D right inside your browser and the user may place any number of included KONE 3D lift assets anywhere within the model. And just like that, in only a few minutes any user can intuitively visualise planned lift shafts.

![Desktop View](/media/junction/junction_hall.jpg){: .w-50 .right}

As for our tech stack, the frontend is written entirely in React, with the 3D model being rendered by Three.JS. The whole page runs on Vite and connects to a Flask server where our smart detection system is running in Python. All code can be found on our [GitHub](https://github.com/DanielC04/Junction2024).

Over 1000 engineers gathered in this hall for Junction. Coding alongside all of them throughout the weekend was a blast. So was getting to know some of them, mostly after the challenge deadlines, of course (can't waste time!). 

Later, representatives of KONE came to our table where we were showcasing monoplan. While we did make it into the five-team shortlist, we unfortunately were not chosen for first. 

We had a great time nevertheless. Thanks to the HPI's PR department, who supported our trip, as is evident by our matching HPI T-shirts seen in our group photo.

Lastly, we created a pitch video for KONE in which you can see our web app in action!

{% include embed/youtube.html id='5qLezPhlHBE' %}

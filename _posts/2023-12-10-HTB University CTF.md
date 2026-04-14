---
title: Joining the HPI team to compete in HackTheBox's worldwide CTF
date: 2023-12-10
tags: [ctf, cybersec, contest]
toc: true
comments: false
description: My first CTF experience
image:
    path: /media/htb_ctf/hackthebox.jpg
    alt: just the HackTheBox logo
---

## Joining the student cybersecurity club

At HPI---as is the case at many universities---student clubs are an important part of campus social life and extracurricular activities alike. Shortly after I started my degree at HPI, I joined the cybersecurity club. I had been personally interested in cybersecurity for some years now. 

From then on, I participated in weekly meetings. Aside from organisational topics, we talked about recent events in the cybersecurity space or presented interesting bits and bobs---a scheduled section aptly titled "cool stuff". Additionally, we would sometimes internally play small competitive cybersecurity challenges on [HackTheBox](https://www.hackthebox.com/), one of the leading platforms for cybersecurity training material.

It did not take too long for me to be introduced to the club's larger-scale activities. Namely, this student club is active as the CTF team [Platypwnies](https://ctftime.org/team/112550) which is ranked 6th in Germany and 51st worldwide in 2024. 

In December, two months after joining the club, the worldwide HackTheBox university CTF became my first-ever CTF participation.

As the name implies, this event is only open to the CTF teams of specific universities such as, of course, the Platypwnies of HPI. It is worth noting that many of the world's best teams are independent teams with open recruiting for talent from all demographics and around the world. Naturally, local university teams are much more limited.

## But what even is a CTF?

CTF stands for "capture the flag" and refers to a type of cybersecurity competition. Multiple subtypes of CTF exist, but I will exclusively be referring to jeopardy-style CTFs and broadly calling them CTFs throughout. Such a CTF typically works as follows: 

The organisers of the event have prepared a number of _challenges_. The participants most often form teams. The CTF takes place over the course of a relatively short, strictly limited time frame, oftentimes a day or two. During this time, members of a team will attempt to solve the provided challenges. Solving a challenge generally consists of _capturing a flag_ (a specific string) from within the scenario provided by the challenge. 

These scenarios can vary and are usually categorised based on how they are structured.\
For instance, there are 
- web scenarios in which the players connect to a web server (instanced per team) on which the flag is located and from which is has to be extracted
- cryptography scenarios in which the flag is encrypted and has to be decrypted by the players somehow
- reverse engineering in which binaries were prepared that can output the flag in some way
- forensics in which files have to be downloaded and investigated
- in OSINT a trail of social media profiles, images, usernames/emails and more has to be tracked down

and many more. Scenarios that may pertain to specific technology such as LDAP or to custom situations. Sometimes backend code will be available to the players and has to be understood and analysed for vulnerabilities.

In any case, during the event, all teams are simultaneously and independently solving these challenges. Every submitted flag yields points for the team, with the number of points generally being based on the number of teams which have solved the flag. Importantly, the points a team receives for a flag can still decrease after submission, decreasing the team's point total when other teams solve that same challenge. 

At the end of the event's duration, the team with the most points wins. If a team manages to solve all challenges within the event, they win right away, as a higher point total cannot be achieved. Any further team solving all challenges will then be placed in the next highest rank. 

## The event itself

HTB's university CTF (2023) took place over the course of 48 hours and featured a wide array of CTF challenges from diverse categories, including web, crypto, reverse engineering, forensics and more. 995 universities from all six populated continents were signed up to compete. Each team was limited to 30 participants, which our team ended up being just shy of.

Since HPI closes during the night, we had previously organised an office space in which we could all stay for the duration of the event. Everyone brought sleeping bags; food and drinks were paid by the club's budget. 

And so the event days came, and we spent our weekend solving cybersecurity challenges. Small groups broke off and tackled different challenges; a digital board was used to keep track of this, and regular meetings were held to discuss challenges and exchange ideas on ones which we were stuck on. We ate together and, honestly, had a great time. 

I will admit that my contributions to the team were minor in this event. As a beginner who had only just started studying computer science, I rarely had any novel insights and more so learned from the older students.
Despite this, the event motivated me to stick with the cybersecurity club and join them in occasional CTFs from then on, some of which I will have noted here on my site.

We ended up placing 5th. A stellar rank considering 1000 participating universities, but disappointing for the older members, as they had placed 1st the year before (though we would redeem ourselves with 1st place in the following year).

For me, this event was just the start of my ventures into cybersecurity. Right away I used the free year of HackTheBox VIP I had won as a member of the 5th-place team to complete some beginner courses on the platform about SQL injections, XSS and the like.

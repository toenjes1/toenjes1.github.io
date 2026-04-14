---
title: Cybersecurity in Practice
date: 2025-03-05
tags: [cybersec, uni]
toc: false
comments: false
---

One of the most distinctive courses I chose during my degree was Cybersecurity in Practice. As the name suggests, the course placed a strong emphasis on hands-on work, complemented by a well-structured lecture series that introduced a broad range of foundational security concepts. Early topics included networking fundamentals such as the TCP/IP stack, classifications of threat actors and attack types, and the core security objectives (often summarised as confidentiality, integrity and availability). From there, the course progressed into more specialised areas, including reconnaissance techniques, operating system security and sandboxing, authentication and authorisation, application security, cryptography, network security, and principles of secure software development and distribution.

The practical components of the course were organised around the extensive "_network scenario_". 

Initially came some setup tasks such as configuring and familiarising ourselves with Kali Linux, setting up some network connections and so on. After we had completed these, we were given access to a massive custom-built network maintained by the teaching team. This environment consisted of over forty different machines, each with distinct configurations and behaviours. Also consider that a separate instance of this network had to be maintained for every single student with routing based on our authentication with the network and so on, such that every individual had the full range of experimentation.

Our task throughout the semester was to systematically explore this network: performing scans to identify hosts, mapping the network topology, and investigating each system for vulnerabilities to be exploited.

![Desktop View](/media/cip/network_plan.png){: width="972" height="589" }
_A part of the network plan_

The vulnerabilities varied greatly, including injection flaws, misconfigurations, cross-site scripting, spoofing techniques, and more complex interactions between multiple systems. Once identified, these weaknesses could be exploited to retrieve hidden pieces of data, which served as proof of successful attacks and contributed to the overall assignment. This structure created a continuous, investigative workflow. I imagine it resembled real-world penetration testing scenarios, at least in some ways. Either way, it was assuredly a genuine test of skill as well as perseverance. 

Among the exploits I successfully ran on the targets were the following:
- Sending base64-encoded reverse shells through template injection
- Uploading malware to an online image analyser with a title that executes itself due to poor sanitisation
- Breaking out of Docker containers via mounting points
- Reverse engineering C binaries
- Uploading an XSS post to a forum where an automated administrator bot reads the posts every minute 
- Using a misconfigured dokuwiki installation to execute code on the server and escalate privileges
and many more.

The course concluded with a one-hour oral examination, but the primary challenge was definitely in the sustained practical effort required over the whole semester. Cybersecurity in Practice is infamous within my programme as one of the most demanding modules, both in scope and time commitment. As the teaching team had not set up a VPN into the network initially, we had to be present at specific ports to attempt these challenges for a good chunk of the semester. And, frankly, the VPN's connection speed did also struggle later on. This meant long evenings on campus, staying until 11 pm, when I was forced to stop, as this is the university building's closing time. Despite this, the experience was outstanding---and so was the lecture. Alongside [operating systems 2](/posts/Styrikerfi), it remains one of my favourite courses.

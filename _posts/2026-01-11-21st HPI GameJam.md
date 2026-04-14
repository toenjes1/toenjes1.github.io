---
title: I won the 21st HPI GameJam
description: Yet another game :)
date: 2026-01-11
tags: [gamedev, godot, gdscript, contest]
toc: false
comments: false
image:
    path: /media/21st_gamejam/dino_mainmenu.png
    alt: our game's main menu screen
---

An amazing fusion of pirates, dinosaurs, and cocaine! Find your rhythm and defeat the sea monster before it consumes all your amphetamines! 

This is what our third installation in the HPI GameJam participation series is all about. 

D.I.N.O. stands for "Dinosaurs, Instruments, Narcotics and the Octopus", and it fully captures the spirit of our game.

For the 21st HPI GameJam---my third one---, we formed a six-person team, up 50% from our previous four-person teams. We 1.5x'ed in size because we knew that this year we had to go bigger and better! The theme this time: "historically accurate". A prompt, which tempted many---us included---to an ironic play on gravely inaccurate historical depictions. Our depiction of choice? Pirate dinosaurs, smuggling cocaine. 

Getting six people on board with an idea turned out to be quite a bit more challenging than convincing just four. Our deliberation session definitely exceeded the three hours we spent during the [18th HPI GameJam](/posts/18th-HPI-GameJam). We eventually settled on, admittedly, a relative simple core gameplay mechanic: a rhythm game. Rhythm games are a fairly popular genre of video games with popular games on various platforms, including Beat Saber, Guitar Hero, Piano Tiles, Osu!, Geometry Dash, Hi-Fi Rush, and many more. Now came our entry in this genre. 

To merge our desired rhythm mechanic with the premise of dinosaur pirates, we contrived an evil octopus who wants to steal the cocaine being smuggled. He attacks the pirate ship with his tentacles, and the pirate dinosaurs have to play their _instruments_ to fire the ship's cannons!

Development went great. With six people, we actually had more than one person working on art. As it is a hard requirement for a rhythm game, we even had sound (a first for me during GameJams), including self-composed tracks in levels 3 and 4! Personally, I spent all of my weekend in the Godot engine. Mostly writing code, but also making some simple animations and shaders. In general, we were quite focused on polish, such as animations, transitions, multiple scenes and some sound effects. We ended up creating four levels with increasing difficulty (the first level being a tutorial to introduce the controls---something I've also never achieved before at a GameJam).

I had a phenomenal time. Again, I found that setting your mind to a goal and just focusing on it is incredibly rewarding. In the corresponding post, I mentioned how we had created some unnecessary overhead during the 18th HPI GameJam by developing on feature branches. It turns out that, for a GameJam, such "good practice" is indeed out of place. Even six people constantly pushing to main during this weekend (207 commits in two days) went just fine. Sadly, my teammate who created this repository set it to private, so I will not be able to showcase the source. However, the game does have a page on [Itch.io](https://storyxx.itch.io/the-dino-is-a-part-timer) where you can play the game right inside your browser. The loading times are much shorter compared to our web export at the 20th GameJam. :)\
Also check out the rest of the games on [the event page](https://itch.io/jam/hpi-gamedev-klub-jam-21)!

Here is me playing through the second level without skipping any cutscenes:
{%
  include embed/video.html
  src='/media/21st_gamejam/dino_lvl2.mp4'
  types='ogg|mov'
  title='This is what a full level looks like, including our opening and closing scenes'
  autoplay=false
  loop=false
  muted=false
%}

I noticed that I have not really described the final rating process, so I will do it now. After the development deadline around 6 pm on Sunday (after 48 h of development), every team first presents their game in front of all attendees. Then follows the play testing round. Every team sets up their game at one station, and all attendees go around and try out everyone else's game. Afterwards, each team gets to rank all other teams in all categories, some of which are entertainment value, artistic presentation and originality. Lastly, the rankings are tallied, and the team with the best sum of rankings wins.

Some considerations can be made regarding which _kinds_ of a game's strengths shine brightest here. A *functional* and *immediately engaging* gameplay mechanic paired with a strong *art style* is, I would say, most important. What is not so important includes complexity/depth, amount of content, story, replayability, message, etc. Simply put: the players only engage with your game for a maximum of, let's say, ten minutes. Sometimes, just a minute or two. This is all the time you get to convince them. We noticed this during the [20th HPI GameJam](/posts/20th-HPI-GameJam) where we created a relatively complex and original game. This led to our game being error-prone and presenting a high barrier of entry; players first had to learn the rules of the card game. In contrast, we made this weekend's game much more simple and palpable. Press the button when the tentacle lights up. And by saying this, I do not mean to discredit GameJam games at all. Simple, fun games totally have their place in gaming. One only has to be aware of the target audience (given a high rating is even what one is competing for). 

And so we won. It appears our aim to create an engaging game worked out. In fact, I was very pleased when one of the attendees attempted our second level a couple of times, said he'd only give it one more shot, and then proceeded to spend maybe another ten attempts until he finally beat it. That is exactly the type of behaviour you wish to see in your players.

For some more exciting gameplay: level four
{%
  include embed/video.html
  src='/media/21st_gamejam/dino_lvl4.mp4'
  types='ogg|mov'
  title='Me attempting a more challenging level, you can hear the fail sounds due to me missing the timing 😅'
  autoplay=false
  loop=false
  muted=false
%}

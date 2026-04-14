---
title: Second place at the 20th HPI GameJam
description: I made a game again
date: 2025-04-27
tags: [gamedev, godot, gdscript, contest]
toc: false
comments: false
image:
    path: /media/20th_gamejam/erit_mainmenu.png
    alt: our games' main menu
---

After the [18th HPI GameJam](/posts/18th-HPI-GameJam), we came back for seconds. As mentioned there, a GameJam is all about creating a video game in a strictly limited amount of time.

This time around, two of my teammates had already set their mind on creating a card game. When the theme, _time travel_, was announced then, it was mainly a matter of incorporating the theme into a card game of some sort. As far as I can tell, the reason for their conviction was their obsession with the game Balatro.

![Desktop View](/media/20th_gamejam/erit_ingame.png){: width="972" height="589" .w-50 .right}
First, we came up with an original card game concept on paper. We then transferred the concept to a video game that can be played with only mouse clicks and drags, technically making it mobile-friendly. Having done so, we considered how to integrate the time travel theme into our card game. This approach was quite different to our previous participation where we mostly constructed our idea from the theme onwards, rather than adding the theme onto the idea.

We settled on the following. The AI opponent of the player was to be run by a very competent algorithm and possibly even have in-game advantages, such as better cards or more HP. The player should instead have access to time travelling abilities, which would allow gaining special insights about the state of the game, such as predicting the next card to be drawn, predicting the opponent's next card or even turning back time a couple turns. In essence, the player was supposed to abuse time travelling abilities to compensate for the opponent's dominant gameplay. Thus, the plan is laid out for our game "Erit".

We made these graphics to explain the game:

![Desktop View](/media/20th_gamejam/erit_1.png){: width="380" .normal}
![Desktop View](/media/20th_gamejam/erit_2.png){: width="380" .normal}
![Desktop View](/media/20th_gamejam/erit_3.png){: width="380" .normal}
![Desktop View](/media/20th_gamejam/erit_4.png){: width="380" .normal}

Similarly to last time, we banished one of our team members (the same one, to be precise) to the art department. All three others did development.

We started by implementing card dragging, hand cards and a card table. Then we went on to make the rules of the game, HP for the player and computer, the rounds and the win/loss conditions of the game. During the two days of development, we started noticing that our initial plans were rather optimistic. The time travelling abilities, especially the one which was supposed to allow going back in time, were challenging to get right at this point.

![Desktop View](/media/20th_gamejam/erit_gameplay.png){: width="972" height="589" }
_Playing a reverse card onto a losing lane such that the nine points of damage go to the opponent instead_

Sadly, our game ended up quite buggy and not really complete. Incomplete and even unstable games are very common at GameJam, but still, the result was slightly disappointing. Especially since our idea was going in a great direction. 

Due to this and perhaps not getting across the complexity that a challenging card game requires, we only came in second this time around. It was especially sad since the winner actually got to showcase their game at gamescom---the largest gaming event in the world.

The game can be played in the browser on our [Itch page](https://saraqael-m.itch.io/erit).
But beware of the extremely long loading times of Godot's web export for this game.
Additionally, the source code is public on [GitHub](https://github.com/toenjes1/gamejam2025).
Check out the [other games](https://itch.io/jam/hpi-gamedev-klub-jam-20) of the GameJam as well!

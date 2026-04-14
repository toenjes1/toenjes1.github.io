---
title: I won the 18th HPI GameJam
description: Making of a game
date: 2024-05-26
tags: [gamedev, godot, gdscript, contest]
toc: true
comments: false
image:
    path: /media/18th_gamejam/annis_hilation.png
    alt: our game's main menu screen
---

## Lead-up
When I saw the announcement of the 18th HPI GameJam---a university internal GameJam organised by the game development student club every semester--- in my inbox, I immediately set out to assemble a small squad for participation.
As many programmers who play video games, I've thought about making one myself. So I took this opportunity to dabble in game development.

Three friends and I thus signed up for the GameJam, which, in case you don't know, is a type of competition in which the organisers announce a theme at the start, and then all competing teams make a related game in a very limited amount of time. This GameJam lasted only one weekend; larger ones might also last a week or so. Either way, very little time for a video game. That, however, is part of the experience and fun. Especially a weekend-long GameJam lends itself to devoting every waking minute to the game (and temporarily minimising the non-waking minutes), keeping up focus on the objective at all moments of a day, and spending a whole weekend doing one thing and one thing only. This is something that I found out I enjoy quite a lot. I believe I slept for a total of 5 h during that weekend, which is obviously not sustainable for long but lends itself quite well to this sort of competition.

My team and I decided on using the Godot game engine a couple of days before the event. Mainly, so that we could familiarise ourselves with a shared development environment before the strict time limit of the competition commenced. So I followed by some YouTube tutorials and made my first game in Godot the night before the event. 

## The event

The GameJam started with the reveal of the theme and scoring categories. The theme turned out to be "_Architects of Annihilation_", which, frankly, is quite broad. But seeing all the teams' takes on an interpretable theme is also part of the fun. Additionally, it was said that the games should be _couch co-op_, meaning that players could cooperate on a locally shared device. How well a game achieved this style of playing also became one of the scoring categories, alongside gameplay entertainment value, visual interest, and originality (sort of the classics).

### Conjuring a plan

And then came the brainstorming session. Naturally, the first step of the process must be to conjure up an idea. I believe that this is also the most important step of the process. You have to consider, of course, the theme and scoring categories. And as with most projects, you have to gauge the skills of your team and your time and resources as well as your target audience. It is important not to set your goal too high or too low, to make it appropriate for the upcoming playtesting session. The core idea and specialities of the game have to reveal themselves naturally and quickly to a novice player such that, at the end, the other teams (all teams score each other) understand the vision.

All of that is to say that there is actually quite a lot of thought that can go into even a two-day development project like this one.

As brainstorming goes, my teammates and I collected a great many ideas. We ended up converging towards a 2D top-down action game in which two cooperating players could simultaneously control two separate characters and fend off hordes of attackers. It is straightforward to then map both sets of controls onto one keyboard or allow for two connected controllers to achieve that desired local multiplayer experience. In and of itself this is all a fairly typical setup for a video game. That is why we wanted to add some sort of twist, an original flavour to our game.

### The idea
Finally, we came up with the following: one of the characters was the main fighting entity. He would fend off the opponents by swinging his arms at them. When getting hit, however, he was in danger of losing his limbs. Enemies could take off his arms and legs when he did not manage to combat them. Losing limbs impedes this character's ability to fight (as one might expect): losing arms meant fewer attacking opportunities, and losing legs meant decreased movement speed. 

The other character then had the capability to reattach those limbs by picking them up off the ground and taking them to the stump of the body. She only had weak defensive capabilities of her own, and if she got hit, it would actually take HP off a shared health bar. 

So in summary, there are two distinct roles. And they have to cooperate uniquely to succeed.

We then also spun a simple story around this mechanic where she is a scientist who created this larger being (think Frankenstein's monster, clearly). He can protect her physically, and she can repair his damaged body. The annihilation theme then... well, they together annihilated the enemies. Or they had set out to annihilate the characters. And she is the "architect" of her creature, right? Oh, well. Either way, we named the scientist Anni and her creation Hilation so that we could call it: "Anni's Hilation". Theme clearly fulfilled, don't you think?

With our goal in place, we broke the task down into a list of To-dos which we placed as sticky notes on a Kanban-style board. Very standard practice for a reason. We also designated roles: most notably, one of our members was assigned to visuals exclusively while the other three of us would handle development. Development in turn was categorised into the playable characters, enemies/enemy spawning and so on.

All of this took around 3 hours off our 48-hour time frame. Time very well spent!

### Development and the game
With roles and To-dos in place, the development process in such an event is quite standard, albeit highly accelerated. Some priorities do also shift: features are much more important than maintainability, legibility in code, performance, style guidelines, design patterns, or any of such irrelevant crap.

Godot is an intuitive environment, and while GDScript will not become my favourite, it easily suffices for this task. One organisational decision we did make was to work on feature branches on Git. Arguably, since development periods were so, so short, and we all sat in a room together, coordinating pushes to main would've been possible as well. Possibly more efficient. We did deal with some merge conflicts, partially due to a lacklustre .gitignore for Godot projects (GitHub has a template; should've maybe used it).

Our repository is public and can be found [here](https://github.com/MaximStanko/UntitledAnniHilationGame) in case you're curious about the code.

Throughout development, decisions have to be made. Sometimes due to missing details in the plan, sometimes due to new realisations regarding implementation complexity or time running out, etc. In a team of four with no other stakeholders involved, the decision-making overhead is very small. Thus, the game takes shape while being created. In a way, you can imagine it like rapid prototyping or agile development, except even faster. 

We landed on spawning our enemies in waves from fixed locations. One wave of enemies had to be defeated before the next one spawned, and waves became increasingly difficult. We made three enemy types which were introduced as the players progressed.

The final game's main page is on [itch.io](https://saraqael-m.itch.io/annis-hilation). You can play it right now on Windows; we provide a fully functional download. The controls using controllers are on the itch.io page.

![Desktop View](/media/18th_gamejam/annis_hilation_ingame.png){: width="972" height="589" }
_Screenshot of an early moment within the game: Anni is holding a limb and bringing it back while bats are attacking_

The setting is a graveyard since this is where Anni sourced the biological components for her creation.

### Scoring
We won :)

By quite a margin, actually. Our unified pixel art-look crushed the art style category, and we also met the consensus on "couch co-op" mechanics spot on.
Some of the other games are found on the [event's itch page](https://itch.io/jam/hpi-gamedev-klub-jam-18).

## Finishing thoughts
Whenever such an event ends, exhaustion naturally sets in. 48h of concentrated work on little sleep and nutrition expectedly has this effect. The immediate reaction after such a crunch is: "never again". However, after recovering from my mortal needs, I am satisfied. Not just due to our great placement, but---perhaps more importantly--- due to the gratification of achieving. Setting your mind to a goal and dedicating time to it, even if it is only a weekend, feels accomplishing after all.

We all agreed that we would, time permitting, be back soon.

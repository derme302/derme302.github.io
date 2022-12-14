---
title: "Fixing the Bubble Shooter experience on mobile"
date: 2022-12-14T17:30:00+10:00
categories:
  - GameMaker
  - Games
tags:
  - gamedev
---

There's a serious problem in a very niche game genre on Google Play. It seems like every bubble shooter on the store is designed to take your money and steal your data, which doesn't seem right when it's based on the 1994 hit Puzzle Bobble by Taito.

I've recently launched my brand new game [Just Bubbles](https://frostcube.com/post/just-bubbles/), but before we launched Just Bubbles I wanted to make sure that it stood apart from the marketplace. Most of the games currently available are visually appealing but more in a distracting sort of way like a slot machine. Just Bubbles wasn't designed to grab your attention and make a quick buck off ads it was designed to be an enjoyable and relaxed experience. As you can you see most of the games currently depend on advertising revenue or in the worse case, creating an environment where you have to spend money to progress. These games are creating a false preposition of value, they are design to make you think spending money is worthwhile instead of what they should be doing of creating a experience worth paying for.

As you can see from the table below, even when they aren't taking your money they are mining you for data, mainly to share with 3rd parties.

| Game Name                                                                                                                 | Free to Play?      | No Ads?                       | No in app purchases?          | Doesn't collect data?         | Doesn't share data with 3rd parties? |
| ------------------------------------------------------------------------------------------------------------------------- | ------------------ | ----------------------------- | ----------------------------- | ----------------------------- | ------------------------------------ |
| [Just Bubbles](https://play.google.com/store/apps/details?id=com.frostcube.justbubbles)                                   | :white_check_mark: | :white_check_mark:            | :white_check_mark:            | :white_check_mark:            | :white_check_mark:                   |
| [Bubble Shooter](https://play.google.com/store/apps/details?id=bubbleshooter.orig)                                        | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :white_check_mark:            | :negative_squared_cross_mark:        |
| [Bubble Shooter Kingdom](https://play.google.com/store/apps/details?id=com.bigcool.puzzle.bubbleshooterkingdom)           | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Shooter Royal Pop](https://play.google.com/store/apps/details?id=linkdesks.bubblegames.bubbleshooter.royal.pop)   | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :white_check_mark:                   |
| [Bubble Shooter Viking Pop](https://play.google.com/store/apps/details?id=linkdesks.pop.bubblegames.bubbleshooter)        | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Shooter 2022](https://play.google.com/store/apps/details?id=com.oneup.ball.shooting.blast.free)                   | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :white_check_mark:            | :white_check_mark:                   |
| [Bubble Shooter: Bubble Games](https://play.google.com/store/apps/details?id=com.matching.bubble.pop.bubble.shooter)      | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Witch 3 Saga](https://play.google.com/store/apps/details?id=com.king.bubblewitch3)                                | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Shooter Rainbow](https://play.google.com/store/apps/details?id=com.blackout.bubble)                               | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Shooter Legend](https://play.google.com/store/apps/details?id=com.linkdesks.iBubble)                              | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Shooter: Panda Pop!](https://play.google.com/store/apps/details?id=com.sgn.pandapop.gp)                           | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Witch 2 Saga](https://play.google.com/store/apps/details?id=com.midasplayer.apps.bubblewitchsaga2)                | :white_check_mark: | :white_check_mark:            | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :white_check_mark:                   |
| [Primitive Shooter](https://play.google.com/store/apps/details?id=game.bubble.shooter.dragon.pop)                         | :white_check_mark: | :negative_squared_cross_mark: | :white_check_mark:            | :negative_squared_cross_mark: | :white_check_mark:                   |
| [Angry Birds POP Bubble Shooter](https://play.google.com/store/apps/details?id=com.rovio.ABstellapop)                     | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Shooter 2](https://play.google.com/store/apps/details?id=shooter.two.purple)                                      | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Inside Out Thought Bubbles](https://play.google.com/store/apps/details?id=com.disney.thoughtbubbles_goo)                 | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :white_check_mark:                   |
| [Bubble Shooter Genies](https://play.google.com/store/apps/details?id=com.linkdesks.bubblegames.bubbleshooter)            | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Simon’s Cat - Pop Time](https://play.google.com/store/apps/details?id=com.strawdogstudios.simonscatpoptime)              | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Shooter! Extreme](https://play.google.com/store/apps/details?id=bubble.shooter.exxtreme)                          | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Bubble Shooter - Snoopy POP!](https://play.google.com/store/apps/details?id=com.jamcity.snoopypop)                       | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |
| [Smurfs Bubble Shooter Story](https://play.google.com/store/apps/details?id=com.sonypicturestelevision.smurfslostvillage) | :white_check_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark: | :negative_squared_cross_mark:        |

I will give a shout to Primitive Shooter, which is a pretty close second to Just Bubbles, but still has ads. For focused Bubble Shooter experience you can [download Just Bubbles now](https://frostcube.com/post/just-bubbles/).

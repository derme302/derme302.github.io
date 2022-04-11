---
id: 26
title: 'GameMaker: ThreeJS Extension Demo!'
date: 2013-05-15T05:20:00+00:00
author: Derme
layout: post
guid: http://derme.coffee/2013/gamemaker-threejs-extension-demo/
permalink: /2013/05/gamemaker-threejs-extension-demo/
image: /uploads/2013/05/Screen-Shot-2013-05-10-at-10.29.09-PM-624x464.png
categories:
  - GameMaker
---
Those of you that [follow me on Twitter](https://twitter.com/Derme302) will know that I've spent the last week working on integrating the ThreeJS (r58) library with GameMaker: Studio. Now if you are already bursting with excitement you can skip to the end of the post for a link to the working demo!

![ThreeJS Demo](/uploads/2013/05/Screen-Shot-2013-05-10-at-10.29.09-PM-300x223.png#center)

The most awesome thing about this extension is that you can still do all your input control, AI and GUI though the GameMaker canvas. I've done this by using the CSS attribute z-order to &#8220;stack&#8221; the GameMaker canvas over the WebGL Renderer, I'm not sure this is the most conventional way to achieve this but it was easy to implement and seems to work fine.

![Canvas Stack](/uploads/2013/05/blog_example-300x271.png#center)

At the moment you can draw cubes, spheres and create lights however I plan to extend the extension over the coming months to allow custom models (.obj) to be used and textures. This is going to take a bit longer as I don't have a huge amout of free time at the moment, so I decided to release it as-is and as the extension isn't minified you can tweek it untill your heart is content or I release a update.

At the moment the following functions have been integrated, you'll notice that some of them still aren't complete. e.g. Lights don't have a id yet so they can't be deleted which I plan to add at a later stage, once I work out a solution to clearing scenes without creating memory leaks.

![Code Example](/uploads/2013/05/Screen-Shot-2013-05-10-at-10.59.39-PM-300x143.png#center)

Finally my personal favourite the ability to still be able to use GameMaker's room editor for level design, here is what the current demo level looks like:

![Editor Level](/uploads/2013/05/Screen-Shot-2013-05-10-at-11.02.07-PM-300x157.png#center)

That about wraps up everything, so how about trying out the demo? (Requires: Google Chrome)

**Update 11/4/2022:** The demo example was broken a long time ago, but you can find the source code for Game Maker Studio 2 on [GitHub](https://github.com/derme302/gms-j3d/tree/dev/gms2)

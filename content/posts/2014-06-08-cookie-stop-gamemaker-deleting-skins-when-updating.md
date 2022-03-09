---
id: 136
title: 'Cookie - Stop GameMaker deleting skins when updating'
date: 2014-06-08T08:30:01+00:00
author: Derme
layout: post
guid: http://derme.coffee/?p=136
permalink: /2014/06/cookie-stop-gamemaker-deleting-skins-when-updating/
image: /uploads/2014/06/banner_image-624x159.png
categories:
  - GameMaker
tags:
  - guide
---
GameMaker's auto-updater has its issues, but deleting your customs skins shouldn't be one of them.

One of GameMaker's hidden features is that it has two folders on your computer. The first folder stores the main program that gets overwritten when you update. The second folder is where you can keep all your skins, tutorials, extensions and DnD libraries safe from the evil auto-muncher.

So the folder where the main components of the IDE are is located at  

```
C:\Users\<Username>\AppData\Roaming\GameMaker-Studio
```

Don't store anything here, it won't survive. The place you should put it instead is:  

```
C:\Users\<Username>\AppData\Local\GameMaker-Studio
```

Which will save you from ever having to worry about it disappearing again!
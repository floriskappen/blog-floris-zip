---
title: Creating a game without an engine
author: Floris
featured: false
draft: false
tags:
  - game-development
pubDatetime: 2021-04-15T20:47:52.756Z
ogImage: ""
description: When I wanted to create my first game, I only had a background in web development. I wanted to create a game in Javascript, so I chose Phaser for my first project.
---

_Worked on it from 14 Jan 2020 to 19 Feb 2020 during school_

# Creating a game without an engine

When I wanted to create my first game, I only had a background in web development. I wanted to create a game in Javascript, so I chose [Phaser](https://phaser.io/) for my first project, which is a game **framework**, not an **engine**. Which means you don't have a UI where you can click some scenes together and import your assets by dragging and dropping them.

## Table of contents

## First impressions

It took some getting used to the framework, but the documentation was decent once I understood how to navigate it. I really enjoyed the fact that I am scripting every part of the game, instead of using all types of prebuilt objects like I would have in [Unity](https://unity.com/).

It really felt like I was building things from scratch, even though Phaser already included nearly everything I needed, like Physics and scene management. For a first-timer it was a cool experience to say the least. Phaser also has a lot of examples for all the features it includes so it was really easy to find code snippets for specific features I wanted to use.

### Organisation issues

As the project got bigger it kept getting harder and harder to keep everything organized. I had a lot of assets to import and assign UID's to so the files where that happened were getting extremely big. I think there are probably really nice ways to keep everything organized that I didn't know about though.

This is a file where I kept track of all the UID's in the game. You need a unique string for almost everything from images to individual animations... so that's why it's so huge even though the game isn't super big yet.

![CST](https://i.postimg.cc/9Xg8QwYx/vof9-FW3-Skr.gif)

## The game idea

My idea was to basically build a smash clone. It was for fun and to learn so I didn't really think about how viable my idea would be if I were to actually put the game out there. I just wanted to create something I would enjoy, and that was within my reach.

You would select a gamemode, then a character and a stage. The objective was to brawl it out on the stage, knocking the oponent to the side until they are out of the camera's view, at which point they would loose a life and respawn in the middle of the stage.

## I'm not an artist

I decided to go for a pixel art style, because I though it would be easiest for me to create. But I ran into a problem I still haven't figured out a solution for in 2021... which is that I really enjoy writing code and designing the game, but I don't really enjoy creating art for it.

I created the first stage which I'm quite proud of though.

![stage-1](https://i.imgur.com/tsBy7fl.png)

I also created some dash effects, but the rest of the assets are all from [OpenGameArt](https://opengameart.org/) or from some people from my school that I asked for help.

As I said I still struggle with that problem as of writing this in 2021, where I depend too much on artists to create a game. I should definetly consider my inability to create art way more when thinking of a game idea...

## Some cool features

Enough talking, let's look at some of the cool parts of this project.

### Menu's & controller support

![menus](https://i.postimg.cc/PxrgBsdN/LGo-Ax1q0-MY.gif)

The menu's were definetly not finished, but considering how brutally difficult it was to create them in Phaser I'm pretty happy with the flow. There are also some little animations which make it all feel better.

I also added controller support, through which 2 players could play together. On the top right you can see an icon of a keyboard. If you plug in a controller and press a button you will see a controller icon appear, which would automatically become Player 2.

### Movement & abilities

![movement](https://i.postimg.cc/ZK2yn4gt/hnq-P7-Zd-Tt-X.gif)

The main highlight is obviously the gameplay, which I'm also quite happy with. Code-wise I thought I had a pretty nice approach, where there was one base character class which contained all kinds of actions, like "side light attack", which could then be handled in child classes inheriting from that parent class.

The camera movement also worked pretty nicely I think, and the screenshake and pixel art effects really add to it.

You have abilities in this game, and after you use one you will see it's icon slowly fade out. While it's fading out it's on cooldown.

If you hit an enemy, you also see their abilities for a short time. I don't remember why I chose to do this, but it probably just looked cool.

## Conclusion

Cool first project that I sadly stopped working on as I didn't find the right artists which killed my motivation. I was getting to a stage where art was really important but I just couldn't find anyone that wanted to put in the time to create all the assets, which I totally understand.

I still think the end result is pretty cool for the time I put into it, and it definetly opened my eyes to how fun game development can be.

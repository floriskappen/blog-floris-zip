---
title: creating a game without an engine
author: Floris
featured: false
draft: false
tags:
  - game-development
pubDatetime: 2021-04-15T20:47:52.756Z
ogImage: ""
description: i tried to recreate smash bros in javascript using phaser - with pixel art, controller support, hit effects, and way too much code in one file.
---

_worked on it from 14 jan 2020 to 19 feb 2020 during school_

# creating a game without an engine

when i wanted to create my first game, my background was mainly web development. since i wanted to make a game in javascript, i picked [phaser](https://phaser.io/) for my first project, which is a game **framework**, not an **engine**. this means it doesn't have a ui where you can just click scenes together and drag-and-drop your assets.

## first impressions

phaser took some getting used to, but the documentation was pretty solid once i figured out how to navigate it. i really enjoyed scripting every part of the game myself, instead of relying on prebuilt objects like i would’ve had to do with [unity](https://unity.com/).

it genuinely felt like i was building something from scratch, even though phaser already included almost everything i needed, like physics and scene management. for someone new to game development, this was a super cool experience. phaser also has plenty of examples for all its features, making it really easy to find snippets of code whenever i needed something specific.

### organisation issues

as the project grew, it became harder and harder to keep everything organized. i had lots of assets to import and had to assign unique ids (uids) to each one, making the files handling this part really messy and huge. i'm sure there were probably better ways to organize it all that i simply didn't know about at the time.

here’s an example file where i kept track of all the uids. nearly everything -- from images to individual animations -- needed a unique string identifier. that's why the file became so enormous even though the game itself wasn't super big yet.

![CST](https://i.imgur.com/8imNQS1.gif)

## the game idea

my idea was essentially a smash bros clone. it was purely for fun and learning, so i didn't really think about whether it would be viable as a public release. i just wanted to create something enjoyable and within my abilities.

you'd pick a game mode, select a character and a stage, and then fight on that stage by knocking your opponent sideways until they're out of camera view. once knocked out, they'd lose a life and respawn at the center of the stage.

## i'm not an artist

i decided on a pixel-art style since i thought it would be easiest for me. but this is where i hit a problem -- one i still hadn't solved by 2021 -- which is that while i really enjoy coding and designing games, i don't enjoy creating art at all.

still, i managed to make the first stage myself, which i'm quite proud of.

![stage-1](https://i.imgur.com/tsBy7fl.png)

i also made some dash effects, but almost all the other assets were from [opengameart](https://opengameart.org/) or made by friends from school whom i asked for help.

this issue was still troubling me when writing this in 2021 -- i remained too reliant on artists to finish a game. in the future, i should definitely consider my lack of art skills more carefully when choosing a game idea.

## some cool features

enough talking -- let's take a look at some of the cooler parts of this project.

### menus & controller support

![menus](https://i.imgur.com/3cyIfjP.gif)

the menus weren't completely finished, but considering how brutally hard it was to create them in phaser, i'm pretty happy with how they turned out. i even added some little animations that made everything feel smoother.

i also built controller support so two players could play together. in the top right corner, there's an icon showing a keyboard. when a controller is plugged in and you press a button, a controller icon appears, automatically assigning that controller to player 2.

### movement & abilities

![movement](https://i.imgur.com/jtWBQKr.gif)

the highlight was obviously the gameplay itself, which i'm pretty satisfied with. from a coding standpoint, i had a neat approach: a single base character class handled generic actions like "side light attack," and then child classes could inherit and modify these actions individually.

i also liked how the camera movements worked, and the screenshake and pixel-art effects really added to the feeling.

characters had abilities, and after using one, its icon would fade out, indicating a cooldown. additionally, hitting an enemy briefly showed their abilities. i don't exactly remember why i added this -- it probably just looked cool.

## conclusion

it was a cool first project, but sadly i stopped working on it when i couldn't find suitable artists, killing my motivation. at the point i stopped, art was becoming increasingly important, but i just couldn't find anyone who wanted to spend the time creating all the necessary assets -- which i completely understand.

overall, i still think the final result was pretty cool for the time and effort i put in, and it definitely opened my eyes to how much fun game development can be.

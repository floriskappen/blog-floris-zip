---
title: Whiteboard app
author: Floris
featured: false
draft: false
tags:
  - web-devevelopment
pubDatetime: 2021-04-15T20:47:52.756Z
ogImage: ""
description: In January of 2020 I worked on what could have been Miro! Just kidding... The idea was very similar though.
---

# Whiteboard App

In January of 2020 I worked on what might have been Miro. Just kidding!

## Table of contents

## Introduction

It all started when I found the [Paper.js](http://paperjs.org/) library. I thought it looked very cool and really wanted to build something with it. To be honest, it provided nearly everything I needed for my app. All the data types were present, and I just had to make use of them to create the app I wanted.

At this point I had just gotten the hang of [VueJS](https://vuejs.org/), which I noticed because of the fact that the bulk of the app is inside of one big .vue file. If I remember correctly I was planning on splitting it up into different components, but I should have just done that from the start.

## The idea

The plan was to create a whiteboard app, where you can create your own room that stays alive for 24 hours, and generate a shareable link which you can send to other people so you can collaborate.

I originally planned to use [Websockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) to make the connection possible, but the entire backend of the app never came to fruition.

I did however create some awesome tools in the front-end, which you can see here.

![collabza_tools](https://i.imgur.com/mfa1woz.gif)

## Downsides of vectors

I wanted to create some cool pencil tools, and maybe even brushes. But since [Paper.js](http://paperjs.org/) is vector based, anything you draw is made out of points. To save on performance, these points are created sparingly with [Bézier curves](https://en.wikipedia.org/wiki/B%C3%A9zier_curve) to make everything seem smooth. This is awesome, but the downside is that when you draw or erase things, it's not smooth like it would be in a program like photoshop. You can see what I mean here.

<util-aligner center>

![collabza_erase](https://i.imgur.com/e9P2Gs0.gif)

</util-aligner>

## Layer system

Another feature I'm quite proud of is the layer system. I store every object in layers, which works just the way you would expect it to coming from programs like photoshop. I guess in hindsight this feature is very useful for creating more complex works instead of the more simple and temporary ones you would expect from a whiteboard app, but I still think it's a really cool feature.

I also group objects by their type. So you have objects created with the drawing tool, or the shape tool. I planned on adding text and image support, but I stopped working on the app before I could implement those.

![collabza_layers](https://i.imgur.com/KgoAx3C.gif)

## Conclusion

This was a cool project that helped me better understand how [VueJS](https://vuejs.org/) worked. I could have expanded on it quite a lot, but I think the direction I had in mind, which was a drawing program like [Aggie.io](https://aggie.io/) just would not have worked out. I am still very pleased with the design, though!
You can [check the code here.](https://github.com/floriskappen/collabza-app)

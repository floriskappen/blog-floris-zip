---
title: creating a platform for my minigames
author: Floris
featured: false
draft: false
tags:
  - game-development
pubDatetime: 2022-02-20T20:47:52.756Z
ogImage: ""
description: i built a godot-powered platform to host tiny games with accounts, highscores, and a custom backend in fastapi - because one game wasn’t enough.
---

_this blog post is a more technical text version of [the video about this project](https://www.youtube.com/watch?v=YH4vsr9XJ8s&)._

for my content creation idea, i planned to build several minigames. since each game would be relatively small, i didn't want to publish each one separately. instead, i decided to build a single platform that i could update whenever a new minigame was released.

### planned features

the features i wanted to include were:

- account management
  - account registration
  - login functionality
  - update account details
  - password reset (receiving an email with a reset code)
  - authenticated requests with session tokens
  - automatic login using session tokens
- highscore submissions (for logged-in users)
- viewing top scores per minigame

### the tech stack

the minigames themselves would be built with [godot 4.0](https://godotengine.org/), which was still in pre-alpha at the time. from a web-development perspective, the godot games would act as the front-end.

for the backend (server), i chose python. godot's scripting language is heavily inspired by python, and i prefer using the same language across a project whenever possible. it helps prevent confusion from constantly switching between different languages.

at my [current job at the time of writing](https://brainial.com/), we use python for the backend and react (js) for the frontend. this occasionally leads me to defining functions incorrectly because i accidentally use syntax from the wrong language when working full-stack.

for this backend, i used [fastapi](https://fastapi.tiangolo.com/), a python framework i really enjoy. as for the database, i picked [postgresql](https://www.postgresql.org/).

### my experience with godot 4.0 pre-alpha

this project was actually made using nightly builds of godot 4.0, just before the first official pre-alpha was released.

i already had a decent amount of experience with godot 3.x. once, i participated in a weekly game jam and created [orbing around](https://kadeflo.itch.io/orbing-around). i've also started a few unfinished projects. one of those had many ui elements, so i was already familiar with building uis in godot. luckily, the ui nodes didn't change much between versions, so transitioning to godot 4.0 was pretty smooth for me.

i could implement most of my design ideas easily, except for gradients with rounded corners. i planned to use shaders as a workaround, but shaders for 2d nodes were pretty broken at the time. apart from this and a few random engine crashes, things went smoothly.

### api calls in godot

by default, every function you call in godot runs on the main thread, meaning they execute sequentially. function b won’t run until function a finishes. api calls usually take at least a few milliseconds waiting for responses from external services (my backend in this case), causing minor stutters or even complete freezes. clearly, api calls shouldn’t run on the main thread -- they need to run in parallel, on a separate thread.

luckily, handling multiple threads in godot is pretty straightforward. i did it only once and admittedly forgot the details afterward, but godot's documentation is awesome and has plenty of examples, even for complex stuff like threading. this makes it very accessible, even for beginners.

however, api calls still require a fair bit of boilerplate code. but since api calls aren't as common in godot as they are in browsers, it makes sense that this hasn't gotten as much attention for simplifying the implementation.

### design

having a decent design from the start is always important to me -- something i'd actually enjoy using. since the platform was pretty straightforward, coming up with a design wasn’t too hard.

_in this gif, there's a small input-field bug caused by updating the godot version_

![design](https://i.postimg.cc/3N9DkJx9/godot-e-JS9k-Hhw-Nh.gif)

the side menu took quite some effort because it had many tabs. i also think it's crucial to add animations and transitions early on, as these greatly improve the ui feel. i genuinely can’t stress enough how important it is for me to have a design i like as soon as possible. if i don’t enjoy how it looks, i easily lose motivation for the entire project.

### making it public

the platform isn’t public yet. the biggest blocker is hosting -- I still need to set that up. some minor tweaks are also needed. ideally, i'd love to set up automatic deployment using github actions. that could also make a really interesting tutorial topic for godot developers.

### conclusion

this short post doesn’t cover every detail of the platform. honestly, the remaining parts aren't very special, either feature- or architecture-wise. so i decided to focus only on the standout topics.

overall, i'm happy with the platform -- it's a solid foundation for hosting all my minigames.

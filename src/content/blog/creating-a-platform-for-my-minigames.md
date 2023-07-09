---
title: Creating a platform for my minigames
author: Floris
featured: false
draft: false
tags:
  - game-development
pubDatetime: 2022-02-20T20:47:52.756Z
ogImage: ""
description: One day while in the shower, I got the idea of starting a project that would combine multiple hobbies of mine into one. Part of it was about creating minigames.
---

_This blog post is a more technical text version of [the video about this project](https://www.youtube.com/watch?v=YH4vsr9XJ8s&)._

# Creating a platform for my minigames

As part of my content creation idea, I was planning to build multiple minigames. Since each game would be quite small, I would not want to publish each of them individually. Instead, I decided on building a platform which I can just update each time a new minigame is released.

## Planned features

The features I planned on adding were the following:

- Account management
  - Register an account
  - Login
  - Update your account
  - Reset password (get an email with a code used to reset the password)
  - Authenticated requests with session token
  - Automatic login with session token
- Highscore submission (when logged in)
- View top scores per minigame

## The tech stack

The minigames would be created in [Godot 4.0](https://godotengine.org/) (which is still in pre-alpha at the time of writing this). From a web-development perspective, the Godot game would act as the front-end.

For the back-end, aka the server, I chose to use Python. Godot's main scripting language is heavily inspired by Python and I like to use the same programming language accross the entire project as much as possible if I'm going to be working on all parts as it prevents confusion about switching between different programming languages.

At my [current job](https://brainial.com/) we use Python in the back-end and React (js) in the front-end. This has often lead to me defining functions wrong often before realising I'm using the syntax of the wrong language whenever I do full-stack work.

In the back-end I use a Python framework [FastAPI](https://fastapi.tiangolo.com/) which I really like. For the database I use [PostgreSQL](https://www.postgresql.org/).

## My experience with Godot 4.0 pre-alpha

This project was actually made with nightly Godot 4.0 builds but the first pre-alpha was right around the corner.

I already had quite a bit of experience with Godot 3.x. One time I participated in a weekly game jam to create [Orbing Around](https://kadeflo.itch.io/orbing-around) and I also started some other projects a while ago which I have not yet finished. One of these projects had quite a lot of UI elements so I was already familiar with building UI's in Godot. The UI nodes hadn't changed a lot with the new Godot version so it was quite easy for me to work with.  
I could quite easily implement most of my design elements, with the exception of gradients with rounded corners. As a solution for this I wanted to use shaders, but those were quite broken for 2D nodes at the time. This was the only real issue I ran into while working on the base platform, apart from a few engine crashes.

## API calls in the engine

Every single function that you execute runs on the main thread by default. This means that they are called in sequence. Function B will be executed only when function A has finished executing. The thing about API calls is that you need to wait at least a few milliseconds for a third party service (in my case my back-end) to respond. This would mean short stutters at best and long freezes at worst. So it was pretty obvious that these API calls should not run on the main thread. Instead, they should run in parallel to the rest of the engine, on a separate thread.

Thankfully it is quite easy to work with multiple threads in Godot. I did this only once and I didn't fully understand it anymore, but Godot's documentation is awesome and contains lots of examples for everything, including threading. This makes it extremely easy to implement this sort of complicated subject for someone with no experience.

API calls do need a lot of boilerplate code though, but I guess it's not as frequent as API calls in browsers so I get that the feature hasn't received as much attention to make it easily accessible as some other features.

## Design

I find it important to always have an at least decent design. Something that I would personally use. Something that lives up to my standards. Ofcourse this platfrom was pretty simple so it wasn't too hard to design something for it.

_In this gif there is a bug with the input fields caused by me updating the Godot version_

![design](https://i.postimg.cc/3N9DkJx9/godot-e-JS9k-Hhw-Nh.gif)

The side menu took quite a lot of effort since it contains a lot of tabs. I also find it very important to add animations/transitions as soon as possible because I think that improves the feel of the UI so much. I can't stress enough how important it is for me to have a design that I like as soon as possible. If I don't like the design I might lose motivation for the project.

## Making it public

The platform is not yet public. This is because I have not set up the hosting part of the platform. Also, some small things need tweaking. But the biggest blocker right now is the hosting.  
I would really love to set up some sort of automatic deployment through GitHub actions. This would also be an interesting topic to make a tutorial on I think, for the Godot part of automatic deployment.

## Conclusion

I have definetly not covered every part of the platform in this short post, but to be honest the rest of the platform is not that special feature-wise or architecture wise. So I only decided to talk about the topics that stood out to me.

I am happy with the platform, it's a great base for all the minigames.

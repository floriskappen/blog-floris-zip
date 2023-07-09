---
title: First big web development project
author: Floris
featured: false
draft: false
tags:
  - web-devevelopment
pubDatetime: 2021-04-14T20:47:52.756Z
ogImage: ""
description: After learning the basics of web dev, I started working on my first big project. It's cool enough to share.
---

# First big project

On 7 Sept of 2019, after finishing my first web development courses, I wanted to put my newly acquired skills to use. So I decided to make one of the standard "first projects": A to-do application. But I would try and think of all the cool features I would want in a to-do app and integrate it.

## Table of contents

## Login & Dashboard

This was a web app, so in order to have persistent todo's users needed to register an account. After logging in they would see a nice dashboard with some cool stats and links to their recent todo's.

The next step in the user journey would be to create their first list. This can be seen as a folder, containing multiple todos. They can customize the list with a color, an icon and share it with others. Yes, this todo app had a sharing system. I'm suprised I managed to pull that off!
![Dashboard](https://i.postimg.cc/gjLnH8Rz/Xe-QPWH70lr.gif)

## Todo creation

Creating a todo is easy. After selecting a list, you can click the plus icon on the lower right to create a new todo. A todo has a title, description, privacy settings, an expiry date and more. You can also select multiple "completion types".

The default would be to just check the todo off, but sometimes you might need a percentage slider or an increment button.

![Create todo](https://i.postimg.cc/TwzWStTL/s-Aqvpfludw.gif)

## Search system

There is a cool universal search bar, which you can use to search todo's, lists and even friends. I think universal search bars are extremely useful, and I'm happy with my implementation.

![Search](https://i.postimg.cc/RCGBgNG9/y8-GMb-C2-JEU.gif)

## Productivity tools

To help you finish your todo items, I also added a productivity tool. There are two settings: Pomodoro Timer & Do-it-now.

The Pomodoro Technique is created by Francesco Cirillo for a more productive way to work and study. The technique uses a timer to break down work into intervals, traditionally 25 minutes in length, separated by short breaks.

The Do-it-now setting is derived from the idea that if a task takes less than 5 minutes to do, you should do it immediately.

![Productivity](https://i.postimg.cc/RZKpbY9f/2-J5-XNpig4-J.gif)

## Social systems

I also tried to implement a social system. Every todo or list you create can be public, friend-only or private. Public means anyone that searches for your username can see the list/todo, while friend-only means that only people you have added to your friend list can see the todo.

You can search for people and send them a friend request. They will receive a notification, and if they accept they will be on your friends list.

You can share lists and todo's aswell, which is really useful. When creating or editing a list or todo, you can invite people to collaborate with. They will receive a notification where they can accept or ignore the invitation. Only the creator of the todo can manage with who it is shared. I never implemented a role system, and I think it would have been kind of overkill anyway.

## Design

At this point I was really into design, and as you can see I put a lot of care into it for this application. I still think it looks great years later!

While writing this post in 2021, I am less focussed on design and more on technique, as I think it fits my goals better. But this project is something I will always be proud of! It's good to know that I didn't design the flat artwork and icons you see throughout the app.

## Conclusion

Even though I never published it, because my motivation ran out and it was just a learning project, I think the end result is something to be proud of, given the fact that I just learned programming. It is the first web dev project I put a lot of time into. It was made in a period of 3 months working ~1.5 hour a day on it on average.

<get-related-articles category="WEB DEV" link-text="Read more">
</get-related-articles>

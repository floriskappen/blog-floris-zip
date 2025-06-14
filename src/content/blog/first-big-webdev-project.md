---
title: first big web development project
author: Floris
featured: false
draft: false
tags:
  - web-devevelopment
pubDatetime: 2021-04-14T20:47:52.756Z
ogImage: ""
description: "my first real web app: a fully-featured to-do list with social sharing, productivity tools, and even a friend system - built before i fully understood how ambitious that was."
---

on 7 sept 2019, after finishing my first web development courses, i wanted to put my newly acquired skills to use. i decided to build one of the classic "first projects": a to-do app. but i wanted to think of every cool feature i could possibly want in a to-do application and integrate them all.

### login & dashboard

since it was a web app, users needed an account to save their todos. after logging in, they'd see a nice dashboard featuring cool stats and quick links to their recent todos.

the next step would be creating their first list. think of lists as folders that can hold multiple todos. each list could be customized with a color and icon, and even shared with other users. yes, this todo app had a sharing system. honestly, i'm still surprised i managed to pull that off!

![Dashboard](https://i.postimg.cc/gjLnH8Rz/Xe-QPWH70lr.gif)

### todo creation

creating a todo was straightforward. after selecting a list, you'd click the plus icon in the bottom-right corner to add a new todo. each todo had a title, description, privacy settings, expiry date, and more. you could even choose between different completion methods.

the default was simply checking off a task, but sometimes you might need a percentage slider or increment button instead.

![Create todo](https://i.postimg.cc/TwzWStTL/s-Aqvpfludw.gif)

### search system

i also implemented a universal search bar, letting users quickly find todos, lists, and even friends. i genuinely think universal search bars are extremely useful, and i was pretty happy with how mine turned out.

![Search](https://i.postimg.cc/RCGBgNG9/y8-GMb-C2-JEU.gif)

### productivity tools

to help users actually finish their todos, i included a couple of productivity tools: the pomodoro timer and the "do-it-now" mode.

the pomodoro technique, created by francesco cirillo, breaks work into focused intervals (usually 25 minutes) with short breaks between them.

the "do-it-now" mode was inspired by the simple idea that if a task takes less than five minutes, you should do it immediately.

![Productivity](https://i.postimg.cc/RZKpbY9f/2-J5-XNpig4-J.gif)

### social systems

another ambitious feature was a social system. every todo or list could be set to public, friends-only, or private. public meant anyone searching your username could see it, friends-only meant only users on your friends list could view it.

users could search for each other and send friend requests, generating notifications that allowed the receiver to accept or ignore. you could also share todos and lists directly by inviting people to collaborate. invited users would get a notification and could accept or decline. only the original creator could manage collaborators -- I never implemented roles, but honestly, that would’ve probably been overkill anyway.

### design

at the time, i was really into design, and as you can see, i put quite a bit of care into the app's visuals. years later, i still think it looks pretty great!

writing this post in 2021, my focus has shifted more toward technical aspects rather than pure design, since that aligns better with my goals now. but this project remains something i'll always be proud of. as a quick note: the flat artwork and icons throughout the app weren't designed by me.

### conclusion

although i never published this project (my motivation ran out and it was purely for learning anyway), i still think the final result is something to be proud of—especially considering i'd just started learning to program. this was the first web development project that i put significant time into. i worked on it for about three months, averaging around 1.5 hours per day.

<get-related-articles category="WEB DEV" link-text="Read more">
</get-related-articles>

---
title: learning projects
author: Floris
featured: false
draft: false
tags:
  - web-devevelopment
pubDatetime: 2021-04-13T20:47:52.756Z
ogImage: ""
description: how i learned web dev from scratch by building apis, task managers, chat apps, and more - all powered by curiosity and a very long summer holiday.
---

in the summer vacation of 2019, i started learning web development. i began following a bunch of udemy courses. since then, i’ve made a few git repos with the projects i built while going through those courses and tutorials.

for web dev, this was the perfect way for me to learn. i’m super motivated by building cool things, so this hands-on approach really worked for me. for more theoretical stuff like machine learning, i wouldn’t recommend udemy though. a lot of those courses rely on buzzwords to get your attention, but the actual content is often pretty shallow.

## nodejs learning projects

in september 2019, i followed a nodejs course where i built a bunch of small apps to learn about design patterns and best practices.

### weather api interaction

in the first project, i built a little script that used weather & geocoding apis. honestly, using existing apis in learning projects is amazing -- it adds so much value without needing to build everything from scratch.

the app let you enter an address, converted it to latitude/longitude using one api, and then passed that to another api to get the weather forecast.

i also learned how to deploy it to [heroku](https://www.heroku.com/), which was cool because i could actually share it with friends.

### task manager api

in the next project, i made my own api. the user flow was something like:

1. register an account
2. log in
3. upload an avatar (optional)
4. create a new task
5. fetch all tasks
6. update task status

there were some other smaller features too, but this was the core.  
i remember struggling with user validation and file uploads. also… i stored avatars as base64 strings in the database, which i definitely wouldn’t do anymore lol. but hey, it worked.

### chatbox app

the final project in the course was a chatbox app. sounds fancy, but it was pretty simple. the front-end was provided by the tutor -- my job was to build the api (again, it was a nodejs course).

you’d type in a room name and a username, and join. everyone in the room would get a message when a new user joined. from there, it worked like a basic chat app.

### conclusion

i really enjoy working with nodejs. since i started out as a front-end dev using javascript, picking up back-end stuff felt super natural because it’s the same language.

## the “complete web developer course”

this was my intro to web dev. a general, but actually solid course. it was _long_, but i was so hyped to learn that i just powered through it -- skipping the parts i already knew like html & css.

javascript was the real turning point for me. it was really hard at first, but at some point it just clicked and everything started making sense.

besides javascript, i also got introduced to databases, apis, and even some basic python. but javascript was 100% the highlight for me.

## typescript

so, at the time of writing this (2021), i don’t use typescript that much. it was cool to learn, and i still remember the core concepts, but i haven’t really felt the need to use it yet. i think it makes more sense for larger-scale projects, and back then i was just working on small personal stuff.

## react

i actually started front-end dev with [vue](https://vuejs.org/), and i’m really glad i did. i love that framework. but at the time, [react](https://reactjs.org/) was by far the most popular, so i figured it’d be smart to learn it too.

for this, i built an ecommerce website using [firebase](https://firebase.google.com/) as the backend. pretty cool project. i learned a lot that carried over into my vue work as well.

one of the cooler things i made in react was a [conway’s game of life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life) app. here’s what it looked like in action:

![golly](https://i.imgur.com/6CsQHYJ.gif)

## conclusion

i did more courses, but these were the highlights. after learning all this stuff, i started building actual portfolio projects -- which you can still find on this site.

i also eventually landed a part-time job at [gravity](https://gravity.nl/) where i learned _so_ much more. not just about tech, but also soft skills, which honestly matter just as much. and yeah, no udemy course is gonna teach you those.

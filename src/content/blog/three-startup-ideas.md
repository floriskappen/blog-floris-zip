---
title: 3 startup ideas
author: Floris
featured: false
draft: false
tags:
  - web-devevelopment
pubDatetime: 2021-04-16T20:47:52.756Z
ogImage: ""
description: "three startup experiments, built back-to-back: from collaborative docs to music reviews and drag-and-drop websites. none made me rich, but all of them taught me more than any course ever could."
---

when i had just turned 16, i registered my first company. i wanted to sell band merch online. i had no clue what i was doing, but i really wanted to just _do something_. it didn’t work out, but it was a fun ride.

after that, in 2018, i started a company with a friend where we made websites for small businesses. at that point, i was mostly focused on design and had just started learning how to code. it didn’t last long, but i learned a lot from it.

it’s always been clear that i’ve had big ambitions. and even though none of my early projects led to huge success, they gave me a lot of experience and pushed me to level up my skills while building out my portfolio.

eventually, i started my own business. this was during the period where i was really motivated to create a startup, even if i had no idea how much work it would actually be. instead of going all-in on one idea, i decided to try a few different ones first. that led to me building three different apps in a pretty short amount of time.

## doccy — code-less documentation generation

doccy was a documentation generator. the idea was inspired by tools like [vuepress](https://vuepress.vuejs.org/), where you configure some settings, create a menu, and then write markdown to generate docs.

but i thought: why not make this accessible to non-devs too? documentation isn’t just for frameworks and api's.

#### login system

while working at [gravity](https://gravity.nl), i often used [strapi](https://strapi.io/), which is a headless cms. i really like it, so i used it for doccy’s backend. i implemented a basic login and password reset flow—just enough to make the app usable quickly. i didn’t add registration yet.

<util-aligner center>

![doccy-it-login](https://i.imgur.com/Bj2Ziyh.gif)

</util-aligner>

#### documentation creation

once you log in, you land on a dashboard that shows your “projects” (which are just different documentations). creating a new one looks like this:

![doccy-it-new-project](https://i.imgur.com/9GoShLO.gif)

#### page creation

each documentation could have multiple pages, which you could create and edit in the editor.

![doccy-it-new-page](https://i.imgur.com/XjTDSbk.gif)

there were supposed to be styling and menu options too, but i never got around to building that. the end goal was to let users:

1. export docs to a zip and host them manually
2. connect to [netlify](https://www.netlify.com/) and deploy directly

i finished the first one. the second one was more effort, so it stayed on the to-do list.

### conclusion

i think this was a solid idea, but i made the right call dropping it. the audience would've been too niche.

## songrev — album & single reviewing platform

i love music, and i also love watching people roast my favorite albums. reviewers like [anthony fantano](https://www.youtube.com/user/theneedledrop) are always entertaining. i also know someone who writes reviews for [sputnik music](https://www.sputnikmusic.com/), which is a super old-school but very active site.

i figured i could build a more modern and user-friendly review platform. on top of that, i integrated the spotify search api, so users could search for any artist listed on spotify.

#### search system

you could search songs, albums, and artists. if an artist wasn’t in my db yet, the app would fetch and store the data from spotify so i could attach reviews to it later. pretty cool system, i think.

![songrev-search](https://i.imgur.com/YNUGXDK.gif)

#### popular tracks & related artists

i also pulled extra info from spotify, like an artist's most popular tracks and their related artists. the review and rating system wasn't functional yet.

![songrev-artist](https://i.imgur.com/8ftznle.gif)

### conclusion

i dropped this one pretty early on. i realized there are already platforms like [rateyourmusic](https://rateyourmusic.com/) that do this better. and something like this would need a ton of marketing to get off the ground. also couldn’t figure out a good monetization model. still had fun playing with the spotify api though—there’s so much data to work with.

## landing pagr — drag & drop landing page builder

this was one of my older ideas. back when i had that small company with a friend in 2018, i stumbled across a landing page app and thought: this is pretty cool. nowadays there are tons of these tools, but back then i could barely find any.

the idea was that you could drag and drop components to build a landing page. then you’d pay the company to generate the real site.

#### our version

my spin on it was to make the landing page exportable right away, so it’d just work out of the box. keep in mind, this was when i barely knew how to code, so i didn’t think through most of the technical challenges. my friend handled the dev side.

i made a design, but eventually we stopped working on it. it was just too hard of a first project, and i think my friend didn’t feel like doing the heavy lifting solo.

#### what came of it?

why mention this? because later, when i started my own company, i built the first version of the site builder i still use as of writing this. the early version was built with nuxt (ssr) and strapi as the cms. i had automated deployment set up via github actions, and deployed everything in docker. honestly, it was kinda sick—but also _super_ expensive.

my cms setup was too complex for strapi. i had loads of nested components and needed dynamic fields, which wasn’t really an option, so i ended up with a bloated mess of fields everywhere. still, i think this version deserves its own blog post one day.

### conclusion

this project was way too ambitious back then. i had plans for tabs to switch between landing pages, user accounts, a payment system for unlocking premium components… it was a lot. with a team of three, this could’ve been done in a few sprints. but at the time, it was just me designing and my friend developing.

still, it eventually evolved into the site builder i use as of writing this, so that’s pretty awesome.

## final verdict

i’ve had a lot of ideas over the years. none of them made me rich, and most were probably too ambitious. but what did i lose? honestly—nothing. what i learned from working on these projects easily outweighs the time i spent on them.

i worked on these in the evenings after school, and i always saw them as potential portfolio work. but deep down, i’ve always held onto the dream that one of these ideas might someday turn into something bigger.

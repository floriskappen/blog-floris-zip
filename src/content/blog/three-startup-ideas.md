---
title: Three startup ideas
author: Floris
featured: false
draft: false
tags:
  - web-devevelopment
pubDatetime: 2021-04-16T20:47:52.756Z
ogImage: ""
description: The idea of creating a software startup has always fascinated me. Ofcourse I came to the realisation that it takes more than just a good idea, but that didn't stop me from trying!
---

# The three startup ideas

When I just turned 16, I registered my first company. I wanted to sell band merchandise online. I had no idea what I was doing, but I wanted to do something. It didn't work out, but was an enjoyable journey nonetheless.

Afterwards, in 2018 I started a company with a friend. We made websites for small businesses. At this time I was only designing, and just learning how develop. This lasted for a short while, but I learned a lot.

It's clear that I've always had big ambitions. And even though I haven't seen the big results I have once hoped for, it has given me a lot of experience, and the motivation to get my skills to the next level while expanding my portfolio at the same time.

Eventually I started my own business. This was in the period where I really wanted to create a startup, even though I didn't know how much work it would be. I decided that I wanted to try out different ideas before investing all my time in one of them. This lead to me creating three different applications in a short time.

## Table of contents

## Doccy, code-less documentation generation

Doccy is a documentation generation software. The idea came from documentation generators like [VuePress](https://vuepress.vuejs.org/), where after tweaking some settings and creating your menus, you can write documentation with markdown.

I thought it would be nice for non-developers to be able to use this aswell, since documentation is obviously not only useful for frameworks and API's.

#### Login system

While working at [Gravity](https://gravity.nl) I often used the [Strapi](https://strapi.io/) headless CMS. I think it's awesome! So I used that as the back-end of the application. I made simple login & password forgot systems to authenticate users. I wanted to make it usable as quick as possible, so I didn't make a registration system yet.

<util-aligner center>

![doccy-it-login](https://i.imgur.com/Bj2Ziyh.gif)

</util-aligner>

#### Documentation creation

When you arrive on the dashboard, you are greeted by your Projects, or as I called them, Documentations. We can create a new documentation.
![doccy-it-new-project](https://i.imgur.com/9GoShLO.gif)

#### Page creation

Each documentation has different pages, which can be created and edited like so.
![doccy-it-new-page](https://i.imgur.com/XjTDSbk.gif)

There should also be settings for the menu and styling for the docs, but I stopped working on the project before making those. Once you created your documentation the idea was that you could do one of the following:

1. Export it to a zip file, to host yourself
2. Connect with your [Netlify](https://www.netlify.com/) account to deploy it over there.

I implemented the first one, but the second one obviously takes more effort, so I haven't finished that.

### Conclusion

I think this was a pretty interesting idea, but I made the right decision by not continuing with this one. The audience would have been to niche.

## Songrev, an album/single reviewing platform

As an avid music fan, I like watching reviewers like [Anthony Fantano of The Needle Drop](https://www.youtube.com/user/theneedledrop) make fun of my favorite albums. I also know somebody who writes a lot of reviews for [Sputnik Music](https://www.sputnikmusic.com/). The latter however, is a very old-school website (which I have nothing against, I love old-school web design) with a very active community. I thought that with my awesome (not) UX skills I could make a more user-friendly platform, and on top of that you would already be able to find any artist (if they are listed on Spotify) because I was using the Spotify search API

#### Searching system

You can search for songs, albums or artists. If it's an artist that hasn't been searched before, I save key details to my database for later use. I need to store things like song or album ID's in order to connect reviews to them. I think this was a very cool idea.
![songrev-search](https://i.imgur.com/YNUGXDK.gif)

#### Popular tracks, related artists

I also get some other info from Spotify, like an artists popular tracks or related artists. The rating & review systems didn't work yet.
![songrev-artist](https://i.postimg.cc/2y4bGpZv/xs2-OS3n-P7e.gif)

### Conclusion

I stopped working on this one pretty soon. I realised there are other platforms like [RateYourMusic](https://rateyourmusic.com/) that do this way better. Plus, such a platform would need a lot of marketing, and I also couldn't think of a good monetization model for it. Still very fun to work with the Spotify API. So much data to work with!

## Landing Pagr, create landing pages by dragging and dropping components

This is an older idea. Back when I started that company with my friend in 2018, I was searching for inspiration and found this landing page creation app. These days there are hundreds of similar websites, but back then this was one of the only ones I could find. The idea of this app was that you would drag and drop components to create your landing page, and then you could pay the company to create it.

#### Our version

My variation on the idea was to make the landing page immediately exportable, so it would work right out of the box. Remember, this was when I just started to learn how to code, so I didn't really think through all the technical details yet, my friend was the one doing that.

I build a design but eventually we stopped working on it because it was a really hard first project for me, and I think that friend wasn't feeling like doing it all on his own.

#### What came of it?

So what was the point of telling this story? Well, eventually, when I started my own company, I created the first version of what would become my website builder, which is the framework this website is made in! That first version however, used Nuxt server-side rendering & Strapi as the CMS, and I would deploy websites in docker through an automated deployment flow I made with GitHub Actions. Pretty cool I think, but extremely expensive!

My CMS use-case was also too complex for Strapi, as I had many nested components, and I would have liked to have dynamic fields, but that wasn't an option so I just had a lot of fields all over the place. I think this project still deserves a blog post of its' own though.

### Conclusion

This project really was way too ambitious at the time. I remember I wanted to implement tabs where you could switch between different landing pages, account creation & a payment system to unlock different new perks and components, and way more. With a team of 3 this could probably be done in a couple of sprints, but at the time it was just me designing and my friend developing.

But it did eventually turn into the website building app that I still use today! So that's really cool.

## Final verdict

I have had many ideas over the years. None of them have made me a millionaire and they were all way too ambitious. But what did I lose? I think nothing, because in the end, what I learned heavily outweighs the time I put into these projects. I worked on them in the evenings after school, and I really did just see it as potential portfolio work. But I have always dreamed of the possibility of me being able to turn one of my projects into a successful startup.

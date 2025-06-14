---
title: "always getting sold-out concert tickets: a retrospective"
author: Floris
featured: false
draft: false
tags:
  - programming
pubDatetime: 2025-06-14T15:12:00Z
ogImage: ""
description: i wrote a bot to snipe sold-out concert tickets on ticketswap using proxies and throwaway accounts - then realized the ethical cost of outsmarting the system.
---

when a concert is sold out, people (especially in the netherlands) often use ticketswap to find a ticket. this is a secondary ticket marketplace where people resell their tickets if they can't attend anymore.

in 2023, i wrote a bot for ticketswap to help me get tickets for sold-out concerts. this was when i realized i could use the skills i taught myself to get something most other people couldn't.

"technology is everywhere, so it's useful to learn how it works," is something i've heard throughout my life. but at this point, it became obvious that understanding how a system like ticketswap operates could actually give me an advantage. it literally opened doors for me and my friends, taking us to places we otherwise would never have access to.

### the bot

it was a very simple idea. the proof of concept was done in a day. the program would do exactly what i normally do: refresh the event page on ticketswap until a ticket became available. if it did, the bot would immediately add the ticket to my cart—but it used an api connection instead of manually refreshing the webpage.

to bypass their security at the time, i implemented some basic features to stay anonymous and avoid getting banned immediately:

- rotating ip addresses (proxy)
- randomized rotating user agents

the rotating ip was especially time-consuming because i had to research and test many different proxy services to find the cheapest and highest-quality one.

when a ticket was added to my account, i'd receive a notification through discord. this was crucial because ticketswap gives you only 10 minutes to complete the purchase before the ticket leaves your cart.

the biggest challenge was scaling it up. once i started tracking more events and needed more tickets, i had to manage multiple accounts. i used apple's feature that lets you generate random icloud throwaway email addresses since protonmail and many other lesser-known providers were blocked by ticketswap. additionally, i had to ensure i accessed these accounts exclusively from a vpn, because logging in from my real ip would instantly get the account banned. i also had to use different credit cards for each account, since using the same card across multiple banned accounts caused them all to get banned simultaneously.

### the end

eventually, an [article got published](https://www.rtl.nl/rtl-nieuws/artikel/5395608/ticketswap-bots-automatisch-ticket-kopen), criticizing ticketswap for their lack of adequate bot protection. shortly after, they significantly stepped up their security measures and started using [reblaze](https://waap.docs.link11.com/v2.16/introduction-to-reblaze) for bot mitigation. i attempted to bypass this for a while using various methods, but after about a month, all my proxy networks (both residential and datacenter) were blocked. at that point, it was no longer worth the effort.

### ethics

while my bot was active, i gained access to many tickets that otherwise would have gone to either other bots or genuine concert-goers.

initially, this was a revelation to me, since i realized the skills i'd spent years developing could actually be used for something cool. as you might know, i'm a big concert fan, so my friends and i benefited greatly.

but looking back, it was unethical, and i regret taking such an unfair advantage.

the price of many things in our lives is purely determined by supply and demand. concerts, however, are often priced lower than market demand due to subsidies and other considerations. this is great, as everyone should have the opportunity to experience live music.

ticketswap operates on a similar model -- they intentionally cap resell prices to prevent pure market dynamics. i support this approach, as it makes tickets accessible. unlike sites like viagogo, where resell prices often skyrocket, ticketswap allows only a 120% resale markup (plus fees), making tickets immediately affordable to others.

by creating a bot that quickly bought these cheaper, second-hand tickets on ticketswap, i effectively reduced opportunities for others seeking tickets. i gained an unfair advantage, taking something someone else likely deserved more.

this isn't groundbreaking philosophy, but it's still important to me to explicitly acknowledge my actions.

the takeaway here is that acquiring unique skills that set you apart from others is always a double-edged sword. you can definitely misuse those skills if you want. just because you have an advantage doesn't mean you should always take it.

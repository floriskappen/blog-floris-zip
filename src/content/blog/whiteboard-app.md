---
title: whiteboard app
author: Floris
featured: false
draft: false
tags:
  - web-devevelopment
pubDatetime: 2021-04-15T20:47:52.756Z
ogImage: ""
description: in january of 2020 i worked on what could have been Miro! just kidding... The idea was very similar though.
---

in january 2020, i worked on what could’ve been miro. just kidding. kinda.

### introduction

it all started when i stumbled upon [paper.js](http://paperjs.org/). it looked super cool and i immediately wanted to build something with it. honestly, it had pretty much everything i needed out of the box. the data types were all there -- I just had to use them to build the app i had in mind.

at this point, i had just gotten comfortable with [vuejs](https://vuejs.org/). i noticed that because the entire app lived inside one huge `.vue` file. i _was_ planning to split it up into components, but yeah… should’ve done that from the start.

### the idea

the concept was to build a whiteboard app where you could create a room that stays active for 24 hours. you’d get a shareable link that you could send to others so you could draw together in real time.

i originally planned to use [websockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) for real-time collaboration, but the backend never got finished.

what _did_ get built though were some pretty sick front-end tools:

![collabza_tools](https://i.imgur.com/mfa1woz.gif)

### downsides of vectors

i wanted to make some fun pencil and brush tools. but since [paper.js](http://paperjs.org/) is vector-based, everything you draw is made up of points. to improve performance, it creates fewer points and connects them with [bézier curves](https://en.wikipedia.org/wiki/B%C3%A9zier_curve) to make the lines smooth. which is awesome -- until you try to erase.

it’s not like photoshop or other raster-based tools where the eraser just _feels_ right. here’s what i mean:

<util-aligner center>

![collabza_erase](https://i.imgur.com/e9P2Gs0.gif)

</util-aligner>

### layer system

one of the features i’m most proud of is the layer system. i stored every object in layers -- just like you’d expect if you’ve used photoshop. looking back, this might be a bit overkill for a whiteboard app, which is usually more about quick sketches than complex compositions. still, i think it’s a dope feature.

i also grouped objects by their tool type. so objects drawn with the pencil tool were grouped separately from shapes, etc. i wanted to add text and image support too, but never got around to it.

![collabza_layers](https://i.imgur.com/KgoAx3C.gif)

### conclusion

this was a fun project that really helped me understand how [vuejs](https://vuejs.org/) works. i definitely could’ve taken it further, but the direction i was going in -- like building something similar to [aggie.io](https://aggie.io/) -- probably wasn’t the right fit.

still super happy with the design though.  
you can [check the code here.](https://github.com/floriskappen/collabza-app)

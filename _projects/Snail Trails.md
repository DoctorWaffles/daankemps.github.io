---
title: Snail Trails
tags: [Programming, Game Design, UX/UI]
image: https://i.imgur.com/X0S9aiJ.png
description: You play as a snail, slow and steady, whilst painting the level in the color of your slime.
long_description: You play as a snail, slow and steady, whilst painting the level in the color of your slime. The snail can’t go onto blocks which isn’t its color, the snail can however change color with the use color change tiles. There are also pressure plates in the levels, which you have to activate while being colored in the same color of the pressure plate.
date: 2018-07-02
engine: OpenGL
trailer: snail_trails.mp4
---

{% include elements/intro.md %}

Snail Trails was a university project in the third quarter of our second year and required the use of a custom C++/OpenGL engine. On top of that the programmers had to provide a custom Lua scripting API for the game designer to use. We were given four weeks of time for development with a team of four designers/artists and two programmers. In this project we tried to keep a simple yet interesting game concept and a handpainted artstyle inspired by Bastion.

During this project I was responsible for the game and level design, as the game idea originated from me. To iterate quickly on the game design, I made a quick prototype usig Unity. This was also mainly due to the reason that the engineers had to build an engine from scratch, which ment that testing in-engine could only be done in a later stage. 


<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/F74lPUz.gif" caption="Initial idea" %}
    </div>
    <div class="col-sm" style="margin: 1rem auto;">
     <p> Initially the idea was to have two contesting players over a course, similar to Dots & Boxes, however after quick testing it was quickly discovered that a singleplayer puzzle game was a way better, less limiting and more fun solution.</p>
    </div>
</div>



<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/tjXYmw8.gif" caption="Color changing mechanic" %}
    </div>
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/5msb6vp.gif" caption="Lever mechanic" %}
    </div>
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/6w3oWr1.gif" caption="Following camera" %}
    </div>
</div>

Another thing I did during the early development stage was to create a basic user interface wireframe. Once the user interface was approved and the engine had its scripting API added to it, I also implemented the entire user interface, with 2D assets from another artist, to the game using LUA with the scripting API I was provided.


<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
    {% include elements/figure.html image="https://i.imgur.com/nnVDf7A.jpg" caption="Level selection" %}
    </div>
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/WY6TLjV.jpg" caption="Ingame HUD" %}
    </div>
  </div>

<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
    {% include elements/figure.html image="https://i.imgur.com/OXhjTJ3.jpg" caption="Controls" %}
    </div>
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/oX2RIoG.jpg" caption="Main Menu" %}
    </div>
  </div>



{% capture carousel_images %}
https://i.imgur.com/5vHzphQ.jpg
https://i.imgur.com/hzeq2un.jpg
https://i.imgur.com/Uh7LxFZ.jpg
https://i.imgur.com/JLZdQZO.jpg
https://i.imgur.com/fAp8eWj.jpg
https://i.imgur.com/DGDlGGc.jpg
https://i.imgur.com/Jt80W3l.jpg
{% endcapture %}
{% include elements/carousel.html %}

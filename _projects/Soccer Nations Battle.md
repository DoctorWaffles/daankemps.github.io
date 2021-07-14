---
title: Soccer Nations Battle
tags: [Programming, Level Design, 3D]
image: https://i.imgur.com/ChfZcaq.jpg
date: 2018-07-02T09:07:40+0100
description: Soccer Nations Battle is a local multiplayer side-scrolling soccer game. Prepare for fast-paced matches with lots of goals; block, tackle or simply outsmart your opponent. 
long_description: Soccer Nations Battle is a local multiplayer side-scrolling soccer game. Prepare for fast-paced matches with lots of goals block, tackle or simply outsmart your opponent. Play 1v1 up to 4v4 matches in this wild and hilarious party game. The more players, the more chaos, the more laughs.
trailer: soccer_nations_battle.webm
engine: Unity
---

{% include elements/intro.md %}

During my third year I was lucky enough to join [Virtual Play](https://virtualplay.games/)  in Utrecht as an intern. My main task was to fix bugs and add small additional features on their game Soccer Nations: Battle. I also worked on the input system of Soccer Nations: Battle, [Rewired](https://guavaman.com/projects/rewired/). Rewired replaces Unity’s input system with a new system that completely redefines how you work with input, with features like menu ownership and handling reconnecting/disconnecting controllers.

Furthermore I worked on implement a new localisation system, as the initial localization system had its flaws, so we decided to use the [I2 Localization plugin](http://inter-illusion.com/tools/i2-localization/) from the Unity Asset store. I2 Localization provided an easy to use synchronization between an excel sheet (which we located at our Google Drive) for each language strings and keys.


Aside of programming I also worked on some UI/UX improvements. One of the main parts I worked on was improving the userflow from starting up the game, selecting a level and team selection. Previously the userflow had little detail about which level was selected and there were no additional options. The new stage selection gave the player a bit more freedom on how he would like to play his game. With the additional thumbnail on the right there was no longer any confusion which level was selected, as they were quickly distinguishable. 
<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
    {% include elements/figure.html image="https://i.imgur.com/yHxtArX.png" caption="Old level selection" %}
    
    </div>
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/q3H7ZQS.png" caption="New level selection" %}
    </div>
  </div>
</div>

Furthermore I implemented a team selection scene for the selected level.

<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
    {% include elements/figure.html image="https://i.imgur.com/9fBUk9n.png" caption="Hell team selection" %}
    
    </div>
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/hPzFq2Q.png" caption="Heaven team selection" %}
       
    </div>
  </div>

  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
    {% include elements/figure.html image="https://i.imgur.com/cwINyY3.png" caption="Ship team selection" %}
    </div>
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/KAC2rGW.png" caption="Underwater team selection" %}
    </div>
  </div>
</div>







Throughout my internship at Virtual Play, I also participated in the Dutch Game Garden's [Network Lunches](https://www.dutchgamegarden.nl/project/network-lunch/). The network lunches attracted creative professionals, teachers, project leaders, future interns, and potential clients. During all the network lunches we played Soccer Nations: Battle together with or against other attendees, wrote down bugs, spectated others playing and asked for general feedback which we then further discussed and implemented.

<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
    {% include elements/figure.html image="https://i.imgur.com/VkVswp8.png" caption="Playtesting at Network Lunch" %}
    
    </div>
    <div class="col-sm">
        {% include elements/figure.html image="https://i.imgur.com/PLuL4hA.jpg" caption="Playtesting at Network Lunch" %}
    </div>
  </div>
</div>


{% capture carousel_images %}
https://i.imgur.com/fWl9ykJ.jpg
https://i.imgur.com/e1eCdTv.jpg
https://i.imgur.com/kNWn6Se.jpg
https://i.imgur.com/B33LJty.jpg
https://i.imgur.com/UhJLM2b.jpg
https://i.imgur.com/112KJWT.jpg
https://i.imgur.com/oHJVoYd.jpg
{% endcapture %}
{% include elements/carousel.html %}

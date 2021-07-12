---
name: Soccer Nations Battle
tools: [Programming, Level Design, 3D]
image: https://i.imgur.com/ChfZcaq.jpg
description:  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ac fringilla nunc.
date: 2018-07-02T09:07:40+0100
description: Soccer Nations Battle is a local multiplayer side-scrolling soccer game. Prepare for fast-paced matches with lots of goals; block, tackle or simply outsmart your opponent. 
long_description: Soccer Nations Battle is a local multiplayer side-scrolling soccer game. Prepare for fast-paced matches with lots of goals block, tackle or simply outsmart your opponent. Play 1v1 up to 4v4 matches in this wild and hilarious party game. The more players, the more chaos, the more laughs.
trailer_file: soccer_nations_battle.webm
engine: Unity
---

{% include elements/intro.md %}

During my third year I was lucky enough to join [Virtual Play](https://virtualplay.games/)  in Utrecht as an intern. My main task was to fix bugs and add small additional features on their game Soccer Nations: Battle. Bugs usually consisted on level issues. Besides that I worked on the optmizing the input system, [Rewired](https://guavaman.com/projects/rewired/) Rewired replaces Unity’s input system with a new system that completely redefines how you work with input. I added several user experience changes, such as functionalities that check whether controllers were disconnected whilst being active in a menu, in which case another player will receive ownership of that specific menu. In case the previous player would reconnect, he would regain that ownership. 

Furthermore I worked on implement a new system, as the initial localization system had its flaws, so we decided to use the [I2 Localization plugin](http://inter-illusion.com/tools/i2-localization/) from the Unity Asset store. I2 Localization provided an easy to use synchronization between an excel sheet (which we located at our Google Drive) for each language strings and keys.





In the new version (left) there are now multiple options available on the left side of the screen, which the player can navigate with their left  stick. On the right there is now a right thumbnail of the level, which the player can navigate with their right stick to select the level they would like to play.



The new stage selection should give the player a bit more freedom on how he would like to play his game. With the thumbnail there is no longer confusion which level is which and other levels are quickly distinguishable. Next to user experience I also created scalable scripts which should allow additional options to be done quite quickly.



Every first Wednesday of the month, there was a [Network Lunch](https://www.dutchgamegarden.nl/project/network-lunch/) located at the 5th floor of the Beatrix Building. The network lunch attracted creative professionals, teachers, project leaders, future interns, and potential clients. During all the network lunches we attended, we promoted and playtested Soccer Nations: Battle. 



<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
        <img src="https://i.imgur.com/noNPzz5.jpg"/>
    </div>
    <div class="col-sm">
        <img src="https://i.imgur.com/6TlwmCw.jpg"/>
    </div>
    <div class="col-sm">
        <img src="https://i.imgur.com/t5PSzLK.jpg"/>
    </div>
  </div>
</div>



As a side activity Virtual Play were asked to demonstrate their game [Alpha Mind](https://virtualplay.games/portfolio/alpha-mind-nl/) at Rijkswaterstaat in Utrecht. Alpha Mind is a VR game that you fully control with your brain. The goal of the game is to remain in a desired state of mindfulness. Initially, the game helps you with this, but as you progress the challenge grows! A player who keeps their brain under control, can control nature and the elements with the power of their mind. During those two days we had to guide, aid and inform people about Alpha Mind and mindfulness. Anyone who wanted to try out the demo had to wear a VR headset, a Muse headband and wear headphones so they wouldn’t be distracted by their surroundings. 





<!-- {% capture carousel_images %}
https://i.imgur.com/noNPzz5.jpg
https://i.imgur.com/6TlwmCw.jpg
https://i.imgur.com/t5PSzLK.jpg
https://i.imgur.com/RidzRWb.jpg

{% endcapture %}
{% include elements/carousel.html %} -->



{% capture carousel_images %}
https://i.imgur.com/fWl9ykJ.jpg
https://i.imgur.com/e1eCdTv.jpg
https://i.imgur.com/kNWn6Se.jpg
https://i.imgur.com/B33LJty.jpg
https://i.imgur.com/UhJLM2b.jpg
https://i.imgur.com/112KJWT.jpg
{% endcapture %}
{% include elements/carousel.html %}

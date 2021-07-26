---
title: A visual easing cheatsheet
tags: [Resource, UI/UX]
style: border
color: primary  
description: Nothing in nature moves linearly from one point to another. 
---

For my personal use I created a cheatsheet full of eases with several modes, all with their eases. All these animations were made using [DOTween](http://dotween.demigiant.com/), a Tweening library for Unity, and were automatically generated and recorded used using Unity's [Recorder](https://docs.unity3d.com/Packages/com.unity.recorder@2.0/manual/index.html) and uploaded using my own [ImgurClient for Unity](https://github.com/DoctorWaffles/UnityImgurClient)

Nothing in nature moves linearly from one point to another. In fact, things actually accelerate or decelerate when they move. Our brains are programmed to expect this type of movement, so you should take advantage of this when making animations or user interfaces. Natural movement makes your users more comfortable with your application, leading to a better overall experience. However, avoid them unless they are too short for the end user, otherwise they will feel like the interface is running too slow. 

All videos are running on 60 fps, in case you have trouble viewing them consider changing toggling in between the dark and light mode.

{% capture list_items %}
Color
Movement
Scale
Rotation
Gradient
Jump
Shake position
Shake rotation
Shake scale
{% endcapture %}
{% include elements/list.html title="Table of Contents" type="toc" %}


{% assign eases = "Flash,InBack,InBounce,InCirc,InCubic,InElastic,InExpo,InFlash,InOutBack,InOutBounce,InOutCirc,InOutCubic,InOutElastic,InOutExpo,InOutFlash,InOutQuad,InOutQuart,InOutQuint,InOutSine,InQuad,InQuart,InQuint,InSine,Linear,OutBack,OutBounce,OutCirc,OutCubic,OutElastic,OutExpo,OutFlash,OutQuad,OutQuart,OutQuint,OutSine" %}

{% assign easeArray = eases | split: "," %}



<!-- https://imgur.com/a/F2RJEfC -->
{% assign color = "https://i.imgur.com/VfnnmBX.mp4, https://i.imgur.com/NYirXSI.mp4, https://i.imgur.com/8Y6pjrS.mp4, https://i.imgur.com/OKC6xFq.mp4, https://i.imgur.com/hnawYdt.mp4, https://i.imgur.com/PsZoxqz.mp4, https://i.imgur.com/zDBidcs.mp4, https://i.imgur.com/HuBFUrV.mp4, https://i.imgur.com/6wbbUNZ.mp4, https://i.imgur.com/vrCfnQJ.mp4, https://i.imgur.com/PA3I6sQ.mp4, https://i.imgur.com/DaEnzaW.mp4, https://i.imgur.com/sNiGR1f.mp4, https://i.imgur.com/LtjRSis.mp4, https://i.imgur.com/9tiiN66.mp4, https://i.imgur.com/Bikbeqf.mp4, https://i.imgur.com/kp32jSm.mp4, https://i.imgur.com/C3SgEM0.mp4, https://i.imgur.com/Qy8J8Uf.mp4, https://i.imgur.com/NWOr7lp.mp4, https://i.imgur.com/3tWuQYW.mp4, https://i.imgur.com/OE9LbIw.mp4, https://i.imgur.com/zh9XoLQ.mp4, https://i.imgur.com/eD1qbXB.mp4, https://i.imgur.com/1XnlfiE.mp4, https://i.imgur.com/tHQbnqD.mp4, https://i.imgur.com/170fKG5.mp4, https://i.imgur.com/vWOJBSQ.mp4, https://i.imgur.com/Sis5F24.mp4, https://i.imgur.com/wT9dGw6.mp4, https://i.imgur.com/U2Aymmn.mp4, https://i.imgur.com/jV6aqtt.mp4, https://i.imgur.com/wwBT52n.mp4, https://i.imgur.com/BeWxpDu.mp4, https://i.imgur.com/cTl584h.mp4" %}


{% assign colorArray = color | split: "," %}

### Color 
<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = colorArray[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 






{% assign movement = "https://i.imgur.com/ni4D2wK.mp4, https://i.imgur.com/k0e00Mv.mp4, https://i.imgur.com/p6pJn8N.mp4, https://i.imgur.com/CdRwRTZ.mp4, https://i.imgur.com/0dsmaTQ.mp4, https://i.imgur.com/rYRlApl.mp4, https://i.imgur.com/Gr5DCOi.mp4, https://i.imgur.com/Hnxy6S6.mp4, https://i.imgur.com/nUwbjEO.mp4, https://i.imgur.com/xIoxY3S.mp4, https://i.imgur.com/Sx1jdfs.mp4, https://i.imgur.com/7l3I3KB.mp4, https://i.imgur.com/l53OjwL.mp4, https://i.imgur.com/Zo0KjJQ.mp4, https://i.imgur.com/cww0sMg.mp4, https://i.imgur.com/s5f5neE.mp4, https://i.imgur.com/r0VnO4m.mp4, https://i.imgur.com/Ltb2Zgx.mp4, https://i.imgur.com/TRQlues.mp4, https://i.imgur.com/fGb18Es.mp4, https://i.imgur.com/r8q6qKK.mp4, https://i.imgur.com/FXbEnIX.mp4, https://i.imgur.com/oii2Uii.mp4, https://i.imgur.com/iX5fdRX.mp4, https://i.imgur.com/QCHBMv0.mp4, https://i.imgur.com/ftcq4nn.mp4, https://i.imgur.com/YwDW375.mp4, https://i.imgur.com/kJuqjLv.mp4, https://i.imgur.com/C3lgakt.mp4, https://i.imgur.com/CUTWYso.mp4, https://i.imgur.com/P2W5mIA.mp4, https://i.imgur.com/TjRLjfe.mp4, https://i.imgur.com/ftytlW1.mp4, https://i.imgur.com/kVcldFT.mp4, https://i.imgur.com/htCPoJv.mp4, https://i.imgur.com/CU9vd91.mp4, https://i.imgur.com/iYI9sKz.mp4, https://i.imgur.com/oXWtGI4.mp4," %}


{% assign movementArray = movement | split: "," %}

### Movement [Imgur Album](google.com)
<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = movementArray[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 



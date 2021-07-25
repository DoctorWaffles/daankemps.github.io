---
title: A visual easing cheatsheet
tags: [Resource, UI/UX]
style: border
color: primary  
description: Nothing in nature moves linearly from one point to another. 
---

For my personal use I created a cheatsheet full of eases with several modes, all with their eases. All these animations were made using [DOTween](http://dotween.demigiant.com/), a Tweening library for Unity, and were automatically generated and recorded used using Unity's [Recorder](https://docs.unity3d.com/Packages/com.unity.recorder@2.0/manual/index.html).

Nothing in nature moves linearly from one point to another. In fact, things actually accelerate or decelerate when they move. Our brains are programmed to expect this type of movement, so you should take advantage of this when making animations or user interfaces. Natural movement makes your users more comfortable with your application, leading to a better overall experience. However, avoid them unless they are too short for the end user, otherwise they will feel like the interface is running too slow. 

All videos are running on 60 fps, in case you have trouble viewing them consider changing toggling in between the dark and light mode.


{% capture list_items %}
Movement
Scale
Rotation
Color
Gradient
Jump
Shake position
Shake rotation
Shake scale
{% endcapture %}
{% include elements/list.html title="Table of Contents" type="toc" %}

{% assign eases = "Unset,
        Linear,
        InSine,
        OutSine,
        InOutSine,
        InQuad,
        OutQuad,
        InOutQuad,
        InCubic,
        OutCubic,
        InOutCubic,
        InQuart,
        OutQuart,
        InOutQuart,
        InQuint,
        OutQuint,
        InOutQuint,
        InExpo,
        OutExpo,
        InOutExpo,
        InCirc,
        OutCirc,
        InOutCirc,
        InElastic,
        OutElastic,
        InOutElastic,
        InBack,
        OutBack,
        InOutBack,
        InBounce,
        OutBounce,
        InOutBounce,
        Flash,
        InFlash,
        OutFlash,
        InOutFlash," %}

{% assign easeArray = eases | split: "," | sort %}



{% assign doFillAmount = "https://i.imgur.com/ni4D2wK.mp4, https://i.imgur.com/k0e00Mv.mp4, https://i.imgur.com/p6pJn8N.mp4, https://i.imgur.com/CdRwRTZ.mp4, https://i.imgur.com/0dsmaTQ.mp4, https://i.imgur.com/rYRlApl.mp4, https://i.imgur.com/Gr5DCOi.mp4, https://i.imgur.com/Hnxy6S6.mp4, https://i.imgur.com/nUwbjEO.mp4, https://i.imgur.com/xIoxY3S.mp4, https://i.imgur.com/Sx1jdfs.mp4, https://i.imgur.com/7l3I3KB.mp4, https://i.imgur.com/l53OjwL.mp4, https://i.imgur.com/Zo0KjJQ.mp4, https://i.imgur.com/cww0sMg.mp4, https://i.imgur.com/s5f5neE.mp4, https://i.imgur.com/r0VnO4m.mp4, https://i.imgur.com/Ltb2Zgx.mp4, https://i.imgur.com/TRQlues.mp4, https://i.imgur.com/fGb18Es.mp4, https://i.imgur.com/r8q6qKK.mp4, https://i.imgur.com/FXbEnIX.mp4, https://i.imgur.com/oii2Uii.mp4, https://i.imgur.com/iX5fdRX.mp4, https://i.imgur.com/QCHBMv0.mp4, https://i.imgur.com/ftcq4nn.mp4, https://i.imgur.com/YwDW375.mp4, https://i.imgur.com/kJuqjLv.mp4, https://i.imgur.com/C3lgakt.mp4, https://i.imgur.com/CUTWYso.mp4, https://i.imgur.com/P2W5mIA.mp4, https://i.imgur.com/TjRLjfe.mp4, https://i.imgur.com/ftytlW1.mp4, https://i.imgur.com/kVcldFT.mp4, https://i.imgur.com/htCPoJv.mp4, https://i.imgur.com/CU9vd91.mp4, https://i.imgur.com/iYI9sKz.mp4, https://i.imgur.com/oXWtGI4.mp4," %}


{% assign doFillAmountLinks = doFillAmount | split: "," %}

### Movement
<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = doFillAmountLinks[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 

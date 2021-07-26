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



<!-- https://imgur.com/a/WCrQXUJ -->
{% assign color = "https://i.imgur.com/NWSIhL0.mp4, https://i.imgur.com/tRZ8ay2.mp4, https://i.imgur.com/qpJ5eUX.mp4, https://i.imgur.com/VRIy8z0.mp4, https://i.imgur.com/P9mUK1i.mp4, https://i.imgur.com/X88rTno.mp4, https://i.imgur.com/GzSdNRR.mp4, https://i.imgur.com/e40bAni.mp4, https://i.imgur.com/nQz11R3.mp4, https://i.imgur.com/bEm1gLM.mp4, https://i.imgur.com/PqGLNM7.mp4, https://i.imgur.com/VtSreDr.mp4, https://i.imgur.com/bm2cy7z.mp4, https://i.imgur.com/9gghGwc.mp4, https://i.imgur.com/EqJd00y.mp4, https://i.imgur.com/MJr10Eo.mp4, https://i.imgur.com/UnSfYGQ.mp4, https://i.imgur.com/oIK3HI0.mp4, https://i.imgur.com/QM8EjkK.mp4, https://i.imgur.com/KPapXc9.mp4, https://i.imgur.com/8gcAP4J.mp4, https://i.imgur.com/2mQAPFJ.mp4, https://i.imgur.com/JkjoV44.mp4, https://i.imgur.com/zeHm07R.mp4, https://i.imgur.com/Wazl5wv.mp4, https://i.imgur.com/uvrz9JJ.mp4, https://i.imgur.com/JRatIHW.mp4, https://i.imgur.com/T460EnT.mp4, https://i.imgur.com/PrZAMbT.mp4, https://i.imgur.com/x7Bgi5j.mp4, https://i.imgur.com/3EWJEGr.mp4, https://i.imgur.com/wb9Nt2A.mp4, https://i.imgur.com/PSYJPiR.mp4, https://i.imgur.com/Lq1JfpP.mp4, https://i.imgur.com/WW6EzYe.mp4, https://i.imgur.com/RFUOrlu.mp4, https://i.imgur.com/MxRIXTP.mp4, https://i.imgur.com/ocmZWMQ.mp4," %}


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



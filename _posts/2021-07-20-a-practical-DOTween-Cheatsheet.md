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


<script>
    $(document).ready(function() {       
        $('.video').each(function(i, obj) {
            $(this).on("mouseover", function() { hoverVideo(i); });
            $(this).on("mouseout", function() { hideVideo(i); });
        });
});

        function hoverVideo(i) {  
                $('.hovervideo')[i].play(); 
        }

        function hideVideo(i) {
                $('.hovervideo')[i].currentTime = 0; 
                $('.hovervideo')[i].pause(); 
        }
</script>





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
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut ut dapibus sem. Proin tincidunt lacus varius malesuada rutrum. Cras molestie faucibus quam, non tristique lacus maximus ut.
<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = colorArray[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 


<!-- https://imgur.com/a/u50BNNu -->
{% assign scale = "https://i.imgur.com/hL7yuKH.mp4, https://i.imgur.com/b4DQG50.mp4, https://i.imgur.com/bD9Yj9h.mp4, https://i.imgur.com/SmWNc2U.mp4, https://i.imgur.com/V64AjET.mp4, https://i.imgur.com/djCu9Tm.mp4, https://i.imgur.com/ibznE8T.mp4, https://i.imgur.com/7ExmAOk.mp4, https://i.imgur.com/Ng8pN2H.mp4, https://i.imgur.com/7PIHdPC.mp4, https://i.imgur.com/w6FmPPF.mp4, https://i.imgur.com/lbiFN0F.mp4, https://i.imgur.com/ZTr5H9W.mp4, https://i.imgur.com/DKG84WK.mp4, https://i.imgur.com/d4gZEs5.mp4, https://i.imgur.com/geosxC4.mp4, https://i.imgur.com/HUFuZXb.mp4, https://i.imgur.com/wkVnFd7.mp4, https://i.imgur.com/MrCi6iE.mp4, https://i.imgur.com/Fnz8kQH.mp4, https://i.imgur.com/9M2RBbL.mp4, https://i.imgur.com/ea9kPYu.mp4, https://i.imgur.com/19zoLYE.mp4, https://i.imgur.com/cJOYCGI.mp4, https://i.imgur.com/Of2ViR2.mp4, https://i.imgur.com/s2IxPAr.mp4, https://i.imgur.com/qRbXr9S.mp4, https://i.imgur.com/550ZKCz.mp4, https://i.imgur.com/diXjCSB.mp4, https://i.imgur.com/VMFAEYP.mp4, https://i.imgur.com/YPInDgS.mp4, https://i.imgur.com/jh6V4Nz.mp4, https://i.imgur.com/DVuVikU.mp4, https://i.imgur.com/HfXEfrb.mp4, https://i.imgur.com/G7Y4ckQ.mp4" %}


{% assign scaleArray = scale | split: "," %}

### Scale 
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut ut dapibus sem. Proin tincidunt lacus varius malesuada rutrum. Cras molestie faucibus quam, non tristique lacus maximus ut.
<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = scaleArray[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 


<!-- https://imgur.com/a/BQTEAAc -->
{% assign rotation = "https://i.imgur.com/q67VV3B.mp4, https://i.imgur.com/1kijmQk.mp4, https://i.imgur.com/OQJIUME.mp4, https://i.imgur.com/kuJcaXX.mp4, https://i.imgur.com/5nGWLh8.mp4, https://i.imgur.com/H7glidC.mp4, https://i.imgur.com/XzrFEsS.mp4, https://i.imgur.com/nuYyEHB.mp4, https://i.imgur.com/DUxzJpK.mp4, https://i.imgur.com/kWWpjD9.mp4, https://i.imgur.com/Eu9mvpl.mp4, https://i.imgur.com/LzlLbZT.mp4, https://i.imgur.com/giBmZc7.mp4, https://i.imgur.com/AXcDWDY.mp4, https://i.imgur.com/RQgxUFW.mp4, https://i.imgur.com/2EMW6QH.mp4, https://i.imgur.com/oceZT2d.mp4, https://i.imgur.com/NwAXNdq.mp4, https://i.imgur.com/YvwXmTo.mp4, https://i.imgur.com/8aTgdTj.mp4, https://i.imgur.com/K07RQcU.mp4, https://i.imgur.com/txVp1ff.mp4, https://i.imgur.com/TBHsAOO.mp4, https://i.imgur.com/k7ugop0.mp4, https://i.imgur.com/wV4VC5X.mp4, https://i.imgur.com/yQhKsBZ.mp4, https://i.imgur.com/ZnBqzie.mp4, https://i.imgur.com/tkYQloY.mp4, https://i.imgur.com/ocSyi0H.mp4, https://i.imgur.com/jviFl6s.mp4, https://i.imgur.com/FPWNHbV.mp4, https://i.imgur.com/jxNpSES.mp4, https://i.imgur.com/tqee4Hw.mp4, https://i.imgur.com/H0QC8WC.mp4, https://i.imgur.com/HxHiQZp.mp4" %}


{% assign rotationArray = rotation | split: "," %}

### Rotation 
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut ut dapibus sem. Proin tincidunt lacus varius malesuada rutrum. Cras molestie faucibus quam, non tristique lacus maximus ut.
<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = rotationArray[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 


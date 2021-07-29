---
title: A visual easing cheatsheet
tags: [Resource, UI/UX]
style: border
color: primary  
description: Nothing in nature moves linearly from one point to another. 
---

I use tweens in my 

 created a cheatsheet full of eases with several modes, all with their eases. All these animations were made using [DOTween](http://dotween.demigiant.com/), a Tweening library for Unity, and were automatically generated and recorded used using Unity's [Recorder](https://docs.unity3d.com/Packages/com.unity.recorder@2.0/manual/index.html) and uploaded using my own [ImgurClient for Unity](https://github.com/DoctorWaffles/UnityImgurClient)

Nothing in nature moves linearly from one point to another. In fact, things actually accelerate or decelerate when they move. Our brains are programmed to expect this type of movement, so you should take advantage of this when making animations or user interfaces. Natural movement makes your users more comfortable with your application, leading to a better overall experience. However, avoid them unless they are too short for the end user, otherwise they will feel like the interface is running too slow. 



{% assign eases = "Flash,InBack,InBounce,InCirc,InCubic,InElastic,InExpo,InFlash,InOutBack,InOutBounce,InOutCirc,InOutCubic,InOutElastic,InOutExpo,InOutFlash,InOutQuad,InOutQuart,InOutQuint,InOutSine,InQuad,InQuart,InQuint,InSine,Linear,OutBack,OutBounce,OutCirc,OutCubic,OutElastic,OutExpo,OutFlash,OutQuad,OutQuart,OutQuint,OutSine" %}

{% assign easeArray = eases | split: "," %}

<!-- https://imgur.com/a/F2RJEfC -->
{% assign color = "https://i.imgur.com/VfnnmBX.mp4, https://i.imgur.com/NYirXSI.mp4, https://i.imgur.com/8Y6pjrS.mp4, https://i.imgur.com/OKC6xFq.mp4, https://i.imgur.com/hnawYdt.mp4, https://i.imgur.com/PsZoxqz.mp4, https://i.imgur.com/zDBidcs.mp4, https://i.imgur.com/HuBFUrV.mp4, https://i.imgur.com/6wbbUNZ.mp4, https://i.imgur.com/vrCfnQJ.mp4, https://i.imgur.com/PA3I6sQ.mp4, https://i.imgur.com/DaEnzaW.mp4, https://i.imgur.com/sNiGR1f.mp4, https://i.imgur.com/LtjRSis.mp4, https://i.imgur.com/9tiiN66.mp4, https://i.imgur.com/Bikbeqf.mp4, https://i.imgur.com/kp32jSm.mp4, https://i.imgur.com/C3SgEM0.mp4, https://i.imgur.com/Qy8J8Uf.mp4, https://i.imgur.com/NWOr7lp.mp4, https://i.imgur.com/3tWuQYW.mp4, https://i.imgur.com/OE9LbIw.mp4, https://i.imgur.com/zh9XoLQ.mp4, https://i.imgur.com/eD1qbXB.mp4, https://i.imgur.com/1XnlfiE.mp4, https://i.imgur.com/tHQbnqD.mp4, https://i.imgur.com/170fKG5.mp4, https://i.imgur.com/vWOJBSQ.mp4, https://i.imgur.com/Sis5F24.mp4, https://i.imgur.com/wT9dGw6.mp4, https://i.imgur.com/U2Aymmn.mp4, https://i.imgur.com/jV6aqtt.mp4, https://i.imgur.com/wwBT52n.mp4, https://i.imgur.com/BeWxpDu.mp4, https://i.imgur.com/cTl584h.mp4" %}


{% assign colorArray = color | split: "," %}

### Transparency
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


<!-- https://imgur.com/a/u1pWw5q -->
{% assign rotation = "https://i.imgur.com/9CSG5fp.mp4, https://i.imgur.com/3aonSNt.mp4, https://i.imgur.com/KjfvgV0.mp4, https://i.imgur.com/EhNeDKs.mp4, https://i.imgur.com/SZYanZA.mp4, https://i.imgur.com/P84EF2r.mp4, https://i.imgur.com/qsiEqTw.mp4, https://i.imgur.com/4WTeqHZ.mp4, https://i.imgur.com/R2AP381.mp4, https://i.imgur.com/StTNZlN.mp4, https://i.imgur.com/KeKCyNH.mp4, https://i.imgur.com/e0tN4Ql.mp4, https://i.imgur.com/PlBzeYs.mp4, https://i.imgur.com/byG8yXK.mp4, https://i.imgur.com/6EomY2B.mp4, https://i.imgur.com/3Pr8yZL.mp4, https://i.imgur.com/AJ4eAok.mp4, https://i.imgur.com/M8MKVyx.mp4, https://i.imgur.com/kQPejAm.mp4, https://i.imgur.com/BsZwUM5.mp4, https://i.imgur.com/yHAEG0i.mp4, https://i.imgur.com/BmuWXtD.mp4, https://i.imgur.com/jR8X8wI.mp4, https://i.imgur.com/agiTV0u.mp4, https://i.imgur.com/QkL4AqS.mp4, https://i.imgur.com/0AAyu2u.mp4, https://i.imgur.com/gtUsGgR.mp4, https://i.imgur.com/iuUti41.mp4, https://i.imgur.com/6zUd9CC.mp4, https://i.imgur.com/QuxglGj.mp4, https://i.imgur.com/nODZnfE.mp4, https://i.imgur.com/uKMjb8S.mp4, https://i.imgur.com/9EnLlzz.mp4, https://i.imgur.com/N6fqVRK.mp4, https://i.imgur.com/bCQW5eH.mp4" %}


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


---
title: A visual easing cheatsheet
tags: [Resource, UI/UX]
style: border
color: primary  
description: Nothing in nature moves linearly from one point to another. 
---

For my personal use I created a cheatsheet full of eases with several modes, all with their eases. All these animations were made using [DOTween](http://dotween.demigiant.com/), a Tweening library for Unity, and were automatically generated and recorded used using Unity's [Recorder](https://docs.unity3d.com/Packages/com.unity.recorder@2.0/manual/index.html).

Nothing in nature moves linearly from one point to another. In fact, things actually accelerate or decelerate when they move. Our brains are programmed to expect this type of movement, so you should take advantage of this when making animations or user interfaces. Natural movement makes your users more comfortable with your application, leading to a better overall experience. However, avoid them unless they are too short for the end user, otherwise they will feel like the interface is running too slow. 



{% capture list_items %}
DOGradientColor
DOFillAmount
DOMove
DOColor
DOFade
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



{% assign doFillAmount = "https://i.imgur.com/2G3TBqg.mp4,
https://i.imgur.com/ZJ3JjMO.mp4,
https://i.imgur.com/0ua7CrA.mp4,
https://i.imgur.com/Fwk9iMN.mp4,
https://i.imgur.com/x9rPCA1.mp4,
https://i.imgur.com/3wZU3kr.mp4,
https://i.imgur.com/moTWe1D.mp4,
https://i.imgur.com/L0JKVae.mp4,
https://i.imgur.com/UX2FMOH.mp4,
https://i.imgur.com/29s2FkQ.mp4,
https://i.imgur.com/lxkbVye.mp4,
https://i.imgur.com/emhKmDO.mp4,
https://i.imgur.com/yHT7YQX.mp4,
https://i.imgur.com/R2S3hJz.mp4,
https://i.imgur.com/aEskBRZ.mp4,
https://i.imgur.com/Sd28yHy.mp4,
https://i.imgur.com/4xCK9RZ.mp4,
https://i.imgur.com/bVC5Qqj.mp4,
https://i.imgur.com/hXgzdUm.mp4,
https://i.imgur.com/vkTP1n2.mp4,
https://i.imgur.com/isml7UD.mp4,
https://i.imgur.com/qj8Ltiz.mp4,
https://i.imgur.com/ZI3QSUW.mp4,
https://i.imgur.com/4cCt9Iv.mp4,
https://i.imgur.com/4OCd2cD.mp4,
https://i.imgur.com/dFKY8Sm.mp4,
https://i.imgur.com/RHDgmNW.mp4,
https://i.imgur.com/y7TxIkZ.mp4,
https://i.imgur.com/MUlYecT.mp4,
https://i.imgur.com/mGSYOqB.mp4,
https://i.imgur.com/aPA10qT.mp4,
https://i.imgur.com/X7lMz9f.mp4,
https://i.imgur.com/U0sedny.mp4,
https://i.imgur.com/IZGW2Xp.mp4,
https://i.imgur.com/PwPiuZJ.mp4,
https://i.imgur.com/eFr4p8p.mp4,
https://i.imgur.com/nXpPLMK.mp4,
https://i.imgur.com/HLcNoiF.mp4," %}


{% assign doFillAmountLinks = doFillAmount | split: "," %}

### DOFillAmount
> DOFillAmount(1, 1).SetEase(ease);

<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = doFillAmountLinks[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 

---
title: A practical UI DOTween cheatsheet
tags: [Resource]
style: border
color: primary  
description: Bye bye slow Wordpress, hello lightning fast Jekyll!
---




{% assign doFillAmount = "https://i.imgur.com/2G3TBqgt.mp4,
https://i.imgur.com/ZJ3JjMOt.mp4,
https://i.imgur.com/0ua7CrAt.mp4,
https://i.imgur.com/Fwk9iMNt.mp4,
https://i.imgur.com/x9rPCA1t.mp4,
https://i.imgur.com/3wZU3krt.mp4,
https://i.imgur.com/moTWe1Dt.mp4,
https://i.imgur.com/L0JKVaet.mp4,
https://i.imgur.com/UX2FMOHt.mp4,
https://i.imgur.com/29s2FkQt.mp4,
https://i.imgur.com/lxkbVyet.mp4,
https://i.imgur.com/emhKmDOt.mp4,
https://i.imgur.com/yHT7YQXt.mp4,
https://i.imgur.com/R2S3hJzt.mp4,
https://i.imgur.com/aEskBRZt.mp4,
https://i.imgur.com/Sd28yHyt.mp4,
https://i.imgur.com/4xCK9RZt.mp4,
https://i.imgur.com/bVC5Qqjt.mp4,
https://i.imgur.com/hXgzdUmt.mp4,
https://i.imgur.com/vkTP1n2t.mp4,
https://i.imgur.com/isml7UDt.mp4,
https://i.imgur.com/qj8Ltizt.mp4,
https://i.imgur.com/ZI3QSUWt.mp4,
https://i.imgur.com/4cCt9Ivt.mp4,
https://i.imgur.com/4OCd2cDt.mp4,
https://i.imgur.com/dFKY8Smt.mp4,
https://i.imgur.com/RHDgmNWt.mp4,
https://i.imgur.com/y7TxIkZt.mp4,
https://i.imgur.com/MUlYecTt.mp4,
https://i.imgur.com/mGSYOqBt.mp4,
https://i.imgur.com/aPA10qTt.mp4,
https://i.imgur.com/X7lMz9ft.mp4,
https://i.imgur.com/U0sednyt.mp4,
https://i.imgur.com/IZGW2Xpt.mp4,
https://i.imgur.com/PwPiuZJt.mp4,
https://i.imgur.com/eFr4p8pt.mp4,
https://i.imgur.com/nXpPLMKt.mp4,
https://i.imgur.com/HLcNoiFt.mp4," %}


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

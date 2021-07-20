---
title: A practical UI DOTween cheatsheet
tags: [Resource]
style: border
color: primary  
description: Bye bye slow Wordpress, hello lightning fast Jekyll!
---

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

{% assign doFade = "https://i.imgur.com/OgZegtX.mp4,
https://i.imgur.com/sr5xDKw.mp4,
https://i.imgur.com/11EjdJr.mp4,
https://i.imgur.com/3fdGNNp.mp4,
https://i.imgur.com/lI2VkP0.mp4,
https://i.imgur.com/HiGi3Ma.mp4,
https://i.imgur.com/k4uJDb4.mp4,
https://i.imgur.com/906KhXa.mp4,
https://i.imgur.com/VMoBGYH.mp4,
https://i.imgur.com/dGFfv9t.mp4,
https://i.imgur.com/c1tl3vt.mp4,
https://i.imgur.com/jbF9QIR.mp4,
https://i.imgur.com/g6uJ39j.mp4,
https://i.imgur.com/kiC9N8b.mp4,
https://i.imgur.com/YQs2UZf.mp4,
https://i.imgur.com/jcVqqfq.mp4,
https://i.imgur.com/ZyAjjw3.mp4,
https://i.imgur.com/bOsbva1.mp4,
https://i.imgur.com/Dr2VS8I.mp4,
https://i.imgur.com/AG6iiyX.mp4,
https://i.imgur.com/HCbJjWH.mp4,
https://i.imgur.com/BAFSSdr.mp4,
https://i.imgur.com/mSAKlzw.mp4,
https://i.imgur.com/cZah3pe.mp4,
https://i.imgur.com/Rzaqlce.mp4,
https://i.imgur.com/ud4XwW6.mp4,
https://i.imgur.com/bkvdHAR.mp4,
https://i.imgur.com/iIXrgaG.mp4,
https://i.imgur.com/oSUO6N5.mp4,
https://i.imgur.com/pUpn57M.mp4,
https://i.imgur.com/EfRRY0u.mp4,
https://i.imgur.com/wwtysI8.mp4,
https://i.imgur.com/PbyJgwc.mp4,
https://i.imgur.com/nsU8B1U.mp4,
https://i.imgur.com/CpyZsmR.mp4,
https://i.imgur.com/URpyOQR.mp4,
https://i.imgur.com/dwb4tlG.mp4,
https://i.imgur.com/HBM618a.mp4" %}

{% assign doFadeLinks = doFade | split: "," %}

### DOFade
> DOFade(0, 1).SetEase(ease);

<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = doFadeLinks[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 

{% assign doColor = "
https://i.imgur.com/eQuRGlf.mp4,
https://i.imgur.com/sZujKGt.mp4,
https://i.imgur.com/DCJIKSY.mp4,
https://i.imgur.com/0n97Wib.mp4,
https://i.imgur.com/bOYep28.mp4,
https://i.imgur.com/mjVBAL2.mp4,
https://i.imgur.com/CY730X3.mp4,
https://i.imgur.com/AGDQJZN.mp4,
https://i.imgur.com/MsZt3mK.mp4,
https://i.imgur.com/ijFzmS9.mp4,
https://i.imgur.com/KJP9z8i.mp4,
https://i.imgur.com/vdMjIKi.mp4,
https://i.imgur.com/OOFXs7p.mp4,
https://i.imgur.com/Z8Gebtk.mp4,
https://i.imgur.com/SqHZ8IF.mp4,
https://i.imgur.com/Ycopc0g.mp4,
https://i.imgur.com/mAKma1c.mp4,
https://i.imgur.com/AwmXptZ.mp4,
https://i.imgur.com/H4C5FWE.mp4,
https://i.imgur.com/R8ZjeKw.mp4,
https://i.imgur.com/TcGRwTP.mp4,
https://i.imgur.com/QXkcvMG.mp4,
https://i.imgur.com/ZgVachd.mp4,
https://i.imgur.com/vwYewZR.mp4,
https://i.imgur.com/kqkw9ov.mp4,
https://i.imgur.com/UaZ5VQo.mp4,
https://i.imgur.com/Uh0WJjG.mp4,
https://i.imgur.com/VYQspSu.mp4,
https://i.imgur.com/B0EnofS.mp4,
https://i.imgur.com/rKdTzhW.mp4,
https://i.imgur.com/yvUfTjt.mp4,
https://i.imgur.com/8yWlhdM.mp4,
https://i.imgur.com/Jkp7YeQ.mp4,
https://i.imgur.com/Nqv7wqf.mp4,
https://i.imgur.com/kA4lVsY.mp4,
https://i.imgur.com/27Cgmz5.mp4,
https://i.imgur.com/JQtivTA.mp4,
https://i.imgur.com/xRWEQG6.mp4," %}


{% assign doColorLinks = doColor | split: "," %}

### DOColor
> DOColor(0, 1).SetEase(ease);

<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = doColorLinks[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 


{% assign doFillAmount = "https://i.imgur.com/Y01zzan.mp4,
https://i.imgur.com/stAQeEO.mp4,
https://i.imgur.com/28vH2hq.mp4,
https://i.imgur.com/4IiuevS.mp4,
https://i.imgur.com/HqGH5oH.mp4,
https://i.imgur.com/S2CalgN.mp4,
https://i.imgur.com/ljABwCO.mp4,
https://i.imgur.com/CibpUPG.mp4,
https://i.imgur.com/wGpxnjl.mp4,
https://i.imgur.com/j3nuS7Y.mp4,
https://i.imgur.com/M8sWSEj.mp4,
https://i.imgur.com/tCNeA7w.mp4,
https://i.imgur.com/Jtz5Dpk.mp4,
https://i.imgur.com/24hkK7b.mp4,
https://i.imgur.com/OOojhXJ.mp4,
https://i.imgur.com/yT2exNB.mp4,
https://i.imgur.com/jeDFBC6.mp4,
https://i.imgur.com/PFZT9DI.mp4,
https://i.imgur.com/v3bdjHB.mp4,
https://i.imgur.com/PZVQe7w.mp4,
https://i.imgur.com/UyJAhCU.mp4,
https://i.imgur.com/tSPXIud.mp4,
https://i.imgur.com/SLaXbic.mp4,
https://i.imgur.com/7cdNsRZ.mp4,
https://i.imgur.com/SLhNvwO.mp4,
https://i.imgur.com/TmiR5ey.mp4,
https://i.imgur.com/ekVMHlf.mp4,
https://i.imgur.com/6aZKI4n.mp4,
https://i.imgur.com/WndkiEr.mp4,
https://i.imgur.com/j9eXEAQ.mp4,
https://i.imgur.com/pG2vm8M.mp4,
https://i.imgur.com/0mhY89p.mp4,
https://i.imgur.com/u0hVMP8.mp4,
https://i.imgur.com/xXCkOzj.mp4,
https://i.imgur.com/T0tFVWc.mp4,
https://i.imgur.com/SpVEg5f.mp4,
https://i.imgur.com/SDYQCH1.mp4,
https://i.imgur.com/1TgBaDP.mp4," %}


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

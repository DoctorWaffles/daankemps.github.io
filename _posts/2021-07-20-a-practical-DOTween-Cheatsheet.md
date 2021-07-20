---
title: A practical DOTween Cheatsheet
tags: [Resource]
style: border
color: primary  
description: Bye bye slow Wordpress, hello lightning fast Jekyll!
---


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

{% assign easeArray = eases | split: "," %}

All Dotween eases
> {{ easeArray }}


### Image fades
```DOFade(0, 1).SetEase(ease);```

<div class="row">
{% for ease in easeArray %}
    <div class="col-sm">
  {% include elements/video_figure.html video="https://i.imgur.com/IjF7Leb.mp4" width="100%" height="100%" caption="InBack" %}
    </div>
{% endfor %}
</div> 



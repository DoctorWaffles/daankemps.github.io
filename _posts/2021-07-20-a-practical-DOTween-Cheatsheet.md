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

{% assign easeArray = eases | split: "," | sort %}

{% assign videoLinks = "https://imgur.com/OgZegtX,
https://imgur.com/sr5xDKw,
https://imgur.com/11EjdJr,
https://imgur.com/3fdGNNp,
https://imgur.com/lI2VkP0,
https://imgur.com/HiGi3Ma,
https://imgur.com/k4uJDb4,
https://imgur.com/906KhXa,
https://imgur.com/VMoBGYH,
https://imgur.com/dGFfv9t,
https://imgur.com/c1tl3vt,
https://imgur.com/jbF9QIR,
https://imgur.com/g6uJ39j,
https://imgur.com/kiC9N8b,
https://imgur.com/YQs2UZf,
https://imgur.com/jcVqqfq,
https://imgur.com/ZyAjjw3,
https://imgur.com/bOsbva1,
https://imgur.com/Dr2VS8I,
https://imgur.com/AG6iiyX,
https://imgur.com/HCbJjWH,
https://imgur.com/BAFSSdr,
https://imgur.com/mSAKlzw,
https://imgur.com/cZah3pe,
https://imgur.com/Rzaqlce,
https://imgur.com/ud4XwW6,
https://imgur.com/bkvdHAR,
https://imgur.com/iIXrgaG,
https://imgur.com/oSUO6N5,
https://imgur.com/pUpn57M,
https://imgur.com/EfRRY0u,
https://imgur.com/wwtysI8,
https://imgur.com/PbyJgwc,
https://imgur.com/nsU8B1U,
https://imgur.com/CpyZsmR,
https://imgur.com/URpyOQR,
https://imgur.com/dwb4tlG,
https://imgur.com/HBM618a"}

{% assign videoLinks = eases | split: "," %}

### Image fades
```DOFade(0, 1).SetEase(ease);```

<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-3">
    {% assign video = videoLinks[{{forloop.index0}}] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=video width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 



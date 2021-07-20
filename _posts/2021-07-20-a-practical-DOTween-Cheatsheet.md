---
title: A practical UI DOTween cheatsheet
tags: [Resource]
style: border
color: primary  
description: Bye bye slow Wordpress, hello lightning fast Jekyll!
---
<script>
var cip = $(".video").hover( hoverVideo, hideVideo );

function hoverVideo(e) {  
    $('video', this).get(0).play(); 
}

function hideVideo(e) {
    $('video', this).get(0).pause(); 
}
}
</script>

{% capture list_items %}
DOGradientColor
DOFillAmount
DOMove
DOColor
DOFade
{% endcapture %}
{% include elements/list.html title="Table of Contents" type="toc" %}


<div class="video">
    <video class="thevideo" loop preload="none">
      <source src="https://giant.gfycat.com/VerifiableTerrificHind.mp4" type="video/mp4">
      <source src="https://giant.gfycat.com/VerifiableTerrificHind.webm" type="video/webm">
    Your browser does not support the video tag.
    </video>
  </div>
  Hover mouse over video. Desktop only [ Obviously! ;) ]
</div>



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

{% assign videoLinks = "https://i.imgur.com/OgZegtX.mp4,
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

{% assign videos = videoLinks | split: "," %}

### DOFade
> Fades the target's alpha to the given value <br >
> DOFade(0, 1).SetEase(ease);

<div class="row">
{% for ease in easeArray %}
    <div class="col-sm-2">
    {% assign videolink = videos[forloop.index0] %}
    {% assign caption = ease %}
    {% include elements/video_figure.html caption=caption video=videolink width="100%" height="100%"   %}
    </div>
{% endfor %}
</div> 


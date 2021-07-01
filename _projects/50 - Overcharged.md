---
name: Overcharged
tools: [C#, Unity, School Project]
image: https://i.imgur.com/Y7S36vb.jpg
description: Overcharged is a local multiplayer game in which two players attempt to shoot the ball inside their opponent's hoop.
---

{% include elements/video.html id="yf_GyHBjipY" %}


##### Overcharged (School project - 2018)
> Overcharged is a local multiplayer game in which two players attempt to shoot the ball inside their opponent's hoop. Both players have a set of abilities. Such as dashing, deflecting and a jetpack for jumping, to make the gameplay a bit more interesting.

During the project I was mostly the bridge between the programmers and the artists. Next to that I worked on sounds (with the use of FMOD), modelling, UVing, texturing, some shader work and I transfered most artist content to git.

<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
    <video muted autoplay loop style="height: 100%;  width: 100%;  overflow:hidden;    display:block;">
   <source type="video/mp4" src="https://i.imgur.com/B6nG8SS.mp4">
</video>
    </div>
    <div class="col-sm" style="margin-top: 20px">
<h6>Shader</h6>
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur augue tortor, tempus quis magna in, sodales elementum arcu. Nulla feugiat nisl eleifend neque eleifend, ac lacinia lorem tristique. Vestibulum sit amet lorem vel nunc aliquam pulvinar in ut nisi. 
    </div>
  </div>
</div>

```glsl
void vert(inout appdata_full v) {
    half noiseVal = tex2Dlod(_NoiseTex, float4(v.texcoord.xy, 0, 0)).r;
}

void surf(Input IN, inout SurfaceOutput o) {
    half noiseVal = tex2D(_NoiseTex, IN.uv_NoiseTex).r + (sin(_Time.y)) / _Speed;
    half4 color = tex2D(_RampTex, float2(saturate(_RampVal + noiseVal), 1)) * _Color;
    if (color.a < _Cutoff)
    {
        discard;
    }
    o.Albedo = color.rgb;
    o.Emission = color.rgb;
}
```

<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
    <video muted autoplay loop style="height: 100%;  width: 100%;  overflow:hidden;    display:block;">
   <source type="video/mp4" src="https://i.imgur.com/pcssafq.mp4">
</video>
    </div>
    <div class="col-sm" style="margin-top: 20px">
<h6>Shader</h6>
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur augue tortor, tempus quis magna in, sodales elementum arcu. Nulla feugiat nisl eleifend neque eleifend, ac lacinia lorem tristique. Vestibulum sit amet lorem vel nunc aliquam pulvinar in ut nisi. 
    </div>
  </div>
</div>


```glsl

vertexOutput vert(vertexInput input)
{
    vertexOutput output;
    float4 camDir = mul(UNITY_MATRIX_P,
    mul(UNITY_MATRIX_MV, float4(0.0, 0.0, 0.0, 1.0))
    - float4(input.vertex.x * _Scale, input.vertex.z * _Scale, 0.0, 0.0));

    output.pos = camDir;
    output.tex = input.tex;
    return output;
}

float4 frag(vertexOutput input) : COLOR
{
    float2 tp = float2(input.tex.x, input.tex.y);
    float4 col = tex2D(_MainTex, tp) * _Color;
    if (col.a < _Cutoff)
    {
        discard;
    }
    return col;
}
```

##### Overcharged
As we took Rocket League as an inspiration, the team wanted a similar crowd. I invested some time in creating a billboard shader to recreate such a crowd. It worked out nicely, I used a small script to assign each 'egg' a different color from it's team color range.

Next to the the crowd shader the team wanted some indication around the playfield without obstructing the view of the players. I created a basic shader with a noise texture that scrolled with the use of a sine wave, creating a flowing 'energy field'.
th modelling I focussed mostly on the arena and its stand(s). I kept the field architecture simple and clean, to not distract the players. The only feature the field offers is an indication on which side the player belongs. Both field assets and stand assets were made modular.
or all sounds I used FMOD to add some random modulation to pitch and volume. I made my own custom FMOD class which handled all audio for me, which I for example used for the player's jetpack. Making it so that the volume and pitch of the jetpack is dependent on the jetpack's energy.

As for the sounds themselves, I tried to give them an electric feeling, as the ball itself contained electricity and sparks.

{% capture carousel_images %}
https://i.imgur.com/NC1ma1K.png
https://i.imgur.com/V3eEasw.png
https://i.imgur.com/ghhyJuA.png
https://i.imgur.com/mKEuze0.png
{% endcapture %}
{% include elements/carousel.html %}

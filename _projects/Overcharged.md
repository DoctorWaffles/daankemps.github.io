---
name: Overcharged
tag: [School Project, C#, Shaders]
image: https://i.imgur.com/Y7S36vb.jpg
date: 2017-12-02T09:07:40+0100
engine: Unity
description: Overcharged is a local multiplayer game in which two players attempt to shoot the ball inside their opponent's hoop.
long_description: Overcharged is a local multiplayer game in which two players attempt to shoot the ball inside their opponent's hoop. Both players have a set of abilities. Such as dashing, deflecting and a jetpack for jumping, to make the gameplay a bit more interesting.
trailer_file: overcharged.mp4
---

{% include elements/intro.md %}

Overcharged was a university project in the second quarter of my second year in which we were free to create any indie game we would like to by utilizing any engine we wanted to. We were given three weeks of time for development with a team of four designers/artists and two programmers. During the project I was mostly the bridge between the programmers and the artists. Next to that I worked on sounds (with the use of FMOD), modelling, UVing, texturing, some shader work and I transfered most artist content to git.

As we took Rocket League as an inspiration, the team wanted a similar looking crowd. I invested some time in creating a billboard shader to recreate such a crowd. To assign each billboard a different color, within their team color range, I used a small script. Next to the the crowd shader the team wanted some indication around the playfield without obstructing the view of the players. I created a basic shader with a noise texture that scrolled with the use of a sine wave, creating a flowing 'energy field'. As for the modelling, I focussed mostly on the arena and its stand(s). I kept the field architecture simple and clean, to not distract the players. The only feature the field offers is an indication on which side the player belongs. Both field assets and stand assets were made modular.

For all sounds I used FMOD to add some random modulation to pitch and volume. I made my own custom FMOD class which handled all audio for me, which I for example used for the player's jetpack. Making it so that the volume and pitch of the jetpack were dependent on the jetpack's energy.



<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm">
          <video muted autoplay loop style="height: 100%;  width: 100%;  overflow:hidden;    display:block;">
   <source type="video/mp4" src="https://i.imgur.com/pcssafq.mp4">
    </div>
    <div class="col-sm" style="margin-top: 20px">
    <h6>Shader</h6>
        As we took Rocket League as an inspiration, the team wanted a similar crowd. I invested some time in creating a billboard shader to recreate such a crowd. It worked out nicely, I used a small script to assign each 'egg' a different color from it's team color range.
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


As for the sounds themselves, I tried to give them an electric feeling, as the ball itself contained electricity and sparks.

{% capture carousel_images %}
https://i.imgur.com/NC1ma1K.png
https://i.imgur.com/V3eEasw.png
https://i.imgur.com/ghhyJuA.png
https://i.imgur.com/mKEuze0.png
{% endcapture %}
{% include elements/carousel.html %}

---
title: Flubber! Squash and stretch
tags: [Shaders]
style: 
image: https://jekyllrb.com/img/logo-2x.png
color: dark 
description: Creating a squash and stretch shader for a jelly
---

Squash and strech are one of the [twelve basic principles of animation](https://en.wikipedia.org/wiki/Twelve_basic_principles_of_animation) that were introduced by Disney. By applying squash and strech we add more *weight* and *flexibilty* to an object. And what has extreme flexibilty that can easily give an exaggerated, if not almost comical, effect? Flubber! 

As a good practise to keep going on with shaders, and especially Unity's shadergraph which I have not touched yet, it is time to create a basic squash and strech shader. 

##### Fundementals
To create the illusion of squad and stretch, I want to use the object's velocity to maniuplate the mesh's vertices. So if an object starts to move I want to move the vertices into the opposite direction of where the object is going. Of course I do not want to move the entire mesh, but primarily the vertices that are the highest in the object's space, kind of resembling skewing. 

However, skewing wont give enough of a squash and stretch impression on its own, given it will only work on on the horizontal axis. Therefore we would also need something on the vertical axis, which can be as simply as adding to the position 


Horizontal movement
<div class="container" style="padding: 0px">
  <div class="row" style="margin-bottom: 20px;">
    <div class="col-sm-6">
        <img src="https://i.imgur.com/fE1yxvo.png"/>
        <center><small>Stationary</small></center>
    </div>
    <div class="col-sm-6">
        <img src="https://i.imgur.com/sojrQu2.png"/>
        <center><small>Object moving left</small></center>
    </div>
    <div class="col-sm-6 ">
        <img src="https://i.imgur.com/moG9fjG.png"/>
         <center><small>Object moving right</small></center>
    </div>
    <div class="col-sm-6">
        <img src="https://i.imgur.com/5WVQaWN.png"/>
        <center><small>Object moving up</small></center>
    </div>
    <div class="col-sm-6">
        <img src="https://i.imgur.com/daNsa6V.png"/>
         <center><small>Object moving down</small></center>
    </div>
  </div>
</div>

##### Programming
To start off with, we need the **velocity** of the object. There are two options; using the [Rigibody's velocity](https://docs.unity3d.com/ScriptReference/Rigidbody-velocity.html), if it has one, or to calculate the difference between the current position and the position on the previous frame.

Calculating the transform
```csharp
Vector3 velocity = transform.position - _previousPosition / Time.deltaTime;
_previousPosition = transform.position;
```
Getting the velocity straight from the rigidbody
```csharp
velocity = _rigidBody.velocity;
``` 

To have a more streamlined approach, we could oblige to both by checking if an object has an rigidbody
```csharp
Vector3 _previousPosition;
Rigidbody _rigidBody;

private void Awake()
{
    _rigidBody = GetComponent<Rigidbody>();
}

public Vector3 GetVelocity()
{
    if (_rigidBody && !_rigidBody.isKinematic)
    {
        return _rigidBody.velocity;
    }
    else
    {
        return CalculateVelocity();
    }
}

public Vector3 CalculateVelocity()
{
    Vector3 velocity = transform.position - _previousPosition / Time.deltaTime;
    _previousPosition = transform.position;
    return velocity;
}
``` 

##### Shader
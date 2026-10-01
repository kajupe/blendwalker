---
title: Blender Basics
parent: Getting Started
layout: default
nav_order: 20
authors:
  - key: fioh
    role: "Guide-Writer"
  - key: kaj
    role: "Editor"
is_wip: true
---

# Blender Basics
{: .fs-9 .no_toc }
How to navigate blender in a step by step tutorial, controls, pages, what things do, what are you looking at when you open things
{: .fs-6 .fw-300 }

---

In this section, I will take you step by step in written and video format through the basics!  
Take your time here and take a moment to *practice* these concepts. With practice comes muscle memory, which will allow you to create even faster!

## Basic Navigation and Movement

Starting with where we left off in the previous section, "From Nothing to Something":  
We have our WoL on screen, and we have their Rig in POSE MODE!

A good start, but what does that even mean? And how do we even look around?  
To start here is a VITAL note: YOUR CURSOR'S LOCATION ON THE SCREEN MATTERS. For example, pressing "N" can mean and do different things if your cursor is hovering over different sections of the screen, so keep that in mind!

Now for this section, let's figure out how to navigate the VIEWPORT; the main screen where you can see your model!

* Rotate around focus point ⇒ Hold Middle Mouse Button + Drag
* Zoom ⇒ Mouse Wheel Scroll **OR** Alt + Middle Mouse Button + Drag
* Pan the camera ⇒ Shift + Middle Mouse Button + Drag
* Frame the Selected object ⇒ Numpad .

{: .highlight }
Keybinds and navigation methods can be adjusted in `Edit > Preferences > Keymap`. You might want to change keybinds like the Frame Selected one since it's one that's very handy to have easily accessible, especially if you don't have a Numpad.

<div style="padding:53.96% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1231891149?badge=0&amp;autopause=0&amp;player_id=0&amp;portrait=0&amp" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy" style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe></div>
<!-- <script src="https://player.vimeo.com/api/player.js"></script> -->

<br>

Those were the basic controls for you to navigate the viewport! Now, let's get into how to start posing your character!

1. "Model" vs "Rig"
2. Object Mode vs Pose Mode (Ctrl + Tab w/ Rig Selected)
3. Basic Posing Controls (G, R, RR, S)
4. Rotate to Camera (R) vs Rotate on Gimbal (RR)
5. Reset the Pose (Alt+G, Alt+R, Alt+S)

<div style="padding:53.96% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1231891140?badge=0&amp;autopause=0&amp;player_id=0&amp;portrait=0&amp" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy" style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe></div>

<br>

Practice those controls! Try out some poses!<br>When you're ready, continue on to some more advanced controls:

1. Advanced Posing Controls
2. Locking Movements to Axis (X, Y, Z)
3. Lock Movements Excluding an Axis (Shift+X, Shift+Y, Shift+Z)
4. Global vs Local Axis (Very Basic)
5. Elbows and Knees, and where they point
6. Fingers Closing, Making a Fist
7. Hiding Bone Collections
8. Skirt/Dress Bones
9. Hiding the Overlays for a Cleaner Shot

<div style="padding:53.96% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1231891135?badge=0&amp;autopause=0&amp;player_id=0&amp;portrait=0&amp" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy" style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe></div>

<br>

Now, let's go beyond just the character and explore Blender's other capabilities!

1. Basic Lighting and Camera Controls
2. Rendered View (Eevee)
3. How to Add Objects to a scene (Shift+A)
4. 3D Cursor Manipulation (Shift+RClick)
5. Changing Light Intensities and Basic light Setup
6. Object Duplication (Shift+D)
7. Camera Setup and Positioning

<div style="padding:53.96% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1231891133?badge=0&amp;autopause=0&amp;player_id=0&amp;portrait=0&amp" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy" style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe></div>

<br>

Wild! At this point, you can actually render out a whole pose for your character!<br>
Let's explore what this all looks like in an example session, while going over some other capabilities!

1. Locking a Weapon to your hand/different bones.
2. Example Pose Session
3. Movement Controls (Median Point vs Individual Controls)
4. Light Color Changing
5. Importing Environments (Talk through, show later)

<div style="padding:53.96% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1231891122?badge=0&amp;autopause=0&amp;player_id=0&amp;portrait=0&amp" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy" style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe></div>

<br>

Alrighty, say if we wanted to make an animation and then render it out, how is that done?

1. Basic Animation Keyframing (I) and Automatic keying
2. Rendering
3. Render Image vs Render Animation
4. Render Settings
5. File Outputs
6. Pros and Cons of PNG Sequence or MP4

<div style="padding:53.96% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1231891120?badge=0&amp;autopause=0&amp;player_id=0&amp;portrait=0&amp" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy" style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe></div>

<br>

Let's say we wanna put him in an environment? How do we do that?

1. Importing Environments
2. Environment Optimization and Setup
3. Empties vs Meshes
4. Outliner Organization and Collections

{: .note }
This video is from an older guide, but nothing regarding these things has changed substantially since it was made. It will just feel a little different.

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1231891119?badge=0&amp;autopause=0&amp;player_id=0&amp;portrait=0&amp" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy" style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe></div>

<br>

Next, we are going even further beyond!

1. Animation Import
2. Focus Object Solo View (Numpad /)
3. Armature Modifier
4. Joining Objects (Ctrl+J)
5. Dangers of moving models without the rig while it is still attached to the rig
6. Attaching a model to a new rig
7. Consider, if you are making a video using an FF14 model, an FF14 Environment and an FF14 Animation, why use Blender? Is it easier than in-game? Does it look better?

<div style="padding:53.96% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1231891121?badge=0&amp;autopause=0&amp;player_id=0&amp;portrait=0&amp" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy" style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe></div>

<br>

Incredible job! You have basically completed a project! You imported a character and environment, posed them, added in lighting and camera and rendered it out!

Remember these fundamentals, but this won't be all you need. 

Before you move on! Take a read through the "Start a Project" Section immediately, before doing anything else. 

This will help you prepare for what's next and help you avoid stagnation, especially after you put in all this work already.
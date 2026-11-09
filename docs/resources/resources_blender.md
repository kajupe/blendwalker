---
title: Blender Tools
parent: Resources
layout: default
nav_order: 10
---

# Blender Tools
{: .no_toc }
These are additions to Blender that will make it easier to work with FFXIV rigs, materials, or models.

- TOC
{:toc}

## FFXIV Blender Plugins Master Repository
<div class="custom-tags">
    <div class="custom-tag unique">Unique</div>
</div>
This isn't a singular resource, rather a collection of all the FFXIV-specific ones you're likely to need. This repository makes it so you only have to go to one place rather than each individual repository.  
[GitHub Repo & Installation Guide](https://github.com/ShinoMythmaker/FFXIV-Blender-Plugins)

## Meddle Tools
<div class="custom-tags">
    <div class="custom-tag unique">Unique</div>
    <div class="custom-tag material">Material</div>
</div>
Meddle Tools is the backbone of importing anything that's been exported with Meddle. While you usually won't use this directly when importing Characters, it's what tools like [AetherBlend](#aetherblend) call upon.  
Meddle Tools also comes with materials that aim to replicate the look of in-game ones, for everything from skin to furniture.  
[GitHub Repo & Installation Guide](https://github.com/PassiveModding/MeddleTools)

## AetherBlend
<div class="custom-tags">
    <div class="custom-tag rig">Rig</div>
</div>
AetherBlend is the main addon you'll use for importing and rigging characters. It features a few panels for importing, applying Customize+ scaling to, rigging and animating characters.  
Upon import it can also apply optional features like a custom eye material or using [FFGear](#ffgear) materials.  
[GitHub Repo](https://github.com/ShinoMythmaker/Aetherblend) | [Website w/ Installation Guide](https://aetherblend.mythmaker-studio.com/index.html)

## FFGear
<div class="custom-tags">
    <div class="custom-tag material">Material</div>
</div>
FFGear is a Blender addon for handling FFXIV gear shading and applying dyes to them directly in Blender. It allows for easily setting up shaders for Meddle exports (but will also work with other methods, like if exporting from TexTools). It's meant to allow for more customizability after you've already exported a character.  
While the materials that come with Meddle Tools can be good enough for your needs, FFGear's materials—which are made specifically for gear—will usually look better and are easier to make adjustments to. It's optional but highly recommended.  
[GitHub Repo & Installation Guide](https://github.com/kajupe/FFGear)
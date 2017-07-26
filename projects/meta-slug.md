---
layout: project
type: project
image: images/metal-slug1.jpg
title: Metal Slug
permalink: projects/metal-slug
date: 2016
youtubeId: 85yrW6rgm-s
labels:
  - Java
  - Sprite
  - Eclipse
summary: Metal slug themed sprite 2D shooter game written in Java.
---
### Project Overview
The objective of the game is to destroy the enemies and reach the end of the map. Enemies have set health and also shoot projectiles at the user. There are 8 types of enemies which all have unique projectiles, sounds, and death animations. These include both land and flying units. Sprite animation and projectile explosion animations are also options. 

{% include youtubePlayer.html id=page.youtubeId %}

# Features
### Player
  * Move two dimensionally around map
    * `w` - Up
    * `a` - Left
    * `s` - Crouch
    * `d` - Right
    * `spacebar` - Jump
    
  * Attack
    * `j` - Knife
    * `k` - Shoot bullets
    * `l` - Shoot grenades
    
  * Other
    * Victory animations
    * Periodic reload animations
    
### Enemies
  * Units
    * Airship
    * Helicopter
    * Mecha Robot
    * Scientist
    * Tank
    * Reinforced Tank
    * UFO
    * Zombie Macro
  * Unique sound, projectile, and death animations for enemies

### Other
  * Side scrolling map 
  * Scoreboard
  * Player jump shoot
  * Player crouch shoot
  * Player shoot up
  * `p` - pause
  * `o` - resume
  
# Development 
The sound and image capability is powered by the [EZ Graphics Library](http://www2.hawaii.edu/~dylank/ics111/). The game is built on four classes. 
* Enemy
* Initializer
* Player
* Projectile

The Enemy class controls all functions and features relating to all enemies. The Initializer class controls background music, map generation, and the options screen. The Player class controls all actions involving the player such as collision, animation, and states. The Projectile class controls all projectiles for both the player and all enemies. 

Source: <a href="https://github.com/nathancy/Metal-Slug" target="_blank"><i class="large github icon"></i>https://github.com/nathancy/Metal-Slug</a>

Video demo: <a href="https://www.youtube.com/watch?v=85yrW6rgm-s" target="_blank"><i class="large youtube icon"></i>https://www.youtube.com/watch?v=85yrW6rgm-s</a>


---
layout: project
type: project
image: images/starcraft2-mini-game-logo.png
title: Starcraft 2 Mini Game
permalink: projects/starcraft2-mini-game
date: 2016
youtubeId: --b-9HrKK6w
labels:
  - Java
  - Sprite
  - Eclipse
summary: Starcraft 2 themed sprite 2D shooter game written in Java.
---
### Project Overview
The objective of the game is to destroy all of the units and avoid the buildings. There are 20 units and 20 buildings. Destroying units increase points while hitting buildings decrease points. The player loses the game if the points drop to zero. With each additional kill, the aura of the mothership becomes larger.

{% include youtubePlayer.html id=page.youtubeId %}

# Features
#### Player
  * Move two dimensionally around map (`w, s, a, d`)
  * Three player skins (battlecruiser, leviathan, and mothership)
   * Unit hit detection
      * Ability to shoot projectile to kill units (`k`)
      * Ability to kill units by contact
  * Increasing aura with each kill
 
#### Units
  * Rotating aura
  * Randomly moves across map
  * Unique sound for each unit 
  * Unique death animation
  * +1 point for each kill
  
#### Buildings
  * Rotating aura
  * Teleports player to random location on contact
  * Unique contact sound
  * -1 point for each contact

#### Sound
Two music tracks (`0` and `9` to switch music)
  
#### Skins
There are three skins available to the user. The user can switch between the skins with `1`, `2`, or `3`.

# Development 
The sound and image capability is powered by the [EZ Graphics Library](http://www2.hawaii.edu/~dylank/ics111/). The game is built on two classes.
 * Buildings
 * Units
 
 The Buildings class controls all functions and features relating to buildings while the Units class controls all features involving the units.

Source: <a href="https://github.com/nathancy/Starcraft2-Mini-Game" target="_blank"><i class="large github icon"></i>https://github.com/nathancy/Starcraft2-Mini-Game</a>

Video demo: <a href="https://www.youtube.com/watch?v=--b-9HrKK6w" target="_blank"><i class="large youtube icon"></i>https://www.youtube.com/watch?v=--b-9HrKK6w</a>
---
layout: project
type: project
image: images/micromouse1.jpg
title: Micromouse Simulator 
permalink: projects/micromouse-simulator
date: 2017
youtubeId: Nb8YTFCTzjM
labels:
  - C 
  - Simulator 
  - Embedded Firmware 
summary: Developed a 16x16 Micromouse simulator using a predefined maze display with four levels. 
---
### Project Overview
Micromouse is a small autonomous robot whose task is to navigate a 16x16 maze and compete with other mice to find the center of the maze in the fastest time. The purpose of this project was to build a software tool to allow development of navigation algorithms. The simulator consists of a 16x16 grid of "cells" with walls that span from one post to another in which mice cannot escape the playing field. 

{% include youtubePlayer.html id=page.youtubeId %}

### Rules
The mouse starts in the "start cell", in the lower left corner facing North. The mouse's goal is the "center square" which consists of four cells at the center of the maze. There is only one entrance to the center square. The mouse knows nothing else about the configuration of the maze when it starts other than its location and the location of the center square. Although in a real competition, the fastest run from the start cell to the center square is the mouse's "run time", this simulator will not be concerned about time, only navigation through the maze, finding a path to the center, and counting the cells and unique cells visited. 

### The Details
The simulator contains four levels.

#### Level 0. Drive the Mouse
At Level 0, the maze is predetermined and visible to the user. In addition, the simulator keeps track of the X and Y coordinates as it moves. The mouse has no intelligence and is directly controlled by the user with the following commands:

* w - move forward one cell
* s - move backwards one cell
* a - turn left
* d - turn right
* Entire maze is visible 

<img class="ui centered image" src="../images/level0.JPG">

#### Level 1. The Mouse Discovers
At Level 1, the user has the same movement commands as in Level 0, as well as the additional commands:

* r - right wall hugger
* l - left wall hugger
* m - show the full maze (cheat)
* Cell counter 
* Mousecam

Level 1 provides a "cheat" command to reveal the full configuration of walls in the maze. The simulator keeps track of the mouse's position in the maze and adds a count of how many cells the mouse has visited. In addition, the user has a "mousecam" which shows the mouse's view of the walls on its left, right, and front sides. Level 1 also detects crashes into the walls and allows the user to restart at the start square. 

<img class="ui centered image" src="../images/level1.JPG">

#### Level 2. The Mouse Explores
The user may use all above commands with the addition of:

* n - hide the unknown maze (uncheat)
* Unique cell count

This command allows the user to "peak" at the maze using the 'm' command and then hide the unknown walls again using the 'n' command. In addition, the simulator also shows a count of traversed "unique" cells.

<img class="ui centered image" src="../images/level2.JPG">

#### Level 3. Da Frills
The user may use all above commands and the space command:

* space - random movement (drunken mouse)

Additional frills:

* Default level is 0
* A new maze map
* Hidden easter eggs 

<img class="ui centered image" src="../images/level3.JPG">

Source: <a href="https://github.com/nathancy/Micromouse-simulator"><i class="large github icon"></i>https://github.com/nathancy/Micromouse-simulator</a>

Simulator demo: <a href="https://www.youtube.com/watch?v=Nb8YTFCTzjM"><i class="large youtube icon"></i>https://www.youtube.com/watch?v=Nb8YTFCTzjM</a>

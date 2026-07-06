# Retro-Fred

Retro-Fred is a modern port of the classic ZX Spectrum video-game Fred. Fred is one of the first video-games created in Spain for the Sinclair ZX Spectrum microcomputer. It was developed in 1983 by Fernando Rada, Paco Menéndez and Carlos Granados and distributed by Indescomp. It was licensed, together with Bugaboo (The Flea) by Quicksilva near the end of 1983. It was first published in the United Kingdom, and shortly after in Spain by Investrónica. Retro-Fred is also available in C++, with support for Linux, Windows and Android platforms (https://github.com/8bitfred/retro-fred).

Graphics and sound effects from the original game are copyright to the original authors of Fred.

See the project's scratch page at https://scratch.mit.edu/projects/1053158449. Visit https://www.8bitfred.com for more information.

## The game

Escape from the pyramid and discover its treasures. Find the exit at the top level of the maze while avoiding deadly creatures and collecting objects. You can shoot your gun to scare ghosts away, make mummies disappear and kill vampires and skeletons.

The objective of the game is to reach the exit of the pyramid, located in the top level. The game has 6 levels of increasing difficulty. Each level has more and more difficult enemies:

* Ghosts: they can go through the maze walls. They cannot be killed, but when they are shot they change the direction of movement.
* Rats: they move laterally. Fred must jump vertically to avoid them. They cannot be killed.
* Acid drops: run quickly to avoid getting hit by them.
* Mummies: they walk slowly on the horizontal passages and fall quicky down the vertical corridors. They disappear when they get hit by a bullet, and reappear in a different location.
* Chameleons: they walk on the side of the vertical corridors and jump from one side to the other.
* Vampires: they fly in the maze and change directions randomly. They can be killed by shooting them.
* Skeletons: they walk on the horizontal corridors and climb up and down the ropes, trying to follow Fred. They die when hit by a bullet.

## Objects

There are different types of objects that Fred can collect inside the maze:

* Treasures: they are worth 500 to 1500 points, plus extra bonuses when you reach the exit.
* Power-up: increases the power level.
* Ammo-up: recharges the number of bullets to the maximum level.
* Map: shows a map of the section of the map near Fred. The corridors are shown in white and the walls in blue.

After finishing a level you will get 5000 points, and 1000 bonus point for each treasure collected during the game; and your power will increase by 2 units.

## Files

`Retro-Fred_121.sb3` is the standard implementation that closely reproduces the original reverse-engineered Z80 code.

### Auto-Fred

Auto-Fred is a version of Fred in which Fred’s movements are controlled automatically to guide him to the exit. It uses Dijkstra’s algorithm to find the shortest path as well as infinite power mode.

There are three implementations of Auto-Fred:

A. `Auto-Fred_Dijkstra_recursive.sb3` (a recursive implementation)

B. `Auto-Fred_DepthFirst.sb3`

C. `Auto-Fred_Right-Hand.sb3`

### Debug map

The `slDebugMap.txt` file contains the contents of the `slDebugMap` list from the `Map` sprite in plain text format. It can be imported into the Scratch project for debugging purposes.

### Scratch code

`ScratchCodePDF.zip`, `ScratchCodeSVG.zip`, `Auto-Fred_ScratchCodePDF.zip`, and `Auto-Fred_ScratchCodeSVG.zip` contain the Scratch code in PDF and SVG formats.

### Audio and video 

The `audio.zip` archive contains the sound effects in WAV format, and the `sprites.zip` archive contains the sprites in PNG format.

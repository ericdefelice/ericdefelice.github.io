---
layout: post
title: Building an Engine and Game
categories: game-development programming
---
I have started development on my game engine (and building a game using it).  The plan is to create a full featured 3D game engine from scratch using minimal libraries.  The engine features will include a rendering engine (using DirectX), audio processing (with DirectAudio or XAudio), gamepad support (using XInput), a physics engine, and animation support.  The game I am creating with the engine is currently designed to be an action RPG game with some minor puzzle solving, mainly used to introduce more complicated logic and systems into the game.


## Current status
For the past couple of months I have been building up the core engine functionality.  Things like displaying polygons to the screen, getting keyboard and mouse input, the ability to play audio files, 2D rendering support, etc.  Then I started making a small tech demo using many of the engine components while adding a few others.  Through this exercise I added procedurally generated terrain, support for multiple textures, simple movement physics, and various shaders.  Here is a screenshot of that small demo:

{% include figure.html src="/assets/tech_demo_01.png" caption="Engine Tech Demo" %}

This was a good start and many of the initial features I wanted in the engine, but it wasn't quite the game that I had in mind.  So I decided to start creating a new game with the engine, aptly named "Dungeon Crawler".  As you can tell, I spent quite a while think of game names. :)  In all honesty, that was the first thing that popped into my mind, so I am going with it for now until I have some time to dig more into the game design and decide upon a more proper game title.  For the game functionality, I currently have a player entity with some simple physics based movement and a procedurally generated game world.  I can move the player around the map, but there is no collision yet.  Here is a screenshot of the current state of the game:

{% include figure.html src="/assets/dungeon_crawler_01.png" caption="Current Dungeon Crawler Status" %}


## The development plan
As I stated earlier, I am planning on making an action RPG game with some puzzle solving aspects.  I'm kind of thinking of a mix of dual-stick shooter style gameplay, some RPG style player progression, and some Resident Evil influenced puzzles (where there are locked doors that require items to get through).  These are obviously long term goals for the game as a whole, so my plan is to have many milestones throughout the development.  These milestones will be related to engine functions or gameplay features at first, and then may include optimizations in the future.  For example, I have just finished implementing procedural map generation, and my current implementation is alright for now, but later on, I would like to store the map tiles using a hash table as opposed to a vector.  There is really no need for this now, but if I needed to find a particular tile, for say collision detection, I now have to search through them.  This is an optimization that I would like to make, but I'll leave that for a later time when it makes sense and is more necessary.

That small example shows the main core of my engine and game design philosophy.  I am going to try to get most of the features into the game as quickly as I can, but they will probably be in a rough state to start with.  As I see how the various systems interact and how the APIs should be, I can then begin refining and optimizing them.  I mainly started this project so that I can learn about many of the systems that are needed in a game engine, so if I feel like I have a good understanding of one of those systems, I may not spend as much time on it.


## Whats next?
I have a large list of features that I would like to add to the game, but in the near term, I want to improve the player movement to support rotation (right now the player entity just moves but doesn't rotate), add gamepad support, and get an initial collision detection system in the game.  Once these things are added, I'd like to add enemies and a simple attack to start getting the entity interactions in the game and to be able to start testing how different systems work with one another.  I'll probably end up working on some shaders mixed in there as well, since I find that fun and it is rewarding to see a game that looks better.

As for the blogging side of things, I am planning on writing posts that describe various aspects of the engine or game design, such as the map generation algorithm, or the rendering engine.  Until then, the game code is up on my github here: [https://github.com/ericdefelice/Dungeon_Crawler](https://github.com/ericdefelice/Dungeon_Crawler).

Oh, and one last thing.  You may have noticed that my player character is currently a red rectangle.  Well, I am no artist, so while I may get a better player model in the future, it may not be any prettier.  Also, the red guy is starting to grow on me, so I'm beginning to like the idea of having a red rectangle player with perhaps blue or green enemies of a similar shape.  A design decision for another day though.

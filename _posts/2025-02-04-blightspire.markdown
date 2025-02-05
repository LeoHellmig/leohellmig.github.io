---
layout: post
title: Blightspire
date: 2023-06-14 00:00:00 +0100
description: Blightspire is a game developed in a student made custom game engine. # Add post description (optional)
img: rays-cave.png # Add image post (optional)
tags: [C++, FMOD, ] # add tag

team_size: 10
platforms: Steam Deck & Windows
duration: 16 out of 32 weeks

---

Blightspire is currently still in development.
It is halfway through its development cycle and is starting its production phase soon.

So far the focus has been on the engine which the game will be built on top of.

The game targets the steam deck as its main platform. But the game will most likely be playable on Windows machines as well.
Because of this the team decided to make use of CLion as our IDE and CMake as our build system.

The building blocks of the engine are:

- Application/window
- Input
- Audio
- Ecs
- Inspector / Editor
- Gameplay
- Physics
- Renderer
- UI
- Scripting
- Steam integration

Tools used alongside the engine:

- Tracy profiler
- Radeon GPU Profiler
- Renderdoc

My contributions:

- Audio system
- ECS Integration
- Gameplay programming
- Engine programming
- Adding Tracy profiler

# My Contributions

## ECS Integration ⚙️

💡 *Using EnTT for convenience and familiarity*

### Key Features & Challenges

- Integrated EnTT into the engine to suit our current and future needs in the engine. 
- Designed and implemented a **Scene hierarchy system** through the use of components. Which allows for hierarchical relationships and transformations between entities.
- Implemented an entity editor window using Dear ImGui

🎥 [Before and after content]

🛠 Technologies: C++, EnTT, Dear ImGui

## Audio System 🎵

🚀  *Designed, iterated and implemented a robust and performant audio system using FMOD*

### Key Features & Challenges

- Integrated FMOD into the engine for **3D spatialized sound** and dynamic audio effects
- Developed an **event-driven system** to handle sound playback efficiently
- Debugged and optimized audio playing issues, for seamless audio playing

🎥 [Audio Showcase]
🛠 Technologies: C++, FMOD, ECS


## Gameplay programming 🎮

🔥 *Developed core system to aid in gameplay programming*

### Key Features & Challenges

- Implemented various systems to aid in future gameplay programming
- Created scripting bindings for various modules to extend the Engine API in scripts

🎥 [Gameplay demos]
🛠 Technologies: C++, ECS

## Engine Programming 🛠️

⚡ *Extending the engine's architecture for modularity and extendability*

### Key Features & Challenges

- Integrated Tracy Profiler in the engine
- Inspector module for inspecting and altering values on the fly
- Collaborated on **modular engine architecture**

🛠 Technologies: C++, Tracy, Dear ImGui



Stay tuned for the future game that will reside on this page.
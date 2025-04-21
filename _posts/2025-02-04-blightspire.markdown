---
layout: post
title: Custom Engine & Blightspire
date: 2024-09-02 00:00:00 +0100
description: Blightspire is a game developed in a student made custom game engine. # Add post description (optional)
img: Blightspire1.png # Add image post (optional)
tags: [C++, Custom Engine, FMOD, CMake, Tracy profiler, EnTT, Gameplay] # add tag

team_size: 10
dps: 1
prs: 9
vas: 0
platforms: Steam Deck & Windows
duration: 24/32 weeks
---

Blightspire is being created in our WIP custom engine.
It is 75% through its development cycle and is in its production phase.

We built a custom engine and are working to create a game on top of it.

The game targets the steam deck as its main platform. But the game will most likely be playable on Windows machines as well.
Because of this the team decided to make use of CLion as our IDE and CMake as our build system.

The engine is open source 😀 -> [Github repository](https://github.com/BredaUniversityGames/Y2024-25-PR-BB)

# My Contributions

## ECS Integration ⚙️

*Using EnTT for efficiency, convenience and familiarity*

### Key Features & Challenges

- Integrated EnTT into the engine to suit our current and future needs in the engine. 
- Designed and implemented a **Scene hierarchy system** through the use of components. Which allows for hierarchical relationships and transformations between entities.
- Integrated an entity editor window using Dear ImGui

<img src="../assets/img/BlightSpireECS.png" max-width="100%" height="auto">

🛠 Technologies: C++, EnTT, Dear ImGui

## Audio System 🎵

*Designed, iterated and implemented a robust and performant audio system using FMOD*

### Key Features & Challenges

- Integrated FMOD into the engine for **3D spatialized sound** and dynamic audio effects
- Debugged and optimized audio playing issues, for seamless audio playing
- The game uses **FMOD Events** for audio almost exclusively.

<video class="project-media" max-width="100%" height="auto" controls title="Title">
    <source src="../assets/vid/BlightSpireAudio.mp4" type="video/mp4">
</video>

🎥 [Audio Showcase]
🛠 Technologies: C++, FMOD, ECS, CMake

## Gameplay programming 🎮

*Developed core systems to aid in gameplay programming*

### Key Features & Challenges

- Implemented various systems to aid in future gameplay programming.
- Created **scripting bindings** for various modules to extend the **Engine API in scripts**
- Used Wren **scripting** to create **gameplay features**. 
- Player weaponry & abilities, camera, enemy movement, enemy state machine.

<video class="project-media" max-width="100%" height="auto" controls title="Title">
    <source src="../assets/vid/BlightSpireEnemy.mp4" type="video/mp4">
</video>

🛠 Technologies: C++, ECS, Wren

## Engine Programming 🛠️

*Extending the engine's architecture for modularity and extendability*

### Key Features & Challenges

- Integrated **Tracy Profiler** in the engine
- Inspector module **debug tool** for inspecting and altering values on the fly
- Collaborated on **modular engine architecture**

<img src="../assets/img/BlighspireInspector.png" max-width="100%" height="auto">

<img src="../assets/img/TracyProfiler.png" max-width="100%" height="auto">

🛠 Technologies: C++, Tracy, Dear ImGui, CMake

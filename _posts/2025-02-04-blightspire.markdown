---
layout: post
title: Blightspire
date: 2024-09-02 00:00:00 +0100
description: Blightspire is a game developed in a student made custom game engine. # Add post description (optional)
img: Blightspire.png # Add image post (optional)
tags: [C++, FMOD, CMake, Tracy, EnTT ] # add tag

team_size: 10
platforms: Steam Deck & Windows
duration: 16 weeks so far

---

Blightspire is currently still in development.
It is halfway through its development cycle and is starting its production phase soon.

So far the focus has been on the engine which the game will be built on top of.

The game targets the steam deck as its main platform. But the game will most likely be playable on Windows machines as well.
Because of this the team decided to make use of CLion as our IDE and CMake as our build system.

The engine is open source 😀 -> [Github repository](https://github.com/BredaUniversityGames/Y2024-25-PR-BB)

# My Contributions

## ECS Integration ⚙️

💡 *Using EnTT for efficiency, convenience and familiarity*

### Key Features & Challenges

- Integrated EnTT into the engine to suit our current and future needs in the engine. 
- Designed and implemented a **Scene hierarchy system** through the use of components. Which allows for hierarchical relationships and transformations between entities.
- Integrated an entity editor window using Dear ImGui

<img src="../assets/img/BlightSpireECS.png" max-width="100%" height="auto">

🛠 Technologies: C++, EnTT, Dear ImGui

## Audio System 🎵

🚀  *Designed, iterated and implemented a robust and performant audio system using FMOD*

### Key Features & Challenges

- Integrated FMOD into the engine for **3D spatialized sound** and dynamic audio effects
- Debugged and optimized audio playing issues, for seamless audio playing

<video class="project-media" max-width="100%" height="auto" controls title="Title">
    <source src="../assets/vid/BlightSpireAudio.mp4" type="video/mp4">
</video>

🎥 [Audio Showcase]
🛠 Technologies: C++, FMOD, ECS, CMake

## Gameplay programming 🎮

🔥 *Developed core systems to aid in gameplay programming*

### Key Features & Challenges

- Implemented various systems to aid in future gameplay programming
- Created scripting bindings for various modules to extend the Engine API in scripts

🛠 Technologies: C++, ECS

## Engine Programming 🛠️

⚡ *Extending the engine's architecture for modularity and extendability*

### Key Features & Challenges

- Integrated Tracy Profiler in the engine
- Inspector module for inspecting and altering values on the fly
- Collaborated on **modular engine architecture**

<img src="../assets/img/BlightspireModules.png" max-width="100%" height="auto">

<img src="../assets/img/BlighspireInspector.png" max-width="100%" height="auto">

🛠 Technologies: C++, Tracy, Dear ImGui, CMake



Stay tuned for the future game that will reside on this page.
---
layout: post
title: Coral Engine
date: 2023-06-14 00:00:00 +0100
description: Coral Engine is a custom made C++ engine by a group of 6 students. # Add post description (optional)
img: coral-engine.png # Add image post (optional)
tags: [C++, Engine, Animation, Gameplay] # add tag

team_size: 6
platforms: Windows & PS5
duration: 8 weeks

---

<div class="post-video-container" style="display:flex; flex-direction: row; justify-content: center; align-items: center">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/Z4UFHaJ_ulQ?si=1LSgzoy8_2Ge7DN0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

Coral Engine is a custom engine created by 6 students. 

Contributions:
- Audio
- Animations
- Gameplay
- UI 

[Link to github repository](https://github.com/GuusKemperman/CoralEngine)


# My Contributions

## Model loading 🔃

💡 *Refactoring model loading using Assimp*

### Key Features & Challenges

- Integrated Assimp to replace TinyGLTF allowing for more file formats to be loaded.
- Working around and learning the asset loading and management system present in the engine.
- Serializing 3D models using Cereal and the custom binary serializer already present

🎥 [Before and after content]

🛠 Technologies: C++, GSON, Assimp, Cereal

## Animations 🔧

💡 *Importing, loading, calculating and rendering animated models*

### Key Features & Challenges

- Importing animated meshes in the existing framework
- **Robust animations system** for calculating bone matrices in animated meshes
- **ECS integration** for Hierarchical animated models
- Reflected components for access to animations in scripting 
- Extending the rendering pipeline for **DX12 and PS5** to render animated meshes 
- Support for **animation blending** and attaching entities to animated bones

🎥 [Before and after content]

🛠 Technologies: C++, EnTT, Assimp, DirectX 12, PS5 renderer, hlsl

## Audio Module 🎵

💡 *Integrated FMOD for audio playback*

### Key Features & Challenges

- **Integrated and FMOD** in the engine. Allowing for audio playback.
- Implemented an audio system and components in the ECS to be usable in the game.
- Bound functions to allow for playing audio through the visual scripting.
- Efficient handling of sounds and events.

🎥 [Before and after content]

🛠 Technologies: C++, EnTT, FMOD

## Gameplay ⚔️

💡 *Implementing gameplay*

### Key Features & Challenges

- Camera and player movement
- Tweaking and making player movement feel and look good
- 

🎥 [Before and after content]

🛠 Technologies: C++, Visual Scripting 
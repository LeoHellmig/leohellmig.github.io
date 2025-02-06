---
layout: post
title: Ray's Cave
date: 2023-02-19 00:00:00 +0100
description: Ray's Cave is a game rendered in my own 2D raytracer. # Add post description (optional)
img: rays-cave.png # Add image post (optional)
tags: [C++, Raytracing] # add tag

team_size: Solo
platforms: Windows
duration: 8 weeks

---

## Introduction

Raytracing is more commonly associated with 3D rendering techniques. However in this project I explored how to apply this in a 2D space. Casting rays and detecting obstacles to render a scene with shadows and reflections in real time **on the CPU** using many optimizations.

## How I did this

### Shadows and reflections

Shadows are the absence of light, and are created by occluding a pixel from light. Seeing if a pixel is shadowed the ray traced to it has to intersect with an obstacle.

Reflections add more complexity to this. Needing to check if a light reflected in a reflected surface can reach the pixel unobstructed. 

![alt text](../assets/img/rays-cave-reflection-diagram.png)

### Grid

Tracing a ray to every light source from every pixel was very much hurting performance. A solution I found to this problem was to implement a **light grid** in view space. This grid holds handles to the lights that are influencing each cell by tracing rays. **Eliminating redundant ray tracing** and **reducing computation per pixel**.

### BVH

To achieve shadows I needed to test a ray for intersections with obstacles. Performing intersection for every ray on every object in the scene was not an efficient way to go about this. 
I followed a series of blog posts by my lecturer Jacco Bikker on **implementing a BVH** to spatially partition and check only relevant objects. [Link to the posts](https://jacco.ompf2.com/2022/04/13/how-to-build-a-bvh-part-1-basics/) 

### Performance

By implementing optimizations like the spatial partitioning from grids and BVHs. I was able to achieve a playable frame-rate and keep the rendering in real-time.

A large boost to performance came from moving the computations to multiple cores by adapting my code to utilize OpenMP.

## Challenges

- Precision issues in intersections -> solved using floating-point epsilon corrections
- Performance -> **Spatial partitioning**
- Possible performance increases -> Adapting code to run in multiple threads

## Results

<img src="../assets/img/rays-cave-render.png" max-width="100%" height="auto">

<img src="../assets/img/rays-cave-reflection.png" max-width="100%" height="auto">


<div class="post-video-container" style="display:flex; flex-direction: row; justify-content: center; align-items: center">
  <video muted autoplay loop style="margin:10px">
    <source src="../assets/vid/rays-cave.mp4" type="video/mp4">
  </video>
</div>


<div class="post-video-container" style="display:flex; flex-direction: row; justify-content: center; align-items: center">
  <video muted autoplay loop style="margin:10px">
    <source src="../assets/vid/rays-cave2.mp4" type="video/mp4">
  </video>
</div>



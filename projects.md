---
layout: page
title: Projects
permalink: /projects/
---

## GPU Programming
Projects written primarily in CUDA to take advantage of the GPU for accelerations and optimizations:

<div style="display: flex; align-items: flex-start; gap: 2em;">
  <img src="../images/gpu_pathtracer.png" style="width:300px; border-radius:10px;"/>
  <div>
    <h3><a href="https://github.com/anya0402/Project3-CUDA-Path-Tracer">CUDA GPU Path Tracer - October 2025</a></h3>
    <ul>
      <li>Built a GPU-accelerated pathtracer using CUDA and C++, supporting multiple material shaders, antialiasing, and more.</li>
      <li>Integrated bounding volume hierarchy acceleration to optimize loading .OBJ files, creating a 9x speedup for large meshes.</li>
      <li>Added the ability to make fast and complex renders with texture mapping, and stream compaction for path termination.</li>
    </ul>
  </div>
</div>

<div style="display: flex; align-items: flex-start; gap: 2em;">
  <img src="../images/boids.png" style="width:300px; border-radius:10px;"/>
  <div>
    <h3><a href="https://github.com/anya0402/Project1-CUDA-Flocking">CUDA Boids Flocking Simulator - September 2025</a></h3>
    <ul>
      <li>Developed a real-time, optimized flocking simulation on the GPU using CUDA, based on the Reynolds Boids algorithm.</li>
      <li>Implemented spatial-partitioning algorithms for memory coherence, resulting in a speedup from quadratic to linear time.</li>
      <li>Used CUDA event timers and NVIDIA NSight platforms to analyze and evaluate performance of flocking simulations.</li>
    </ul>
  </div>
</div>

<div style="display: flex; align-items: flex-start; gap: 2em;">
  <img src="../images/stream_compaction.png" style="width:300px; border-radius:10px;"/>
  <div>
    <h3><a href="https://github.com/anya0402/Project2-Stream-Compaction">Stream Compaction - September 2025</a></h3>
    <ul>
      <li>Implemented stream compaction on the GPU using CUDA, based on the <a href="https://developer.nvidia.com/gpugems/gpugems3/part-vi-gpu-computing/chapter-39-parallel-prefix-sum-scan-cuda">NVIDIA GPU Gems 3</a> book.</li>
      <li>Designed a work-efficient scan to use for stream compaction, using up-sweep and down-sweep phases to reduce redundant parallel work and creating a 2.5x speedup from the naive scan.</li>
      <li>Used NVIDIA Nsight Systems and Nsight Compute to analyze memory and kernel performance.</li>
    </ul>
  </div>
</div>



## Computer Graphics
Various coding projects created in the realm of graphics:

![image](../images/cbbunny.png){: style="float: left; margin-right: 3em; width: 200px"}
### [CPU Path Tracer - March 2024](pathtracer/index.html)
- Used bounding volume hierarchy algorithm to accelerate ray intersections with triangles and spheres. 
- Rendered images using global illumination (direct/indirect lighting), and optimized using Monte Carlo probability.

![image](../images/clothsim.png){: style="float: left; margin-right: 3em; width: 180px"}
### [Cloth Simulator - April 2024](clothsim/index.html)
- Utilized mass and spring system to create a cloth simulation and its corresponding collisions with other objects.
- Created Blinn-Phong, bump, displacement, texture, and other shaders for the cloth using the OpenGL API.

![image](../images/cowmesh.png){: style="float: left; margin-right: 3em; width: 200px"}
### [Mesh Edit - March 2024](meshedit/index.html)
- Built Bezier curves using algorithms such as the de Casteljau algorithm
- Implemented loop subdivision for mesh upsampling — creating more mesh subdivisions to smoothen the mesh

![image](../images/rasterized.png){: style="float: left; margin-right: 3em; width: 200px"}
### [Rasterizer - February 2024](rasterizer/index.html)
- Incorporated supersampling to have less aliasing in images with jagged pixel edges
- Gained an understanding of Barycentric coordinates by creating a color wheel using the necessary formulas

&nbsp;



-------
## Animation
-------
&nbsp;

3D-animated short films created with the software Autodesk Maya:

### [Stuffed Animal](https://youtu.be/mdOORVKXDkY?si=koPNOIb7yRLtryYw)

### [The Balloon](https://youtu.be/Jz7I77bFW84?si=AmPSNPBZ2hq-0p8H)
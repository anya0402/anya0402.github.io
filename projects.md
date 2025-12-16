---
layout: page
title: Projects
permalink: /projects/
---

<style>
.project-card {
  display: flex;
  gap: 1.5rem;
  margin: 2.5rem 0;
  align-items: flex-start;
}

.project-media {
  flex-shrink: 0;
  width: 280px;
}

/* Images */
.project-media img {
  width: 100%;
  height: 220px;
  border-radius: 10px;
  object-fit: cover;
}

/* Videos get more space */
.project-media.video {
  width: 360px;
}

.project-media.video iframe {
  width: 100%;
  height: 203px; /* 16:9 for 360px width */
  border-radius: 10px;
}

.project-content h3 {
  margin: 0;
}

.project-content a {
  text-decoration: none;
}

.project-date {
  font-weight: normal;
  font-size: 0.9rem;
  color: #777;
  margin-left: 0.5rem;
}

.project-content ul {
  padding-left: 1.2rem;
  margin: 0.75rem 0 0 0;
}

@media (max-width: 768px) {
  .project-card {
    flex-direction: column;
  }

  .project-media {
    width: 100%;
    max-width: 420px;
  }
}

.section-header {
  margin-top: 4.5rem;
  margin-bottom: 2rem;
  padding: 1.4rem 1.6rem;
  border-radius: 12px;
  background-color: #f2f5ff;
  border: 2px solid transparent;
}

.section-header h2 {
  margin: 0;
}

.section-header p {
  margin: 0.4rem 0 0 0;
  font-size: 0.95rem;
  color: #444;
}

.section-header.gpu {
  background-color: #eef3ff;
  border-color:rgb(152, 169, 210);
;
}

.section-header.graphics {
  background-color: #eef8f1;
  border-color: #4caf50;
}

.section-header.animation {
  background-color: #fff2e8;
  border-color: #ff8c42;
}


</style>



<div class="section-header gpu">
  <h2>GPU Programming</h2>
  <p>High-performance rendering and simulation using CUDA and modern GPU APIs.</p>
</div>

<div class="project-card">
  <div class="project-media">
    <img src="../images/glremix.png" alt="glRemix" />
  </div>
  <div class="project-content">
    <h3>
      <a href="https://github.com/glRemix/glRemix">
        glRemix
      </a>
      <span class="project-date">Dec 2025</span>
    </h3>
    <ul>
      <li>Created a DirectX 12 platform to remaster OpenGL 1.0 apps with real-time path tracing without touching its source code.</li>
      <li>Intercepted OpenGL calls with a shim layer, and used interprocess communication to send to DX12 renderer.</li>
      <li>Implemented features such as asset replacement during runtime, texture and environment mapping, and shadow maps.</li>
    </ul>
  </div>
</div>

<div class="project-card">
  <div class="project-media">
    <img src="../images/gpu_pathtracer.png" alt="CUDA Path Tracer" />
  </div>
  <div class="project-content">
    <h3>
      <a href="https://github.com/anya0402/Project3-CUDA-Path-Tracer">
        CUDA GPU Path Tracer
      </a>
      <span class="project-date">Oct 2025</span>
    </h3>
    <ul>
      <li>Built a GPU-accelerated pathtracer using CUDA and C++, supporting multiple material shaders, antialiasing, and more.</li>
      <li>Integrated bounding volume hierarchy acceleration to optimize loading .OBJ files, creating a 9x speedup for large meshes.</li>
      <li>Added the ability to make fast and complex renders with texture mapping, and stream compaction for path termination.</li>
    </ul>
  </div>
</div>

<div class="project-card">
  <div class="project-media">
    <img src="../images/splats.png" alt="WebGPU Gaussian Splats" />
  </div>
  <div class="project-content">
    <h3>
      <a href="https://github.com/anya0402/Project5-WebGPU-Gaussian-Splat-Viewer">
        WebGPU Gaussian Splats
      </a>
      <span class="project-date">Nov 2025</span>
    </h3>
    <ul>
      <li>Built a real-time Gaussian Splat renderer using the WebGPU API, to create realistic and fast interactive 3D scenes.</li>
      <li>Transformed point cloud data into blended ellipsoids with calculated position, color, opacity, and size attributes.</li>
      <li>Set up pipelines for GPU parallelism, including a compute shader for covariance, frustum culling, depth sorting, etc.</li>
    </ul>
  </div>
</div>


<div class="project-card">
  <div class="project-media">
    <img src="../images/webgpu.png" alt="WebGPU rendering demo" />
  </div>
  <div class="project-content">
    <h3>
      <a href="https://github.com/anya0402/Project4-WebGPU-Forward-Plus-and-Clustered-Deferred">
        WebGPU Forward+ and Clustered Deferred Shaders
      </a>
      <span class="project-date">Oct 2025</span>
    </h3>
    <ul>
      <li>Used the WebGPU API and implemented Forward+ and Clustered Deferred shading pipelines to optimizing the processing of several dynamic lights.</li>
      <li>Integrated geometry-buffer optimizations and clustering for light culling, resulting in an average of 25x speedup.</li>
      <li>Achieved an average 25× lighting performance speedup.</li>
      <li>
        <a href="https://anya0402.github.io/Project4-WebGPU-Forward-Plus-and-Clustered-Deferred/">
          View a live demo here!
        </a>
      </li>
    </ul>
  </div>
</div>


<div class="project-card">
  <div class="project-media">
    <img src="../images/boids.png" alt="CUDA Boids simulation" />
  </div>
  <div class="project-content">
    <h3>
      <a href="https://github.com/anya0402/Project1-CUDA-Flocking">
        CUDA Boids Flocking Simulator
      </a>
      <span class="project-date">Sep 2025</span>
    </h3>
    <ul>
      <li>Developed a real-time, optimized flocking simulation on the GPU using CUDA, based on the Reynolds Boids algorithm.</li>
      <li>Implemented spatial-partitioning algorithms for memory coherence, resulting in a speedup from quadratic to linear time.</li>
      <li>Used CUDA event timers and NVIDIA NSight platforms to analyze and evaluate performance of flocking simulations.</li>
    </ul>
  </div>
</div>


<div class="project-card">
  <div class="project-media">
    <img src="../images/stream_compaction.png" alt="Stream compaction visualization" />
  </div>
  <div class="project-content">
    <h3>
      <a href="https://github.com/anya0402/Project2-Stream-Compaction">
        GPU Stream Compaction
      </a>
      <span class="project-date">Sep 2025</span>
    </h3>
    <ul>
      <li>Implemented stream compaction on the GPU using CUDA, based on the NVIDIA GPU Gems 3 book.</li>
      <li>Designed a work-efficient scan to use for stream compaction, using up-sweep and down-sweep phases to reduce redundant parallel work and creating a 2.5x speedup from the naive scan.</li>
      <li>Used NVIDIA Nsight Systems and Nsight Compute to analyze memory and kernel performance.</li>
    </ul>
  </div>
</div>




<div class="section-header graphics">
  <h2>Computer Graphics Introduction</h2>
  <p>CPU-based rendering, simulation, and OpenGL graphics pipelines.</p>
</div>

<div class="project-card">
  <div class="project-media">
    <img src="../images/cbbunny.png" alt="CPU Path Tracer render" />
  </div>
  <div class="project-content">
    <h3>
      <a href="pathtracer/index.html">CPU Path Tracer</a>
      <span class="project-date">Mar 2024</span>
    </h3>
    <ul>
      <li>Used bounding volume hierarchy algorithm to accelerate ray intersections with triangles and spheres.</li>
      <li>Rendered images using global illumination (direct/indirect lighting), and optimized using Monte Carlo probability.</li>
    </ul>
  </div>
</div>

<div class="project-card">
  <div class="project-media">
    <img src="../images/clothsim.png" alt="Cloth simulation" />
  </div>
  <div class="project-content">
    <h3>
      <a href="clothsim/index.html">Cloth Simulator</a>
      <span class="project-date">Apr 2024</span>
    </h3>
    <ul>
      <li>Utilized mass and spring system to create a cloth simulation and its corresponding collisions with other objects.</li>
      <li>Created Blinn-Phong, bump, displacement, texture, and other shaders for the cloth using the OpenGL API.</li>
    </ul>
  </div>
</div>

<div class="project-card">
  <div class="project-media">
    <img src="../images/cowmesh.png" alt="Mesh editing project" />
  </div>
  <div class="project-content">
    <h3>
      <a href="meshedit/index.html">Mesh Edit</a>
      <span class="project-date">Mar 2024</span>
    </h3>
    <ul>
      <li>Built Bezier curves using algorithms such as the de Casteljau algorithm</li>
      <li>Implemented loop subdivision for mesh upsampling — creating more mesh subdivisions to smoothen the mesh</li>
    </ul>
  </div>
</div>

<div class="project-card">
  <div class="project-media">
    <img src="../images/rasterized.png" alt="Rasterizer output" />
  </div>
  <div class="project-content">
    <h3>
      <a href="rasterizer/index.html">Rasterizer</a>
      <span class="project-date">Feb 2024</span>
    </h3>
    <ul>
      <li>Incorporated supersampling to have less aliasing in images with jagged pixel edges</li>
      <li>Gained an understanding of Barycentric coordinates by creating a color wheel using the necessary formulas</li>
    </ul>
  </div>
</div>



<div class="section-header animation">
  <h2>Animation</h2>
  <p>3D animated short films created using Autodesk Maya.</p>
</div>

<div class="project-card">
  <div class="project-media video">
    <iframe
      src="https://www.youtube.com/embed/mdOORVKXDkY"
      title="Stuffed Animal"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen>
    </iframe>
  </div>
  <div class="project-content">
    <h3>
      <a href="https://youtu.be/mdOORVKXDkY">Stuffed Animal</a>
    </h3>
  </div>
</div>

<div class="project-card">
  <div class="project-media video">
    <iframe
      src="https://www.youtube.com/embed/Jz7I77bFW84"
      title="The Balloon"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen>
    </iframe>
  </div>
  <div class="project-content">
    <h3>
      <a href="https://youtu.be/Jz7I77bFW84?si=IfykeQFD6aNO4-bY">The Balloon</a>
    </h3>
  </div>
</div>
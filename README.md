# webgpu-ocean
A real-time 3d fluid simulation implemented in WebGPU. Works on your browsers which support WebGPU. 

[Try demo here!](https://webgpu-ocean.netlify.app/)

![demo image](https://github.com/matsuoka-601/webgpu-ocean/blob/main/img/webgpu-ocean-demo.gif)

The following are the characteristics of the simulation.
- The simulation is based on Smoothed Particle Hydrodynamics (SPH) described in [Particle-Based Fluid Simulation for Interactive Applications](https://matthias-research.github.io/pages/publications/sca03.pdf) by Müller et al.
  - Compute shader is used for implementing SPH. 
- Screen-Space Rendering described in [GDC 2010 slide](https://developer.download.nvidia.com/presentations/2010/gdc/Direct3D_Effects.pdf) is used for rendering the fluid.
  - Vertex/fragment shader is used for implementing Screen-Space Rendering.
- For fast neighborhood search on GPU, an algorithm described in [FAST FIXED-RADIUS NEAREST NEIGHBORS: INTERACTIVE MILLION-PARTICLE FLUIDS](https://ramakarl.com/pdfs/2014_Hoetzlein_FastFixedRadius_Neighbors.pdf) is used. 

# Terrain Generation

**A 3D terrain visualization project exploring procedural generation, noise algorithms, shader programming, and realistic terrain rendering.**

Academic project developed during the *Visualization & Illumination I* course at the University of Minho (2020/2021), as part of the Computer Graphics specialization.

## Overview

This project explores procedural terrain generation and rendering using GLSL shaders.

The application generates terrain elevation through noise-based algorithms and applies different textures according to terrain height, creating visually distinct landscapes.

It also incorporates lighting calculations, normal mapping, and configurable rendering parameters to explore different terrain appearances.

## Tech Stack

| Area | Technologies |
|---|---|
| Shader Programming | GLSL 3.30 |
| Graphics | OpenGL-compatible rendering pipeline |
| Procedural Generation | Simplex Noise, Fractal Brownian Motion (fBm) |
| Rendering | Vertex & Fragment Shaders |
| Texturing | Height-based Texture Blending, Normal Mapping |
| Configuration | XML |

## Terrain Visualizations

The project includes two scenes demonstrating different terrain textures and visual appearances.

![Terrain Scene 1](scene0.PNG)

![Terrain Scene 2](scene1.PNG)

## Key Features

- **Procedural Terrain Generation** — Noise-based height generation using Simplex Noise and Fractal Brownian Motion.
- **Height-Based Texturing** — Different terrain textures applied according to elevation.
- **Texture Blending** — Smooth transitions between low, intermediate, high, and water regions.
- **Normal Mapping** — Surface detail enhancement through configurable normal maps.
- **Dynamic Lighting** — Directional lighting calculations with adjustable time parameters.
- **Configurable Parameters** — Controls for terrain height, noise scale, texture repetition, and lighting properties.
- **Multiple Terrain Scenes** — Two alternative texture configurations.

## Implementation

### Procedural Height Generation

The vertex shader calculates terrain elevation by displacing the vertices of a grid.

Two height-generation approaches are supported:

- Sampling from a noise texture.
- Procedural generation using fractal noise.

The procedural approach combines multiple noise frequencies through Fractal Brownian Motion to produce terrain variations.

### Terrain Texturing

The fragment shader selects and blends textures according to terrain elevation.

Different texture sets are used for water, low-altitude, intermediate, and high-altitude regions.

Normal maps are incorporated into lighting calculations to enhance surface detail.

### Lighting

The rendering pipeline uses directional lighting and surface normals to calculate illumination.

A configurable time parameter influences the light direction, allowing different lighting conditions to be explored.

## Concepts Explored

- Procedural content generation.
- Shader programming and vertex displacement.
- Noise-based terrain modelling.
- Texture mapping and blending.
- Surface normals and lighting calculations.
- Real-time graphics rendering.

## Project Context

Developed as a group assignment at the University of Minho during the 2020/2021 academic year.

The repository preserves the original shader implementation, rendering configuration, textures, and visual results.

###### By [@HCHexY](https://github.com/HCHexY) [@joanafonsogomes]( https://github.com/joanafonsogomes) [@LPFerreira33](https://github.com/LPFerreira33)

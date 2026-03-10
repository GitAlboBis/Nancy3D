# Nancy3D - For You ♡

## Overview
Nancy3D is a highly personalized, interactive 3D web experience designed as a romantic digital environment for my girlfriend. Built entirely with web technologies, it renders a romantic dinner scene accompanied by floating memories, custom particle effects, and a terminal-style introductory message. 

## Features
* **Terminal Typewriter Intro**: The application opens with a simulated terminal overlay that types out a romantic, personalized greeting before revealing the 3D scene.
* **Interactive 3D Environment**: Powered by Three.js (v0.160.0), the scene allows the user to rotate and zoom using `OrbitControls` with built-in auto-rotation when idle.
* **Procedural Materials & Textures**: Several visual elements are generated dynamically via the HTML5 Canvas API, including a pink romantic text background (used as a fallback), a red-and-white checkered tablecloth, and an intricate Indian-style mandala floor pattern.
* **Custom 3D Scene Composition**: 
  * The scene integrates external GLTF models including sushi bowls, wine glasses, a wine bottle, and a vase with flowers.
  * Custom geometry is constructed programmatically for items like dinner plates, silverware, custom roses, and animated flickering candles.
* **Memory Ring**: A rotating gallery of 10 Polaroid-style photo frames dynamically loads user images (`1.jpeg` through `12.jpeg` and `tavolo2.jpeg`) to float around the central table.
* **Advanced Particle & Visual Effects**:
  * Floating magical pink particles utilizing `AdditiveBlending`.
  * A spectacular background heart cloud constructed from 300 text sprites ("i love you") formatted along a 3D parametric heart equation, featuring pulsation and rotation animations.
  * Extruded 3D floating hearts bouncing gently above the dining area.

## Tech Stack
* **HTML5 / CSS3**: For layout structure and the terminal overlay styling.
* **JavaScript (ES6 Modules)**: Core logic and animation loop handling.
* **Three.js**: Used via CDN for all 3D WebGL rendering, lighting, shadows, and camera management.

## Directory & Asset Structure
To run the project successfully, ensure the following local assets and directories are present relative to the `index.html` file:

* `background.jpg`: Main background image (falls back to procedural canvas if missing).
* `bowl/sushi-bowl/scene.gltf`: 3D model for the left and right dining bowls.
* `sushi/sushi/scene.gltf`: Center sushi model.
* `glass/simple_glass_cup/scene.gltf`: 3D models for the wine glasses.
* `wine bottle/wine_bottle/scene.gltf`: Wine bottle model.
* `flowers/flowers_in_vase/scene.gltf`: Flower vase arrangement.
* **Gallery Images**: Files named `1.jpeg` through `12.jpeg` and `tavolo2.jpeg`, loaded onto the Polaroid frames in the Memory Ring.


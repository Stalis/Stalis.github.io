---
title: Pseudo 3D JS
description: A browser-based pseudo-3D engine with raycasting rendering and an ECS architecture.
status: active
stack:
  - TypeScript
  - ECSY
  - HTML Canvas
  - Webpack
repo: https://github.com/Stalis/pseudo-3d-js
demo: https://stalis.github.io/demos/pseudo-3d-js/
embedDemo: true
date: 2026-10-05
draft: false
---

<div class="demo" data-demo></div>

A small browser game engine that renders a pseudo-3D scene with `HTML Canvas`. Its renderer uses raycasting: for every ray, the camera finds a wall on the map and draws the corresponding vertical texture strip.

## What is included

- An ECS architecture built with ECSY, separating entities, components, and game systems by responsibility.
- Turn-based player movement and rotation.
- Textured walls, sprites, and character portraits.
- Separate engine, gameplay, and interface layers.

## Controls

| Action | Keys |
| --- | --- |
| Move forward / backward | `W` / `S` or `↑` / `↓` |
| Strafe left / right | `A` / `D` or `←` |
| Turn | `Q` / `E` |

The project is built with Webpack. To run it locally, use `npm install` and `npm start`.

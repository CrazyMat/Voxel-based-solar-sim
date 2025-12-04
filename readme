# Universal Earth Voxel Simulation (Beta)

Procedural voxel Earth. Dynamic core–mantle–crust layers. Atmosphere, ice, oceans, and a luminous sun – all running entirely in the browser.

This repository hosts an experimental planetary engine that treats Earth as a living voxel field rather than a static sphere, designed as a foundation for future orbital mechanics, spaceflight, and multi-body simulations. :contentReference[oaicite:0]{index=0}  

---

## ✨ Core Idea

**EARTH-10k** is a WebGL2 / Three.js simulation that:

- Builds a fully voxelized Earth (core → mantle → crust → ocean → atmosphere)
- Generates terrain, oceans, ice caps, and biomes via layered noise
- Uses instanced meshes + LOD for performance at high voxel counts
- Embeds Earth in a simple solar system with a radiant sun and orbital motion
- Exposes controls for time dilation, resolution, and layer visibility

The project is intentionally “systems-first”: it prioritizes structures that can later support realistic gravity, dark matter / dark energy fields, tectonics, and orbital navigation.

---

## 🔭 Features

### Planet Generation
- **Procedural voxel Earth** with configurable:
  - Base radius (in voxels)
  - Voxel size
  - Terrain noise scale
  - Water level
  - Atmosphere density :contentReference[oaicite:1]{index=1}  
- **Layered structure**:
  - **Core** (plasma) – glowing, pulsing inner light source
  - **Mantle** (magma) – convection-tinted voxels animated over time
  - **Crust** – land, ocean, ice, mountains, deserts, forests, grasslands
  - **Atmosphere** – gas shell with volumetric cloud-like voxels

### Biomes & Classification
The crust classifies surface voxels into a set of visually distinct biomes:

- Cryosphere (ice)
- Deep and shallow ocean
- Rainforest, forest, grassland
- Desert / sand
- Mountain rock and snowy peaks
- Mantle magma & core plasma
- Cloud and gas voxels in the atmosphere :contentReference[oaicite:2]{index=2}  

A **Legend panel** in the UI visually explains each class and its color.

### Solar System Context
- **Sun** voxel body at the origin, with:
  - Emissive instanced voxels for a granular solar surface
  - High-intensity point light to illuminate Earth
  - Subtle pulsation for “living star” feel
- **Earth orbit**:
  - Earth orbits the Sun on a circular path
  - Earth rotates on its axis for day/night cycles
  - View modes let you focus on Earth, the Sun, or the full system

### Performance & LOD
- Uses **`THREE.InstancedMesh`** for all voxel fields
- Builds:
  - A **high-resolution LOD** with internal and surface voxels
  - A **low-resolution LOD** with downsampled surface voxels only
- **LOD switching** via `THREE.LOD`: close = high detail, far = simplified :contentReference[oaicite:3]{index=3}  
- Basic occlusion culling: fully surrounded voxels are treated as internal and hidden in most views.

### Dynamic Simulation
- Adjustable **time dilation** (1x–1000x)
- Mantle convection “breathing” via color shifts
- Dynamic **water/ice cycle** based on latitude & global temperature drift
- Pulsing core light and sun intensity
- Atmospheric opacity subtly animates to simulate circulation/winds

---

## 🧰 Tech Stack

- **Three.js** (ES modules via CDN)
- **WebGL2** renderer
- **SimplexNoise** for terrain, ocean, and atmosphere patterns
- **Tailwind via CDN** for HUD styling
- Vanilla HTML / JS single-page app (no build step required) :contentReference[oaicite:4]{index=4}  
